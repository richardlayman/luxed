LuxEd
=======

Editor for LuxRender scene and config files.

![LuxEd](https://raw.githubusercontent.com/richardlayman/luxed/master/ui.png)

Introduction
---------------
LuxEd is a GUI editor for Lux scene and config files. It's intended for 3d artist that want to have full access to Lux's features without having to use Blender. The idea is to export your mesh data to ply or stl files and then use LuxEd to assemble the scene, shade and light it. LuxEd can then export the files for batch rendering. This breaks the connection with Blender allowing for a more diverse pipeline.

Installation
---------------
LuxEd is a single python file that you can run straight from the folder. You will need to have the LuxRays 1.6, Python 3.5, Qt 5.6 and PyQt5 installed. You might be able to get by with lower versions of Python and Qt but you should have the latest LuxRays since the API is changing constantly. LuxEd was developed and tested on Linux but should work fine on any other operating systems.

Currently Supported Features
---------------
- File IO
  * New Scene (bug: this will still show the last rendered image after a scene has been cleared)
  * Add Mesh
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
- Camera
- Objects
- Shapes
  * Mesh
- Materials
  * Matte
  * RoughMatte
  * Glossy2
  * Glass
  * ArchGlass
  * RoughGlass
  * MatteTranslucent
  * CarPaint
  * Cloth
  * Velvet
  * Mirror
  * Metal
  * Mix
  * Null
- Textures
  * UVMapping2D
  * ImageMap
  * Marble
  * Mix
  * Add
  * Substract
  * Band (bugged)
  * Brick
  * CheckerBoard3D
  * ConstFloat1
  * ConstFloat3
  * Dots
  * FBM
  * FresnelApproxK
  * FresnelApproxN
  * Scale
  * UV
  * HitPointAlpha
  * HitPointColor
  * HitPointGrey
  * HSV
  * Windy
  * Wood (bugged)
  * Wrinkled
  * ABS
  * Clamp
  * BlackBody
  * IrregularData
  * LampSpectrum
  * Blender\_Blend
  * Blender\_Clouds
  * Blender\_DistortedNoise
  * Blender\_Magic
  * Blender\_Noise
  * FresnelColor
  * FresnelPreset
  * FresnelSopra
  * FresnelLuxpop
- Lights
  * TODO
- Volumes
  * Clear
  * Homogeneous
  * Heterogeneous 
- Functionality
  * Add Node
  * Remove Node
  * Rename Node
  * Can change the rotation and field-of-view of the viewport camera with the mouse
  * Load multiple ply meshes that will get automatically setup with object, shape and material properties

Known Issues
---------------
When making scenes you may notice that objects are not showing up when loaded. This will happen when due to Lux render errors since the objects are being called with no mesh assigned yet. This is common if you add objects in the SceneLayout and then add the meshes later; lux will not show any of the objects until they have all been loaded. Currently LuxEd does not have a way of telling the user that Lux is failing so this can be a little confusing at first. I plan to add a feature in the future to let the user know that there are render errors.


