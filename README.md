# intro-to-unity-interface
[beginner] Unity Interface-User Interface, Vector, and Transform components

## Welcome to your first Unity Repo! 
This guide is going to be covering the basics of Unity from the different parts of the User Interface to learning basic concepts such as Vectors and Transformations.

Remember: Understanding the interface is key as a video game developer and should be second nature.  So refer back to this if you ever need help!

Happy gaming! 
## A Resource you should definitely check out
https://docs.unity3d.com/Manual/UnityManual.html

## Interface Overview

![Screenshot](https://raw.githubusercontent.com/junior-devleague/intro-to-unity-interface/master/assets/Interface.png?token=AVj6trmd6IxRPSy8lwEI2sW4Q4UU_3ofks5ZiWMEwA%3D%3D)

The Unity Interface is made of 6 seperate windows which are...
1. The Hierarchy Window
2. The Project Window
3. The Inspector Window
4. The Scene View
5. The Game View
6. The ToolBar

### The Hierarchy Window
The Hierarchy Window shows a list of all game objects in the scene.  Through the Hierarchy, game objects can be moved around and objects can be grouped to make Game Object families.  **NOTE:** Objects at the top are the parent while objects inside the parent are the child.

### The Project Window
The project window displays all assets we have available to build the game with.  It gives us easy access to files which include (but aren't limited to) 
* Scripts
* Textures
* 3D Models
* Audio Clips
* Scenes
  * Scenes are assets as well which are also saved and accessed through the project window

### The Inspector Window
The Inspector Window is a context sensitive window which shows us the properties of any object we want to see.  It also lets us add components to individual game objects.

### The Scene View
The Scene View is where we are going to visually build the game.  It allows us to visually interact with objects, adjusting the x, y, z or axis of any object, if needed.

### The Game View
The Game View allows us to preview our game in the editor.  By using the play controls in the toolbar we can play test the game at any time.

### The ToolBar
The Toolbar lets us view, pause, or step frame-by-frame through every scene.  It contains transform tools and gizmo toggles, play controls, controls for account and layout. 
*But, what are these?*
* Transform: Lets us manipulate objects
* Collab: Lets us download updates to the project that someone may have uploaded
* Layers: Lets us hide or show content in-game
  * You can create your own layers and layouts

### And that's it! 
...*Or is it?*

## A few concepts for you to understand

### Vector3 and Vector2
In game Development, Vectors are used to define meshes, directions, and all manners of calculations.  Which makes them *essential* to understand.  Simply, a vector is a **line between two points**.  The length of that line is called the **Magnitude**.  

#### Vector2D
