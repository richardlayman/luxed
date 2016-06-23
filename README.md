LuxEd
=======

Editor for LuxRender scene and config files.

![LuxEd](https://raw.githubusercontent.com/richardlayman/luxed/master/ui.png)

Introduction
---------------
LuxEd is a GUI editor for Lux scene and config files. It's intended for 3d artist that want to have full access to Lux's features without having to use Blender. The idea is to export your mesh data to ply or stl files and then use LuxEd to assemble the scene, shade and light it. LuxEd can then export the files for batch rendering. This breaks the connection with Blender allowing for a more diverse pipeline.

Installation
---------------
LuxEd is a single python file that you can run straight from the folder. LuxEd was developed and tested on Linux but should work fine on any other operating system.

Currently Supported Features
---------------
- File IO
  * New Scene (bug: this will still show the last rendered image after a scene has been cleared)
  * Import Scene
  * Export Render Config
  * Export Scene
- Render Settings
- Engine Type
  * PATHCPU
  * BIASPATHCPU
  * BIDIRCPU
  * PATHOCL
  * RTPATHOCL
  * BIASPATHOCL
  * RTBIASPATHOCL
- Sampler
  * SOBOL
  * METROPOLIS
  * RANDOM
- Filter
  * NONE
  * BOX
  * GAUSSIAN
  * MITCHELL
  * MITCHELL\_SS 
  * BLACKMANHARRIS
- Light Strategy
  * TODO
- Film
  * TODO 
- Objects/Shapes
  * Ply
- Materials
  * Matte
  * RoughMatte
  * Glossy2
  * Glass
  * ArchGlass
  * RoughGlass
  * MatteTranslucent
  * CarPaint
  * Velvet
  * Mirror
  * Metal
  * Mix
  * Null
- Textures
  * ImageMap
  * Marble
  * Mix
  * Scale 
- Lights
  * TODO
- Volumes
  * TODO
- Functionality
  * Add Node
  * Remove Node
  * Rename Node
