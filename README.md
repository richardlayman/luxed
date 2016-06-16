LuxEd
=======

Editor for LuxRender scene and config files.

![LuxEd](https://raw.githubusercontent.com/richardlayman/luxed/master/ui.png)

Introduction
---------------
LuxEd is a GUI editor for Lux scene and config files. It's intended for 3d artist that want to have full access to Lux's features without having to use Blender. The idea is to export your mesh data to ply or stl files and then use LuxEd to assemble the scene, shade and light it. LuxEd can then export the files for batch rendering. This breaks the connection with Blender allowing for a more diverse pipeline.

Installation
---------------
LuxEd is a single python file that you can run straight from the folder. Currently you manually add your objects and materials to the scene. LuxEd was developed and tested on Linux but should work fine on any other operating system.

Currently Supported Features
---------------
File IO
* Export Render Config
* Export Scene
Render Settings
Engine Type
* PATHCPU
Sampler
* Metropolis
Filter
* TODO
Light Strategy
* TODO
Film
* TODO 
Objects/Shapes
* Ply
Materials
* Matte
* Glossy2
* Glass
* MatteTranslucent
* Mirror
* Metal
* Mix
* Null
Textures
* TODO
Lights
* TODO
Volumes
* TODO
