# Getting to Know the Unity Interface
Basics of using the Unity3D game engine platform.

## Welcome to the Unity3D Interface!
This guide will cover the different parts of Unity's user interface and some basic game development concepts such as how to use Vectors and Transformations.

_**Remember:**_ Understanding the interface is key as a video game developer and should be second nature. So refer back to this if you ever need help!

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
![Screenshot](https://raw.githubusercontent.com/junior-devleague/intro-to-unity-interface/master/assets/2Dvector.png?token=AVj6tooFI3VXIiki2wOdkFYWtT5j0kAjks5ZiWbwwA%3D%3D)

A 2D Vector is a way of representing a point from the origin; the 0,0 point on the graph to any point on the 2D plane. *Ex. Above.* Since it is coming from the origin, it already has an implied direction and it is made up of only two components, **x** and **y**.

#### Vector 3D
![Screenshot](https://raw.githubusercontent.com/junior-devleague/intro-to-unity-interface/master/assets/3DVector.png?token=AVj6tlkTQVMXDTVOkBszLJkWgsYU9lHEks5ZiXTAwA%3D%3D)

A 3D Vector is similar to a 2D vector except for the fact that there is an added component known as **z** which represents depth.   The **x** and **z** axis make up the horizontal plane, while the **y** axis represents height.  Keep in mind that any coordinates represented in 3D will be in order **x, y, z**.  

![Screenshot](https://raw.githubusercontent.com/junior-devleague/intro-to-unity-interface/master/assets/LeftHand.png?token=AVj6tkV7RM5yYoh4gDnYhkn4qsh8MGKKks5ZiXR9wA%3D%3D)

*Another way to think of it is like this*

Unity runs on a Left Hand Rule Coordinate System.  This means if you hold your left hand with your index finger pointed upwards and your thumb pointed out, forming an L shape, and your middle finger pointing away from you then the thumb represents the **x-axis**, your pointer represents the **y-axis** and your middle finger is the **z-axis**.  

If you can understand this, you understand how depth, horizontal, and vertical works in Unity and how physics can be applied to them.  

### Transform

Before you understand what Transform is, you must first understand what a **GameObject** is.  A 3D Game Object is the standard building block in Unity, consider it like the dough to pizza.  These include shapes such as Cubes, Spheres, Capsules, Cylinders, Planes, and Quads.  Anytime you're creating a new item in Unity, you're instancing a new Game Object. Below is an example of a Cube GameObject in Unity. 

![Screenshot](https://raw.githubusercontent.com/junior-devleague/intro-to-unity-interface/master/assets/GameObjectCubeExample.png?token=AVj6tjAfpHJrLzH_KqqbI1cL4ctUsBG0ks5ZiYGQwA%3D%3D)

GameObjects are able to hold individual attributes which can modify a GameObject in many, many different ways.  You can see from the example above that the very first component added to the GameObject is **Transform** and the reason is that it is the default component that comes on all GameObjects.  

*The Unity definition of Transform is as so..*
![Screenshot](https://raw.githubusercontent.com/junior-devleague/intro-to-unity-interface/master/assets/UnityTransform.png?token=AVj6tloiMgC7-DU9NgHoUHgqCiLr7ZSuks5ZiYOmwA%3D%3D)

*So, you're probably asking, what is position, rotation, and scale?*

Positon, rotation and Scale are containers that store where that object is on the plane in respect to Origin (0, 0, 0).  

#### Position 

In a 3D object, using the Vector3D (formally called **Vector3** which stores the locations of the **x, y, and z** in the axis) we can adjust the coordinates of where the object is placed on the plane.  Doing so, will automatically update the Position's **x, y, and z** in the Transformer component.

#### Rotation

Rotation does not adjust the position of the Object, but simply the direction of it.  You are able to control the **x, y, and z** to face the object more left, right, up, or down.  Rotation is also useful for being able to control aiming from a first person point-of-view.

#### Scale

Scale is used to change the shape of the Object.  Using scale, we are able to create different size objects and different shapes.  Refer to the pictures for a visual example.

![Screenshot](https://raw.githubusercontent.com/junior-devleague/intro-to-unity-interface/master/assets/Sphere.png?token=AVj6tgpdrgpLzCTfEAHQ0aCCquqB-NHNks5ZiY--wA%3D%3D) 

**This is a sphere GameObject with a Transform.Scale property of (1, 1, 1)**

![Screenshot](https://raw.githubusercontent.com/junior-devleague/intro-to-unity-interface/master/assets/SphereAfterX.png?token=AVj6tqICmx4UQLWz0be2GPbvj2--sKBhks5ZiY_IwA%3D%3D) 

**Here is the same sphere after the object's x-axis was increased by 2 (3, 1, 1)**

![Screenshot](https://raw.githubusercontent.com/junior-devleague/intro-to-unity-interface/master/assets/SphereAfterXandZ.png?token=AVj6tmuSr3ys0cYHTG76VZZxyrw38IXjks5ZiY_RwA%3D%3D) 

**And here is the same sphere after the z-axis was shifted to 4 (3, 1, 4)**

As you can see, you are able to make GameObjects into different shapes, thus forming new objects that can be used wherever needed.  
