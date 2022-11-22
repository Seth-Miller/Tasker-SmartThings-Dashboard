# Tasker-SmartThings-Dashboard
Create SmartThings dashboards in Tasker.

## Create a scene
The tasks currently support one scene called ST Dashboard Scene 1. Create a scene with this title and add nine toggles and nine text boxes.

![Screenshot Tasker ST Dashboard Scene](https://user-images.githubusercontent.com/2525293/203192062-eeb8c9ca-9bd2-4977-bbd7-82ce9e8f8154.png)

Each toggle should be labeled Toggle1 and have the off and on labels updated to `%toggle_off_label(1)` and `%toggle_on_label(1)` respectively with the number reflecting the toggle number. Below each toggle should be a text box labeled with the same number and have the text `%textbox_text(1)`. See [this example](ST_Dashboard_Scene_1.scn) for more details

## Import tasks
Import the tasks from [TaskerNet](https://taskernet.com/shares/?user=AS35m8mZRcYt6YVVoQmlYHnB2eA6q3OQFVnQTIvHJy%2Fu1w22iXZPdD%2BREaNkg%2FYvYOAJBAoOYhM%3D&id=Project%3ASmartThings+Dashboards).

## Create Personal Access Token
Create a Personal Access Token (aka bearer token) in the [SmartThings API](https://developer.smartthings.com/docs/advanced/authorization-and-permissions/) and set the `%Bearer` global variable in Tasker to the value.

## Build Scene Content
Run the `ST Dashboard Build Scene` task to build the scene content. Keep in mind that this can take awhile to run if you have a lot of devices. Once complete, the global variable `%SliderButtons` will be created with content used by the scene.

## Run the Scene
Run the `ST Dashboard Run Scene` task to run the scene. Click the toggles to toggle your devices on and off.
