LuxEd
=======

Editor for LuxRender scene and config files.

![LuxEd](https://raw.githubusercontent.com/richardlayman/luxed/master/ui.png)

Introduction
---------------
LuxEd is a GUI editor for Lux scene and config files. It's intended for 3d artist that want to have full access to Lux's features without having to use Blender. The idea is to export your mesh data to ply or stl files and then use LuxEd to assemble the scene, shade and light it. LuxEd can then export the files for batch rendering. This breaks the connection with Blender allowing for a more diverse pipeline.

Installation
---------------
LuxEd is a single python file that you can run straight from the folder; it doesn't look for any other files or assets. LuxEd was developed and tested on Linux but should work fine on any other operating system.

Status
---------------
LuxEd is still a WIP and not officially released but you can mess with it some. An example file comes with the program and will startup as soon as you run it. There is still a lot of missing features and there will be crashes. If you want to use LuxEd for your own scenes, you'll have to edit your own render.cfg and scene.scn files and put them in the same folder as LuxEd - this will be fixed in the future so you won't have to do this.

