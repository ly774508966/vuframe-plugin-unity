# Vuframe Unity Plugin
![N|Solid](https://github.com/Vuframe/vuframe-plugin-unity/blob/master/Screenshots/header_sqr.png?raw=true)

The Vuframe Plug-In enables you to author interactive 3d content in Unity and publish it directly to the Vuframe platform. Please keep in mind that the plug-in is still in its beta phase.

You need to have a Vuframe Platform Account in order to use this. If you don't have one already, you can sign up here:
http://www.vuframe.com/signup

### Requirements (Compatibility)
Currently this version is compatible and tested with all versions between Unity 4.6.0 up to 5.5.1 At this time only Legacy shaders are supported in Unity 5.

You can download the latest supported version here:
- https://unity3d.com/de/get-unity/download/archive

Unity 5.5 and PBS-material Support is coming soon.
### Install
Launch Unity and open the project you have downloaded or cloned from Github. If you want to add the Unity Plug-In to an existing project, just copy the "Vuframe" folder into your Projects Assets Folder.
### Quickstart:
Add an empty Game Object, name it, click on the Component button and add the "Scene" Component. Add a mesh object (e.g. a Unity standard object) as a child object to your just created Game Object with the scene Component. Hit Play.

Note: The VFScene Component will only take child objects of your scene-object in account. Everything else in your Unity scene will not be exported or affected by the VFScene Component.

### Components
The Plugin consists of several Main Components. The most important ones are:
-  VFScene:
The Scene Component is the base for all operations and interactions you can use with the plug-in. Add an Empty GameObject
to your scene and click on "Add Component" in the Inspector Tab. Use the Filter and search for
Scene to find the component quickly. After you added the Scene Component, it will present you a lot of different settings for your scene. 

- Ego Trigger
Ego Triggers are used to move the camera into Ego Perspective. It is possible to move from one Ego Trigger to another. On a compatible smartphone, the Ego Perspective can be controlled by Touch or GyroScope and used with a Cardboard. 
To Create an Ego Trigger, just create an Empty GameObject and add a Ego Trigger Component.

The included example scenes will show you how to use these and other Components of the Plugin.

### Login
Open the Publishing Window (Window/Vuframe/Publishing) and click the "Login" Button. This will open a Login Dialog in a Browser Window. After you logged in with your platform credentials, a Token is shown in the Browser Window. Copy the Token into the Input Field in the Unity Publishing Window. Click "Save Auth Token" to finish.
### Publish
Save your Root Object (with the Scene Component) as a Prefab and select it. Open the Inspector and select the Cloud Project Folder you want to publish to. Click "Export & Publish" under "Publish" in the VFScene Component.
### Examples:
The Project contains 3 sample Scenes which show some of the basic functionality.
- Car
This scene is setup to open an close the doors by clicking on them, changing the tires by using the UI button
and getting to the drivers seat by using the Ego trigger.
- House
The house example features Variation Groups, Layouts, Event triggers as UI elements and Ego triggers to show
a virtual floor plan with different furniture layouts and a virtual tour. Click on the UI elements on the left to hide
and show the roof. Use the two buttons on the right to switch between the different furniture layouts.
- TV-Set
Our last example is a flat screen TV with 3 different sizes. It also shows additional information like a price-tag and
measurements. It uses layouts and Event Trigger as 3D elements.

### FAQ:
- How can I enable Augmented Reality?
Activate the "OnTable" Feature in the Inspector of your Scene Component.
- With which Unity Versions is this Plug-In compatible?
The Plug-In for now is compatible and tested with all Versions between Unity 4.6.0 and Unity 5.5.1. You can download it from the Unity
Download-Archive here: https://unity3d.com/de/get-unity/download/archive
- Do I need to have a Unity Plus license (or above) to use the Plug-In?
No, you can use the Plug-In with Unity Personal (free) within the limitations of your license of the compatible Version.
- Do I need the Example Scene in my Asset Folder to use the Plug-In?
No, you can delete the Examples Folder from your Asset.
- Which shaders are supported in the Plug-In?
For now we only support the following Shaders:
-- Unity 4:  only Standard Shaders
-- Unity 5:  only Legacy Shaders
- Why does the app crash when I open the 3D model?
Memory Issues, too large or too many textures, too large/complicated meshes.
- Is there an online documentation for the Unity Plugin?
Yes you can find it in our support platform https://vuframe.zendesk.com/hc/en-us/sections/115000265309-Unity-3D-Plugin 

### Known Issues:
- Unity 5 no support for Directional and Directional-Specular Lightmaps
- Unity 5 Normal maps exported wrong

### Screenshots:
- Scene in Editor
![N|Solid](https://github.com/Vuframe/vuframe-plugin-unity/blob/master/Screenshots/1.JPG?raw=true)
- Scene Inspector Window
![N|Solid](https://github.com/Vuframe/vuframe-plugin-unity/blob/master/Screenshots/2.JPG?raw=true)
- Publishing Window
![N|Solid](https://github.com/Vuframe/vuframe-plugin-unity/blob/master/Screenshots/3.JPG?raw=true)
- Scene in Playmode
![N|Solid](https://github.com/Vuframe/vuframe-plugin-unity/blob/master/Screenshots/4.JPG?raw=true)
- Scene with Ego Triggers
![N|Solid](https://github.com/Vuframe/vuframe-plugin-unity/blob/master/Screenshots/5.JPG?raw=true)
- Scene in Ego Perspective
![N|Solid](https://github.com/Vuframe/vuframe-plugin-unity/blob/master/Screenshots/6.JPG?raw=true)
