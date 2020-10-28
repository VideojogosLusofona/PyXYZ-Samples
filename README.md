# PyXYZ

PyXYZ (pronounced pyxies) is a a simple 3D wireframe engine for education, entirely programmed in Python, using only PyGame, NumPy and NumPy-Quaternion.

It is an object-oriented engine, with the main design focus on simplicity and ease of learning and extension, and has very little functionality out-of-the-box: it allows for the programmer to visualize a 3D scene using a virtual camera.

![alt text](https://github.com/DiogoDeAndrade/PyXYZ/raw/master/screenshots/terrain.png "Sample terrain application")

This repository has some some sample applications for the engine.

The engine can be retrieved from https://github.com/VideojogosLusofona/PyXYZ, and the documentation can be read on https://videojogoslusofona.github.io/PyXYZ/.

## Sample applications

All the sample applications implement an application loop. A window is open, the content is displayed there, and the user can quit by pressing the ESC quit or closing the window.

To run the samples, the "pyxyz" directory needs to be copied from the engine repository to
directory where the samples reside.

### Sphere (sample_sphere.py)

![alt text](https://github.com/DiogoDeAndrade/PyXYZ/raw/master/screenshots/sphere.png "Sample sphere application")

The simplest sample, it just creates a red sphere on the center of the viewport and rotates it slowly.

### Hierachy (sample_hierarchy.py)

![alt text](https://github.com/DiogoDeAndrade/PyXYZ/raw/master/screenshots/hierarchy.png "Sample hierarchy application")

This application demonstrates the use of hierarchies. Hierarchies can be created by adding objects as children of other objects. The PRS of child objects will be considered to be in local space (the space of the parent).

### Cube fall (sample_cubefall.py)

![alt text](https://github.com/DiogoDeAndrade/PyXYZ/raw/master/screenshots/cubefall.png "Sample cube fall application")

In this application, cubes are spawned on top of the screen and fall
down with gravity. This demonstrates one way of creating/destroing objects through the life cycle of the application.

It also shows the use of creating classes derived from Object3d (use of hierarchy-based extension instead of component-based)

### Terrain (sample_terrain.py)

![alt text](https://github.com/DiogoDeAndrade/PyXYZ/raw/master/screenshots/terrain.png "Sample terrain application")

This application generates a terrain based on a 2-octave Perlin noise, colors the generated polygons based on height and slope, and rotates the terrain in front of the camera.

This makes use of a helper 2d perlin generator that's part of PyXYZ.

### Missile Game (sample_game.py)

![alt text](https://github.com/DiogoDeAndrade/PyXYZ/raw/master/screenshots/game.png "Sample game application")

This is a sort of incomplete game: the player can shoot some missiles using the mouse, and it demonstrates user input and a more complex application loop. It also shows functionality like creating a mesh from different parts, converting a mouse position into a ray, sphere/sphere collision detection, target tracking and a rudimentary screen flash effect. The game is not complete, since it doesn’t have win/lose condition

## Licenses

All code in this repo is made available through the [MIT license].

## Metadata

* Autor: [Diogo Andrade][]

[Diogo Andrade]:https://github.com/DiogoDeAndrade
[MIT license]:(LICENSE)
