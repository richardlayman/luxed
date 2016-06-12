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

Status
---------------
I had to add a scenegraph to the program which broke it for a little bit but it's virtually back to it's original state. You can add objects, matte and glossy2 materials but that will change soon. There is also no access to the render settings but that too should be fixed soon.
