Changes list
============
- 1.11.0:
 - **Major updates**
 - New option for mesh: ```mesh.showBoundingBox``` to display mesh's bounding box. You can configure back and front color using ```scene.getBoundingBoxRenderer()```. This function returns a ```BABYLON.BoundingBoxRenderer``` where you can define ```backColor```, ```frontColor``` and ```showBackLines``` ([deltakosh](http://www.github.com/deltakosh))
 - New basic mesh: ```BABYLON.Mesh.CreateTorusKnot``` ([deltakosh](http://www.github.com/deltakosh))
 - New ```BABYLON.AnaglyphArcRotateCamera``` and ```BABYLON.AnaglyphFreeCamera``` ([michael-korbas](https://github.com/michael-korbas)), ([deltakosh](http://www.github.com/deltakosh))
 - Tags system ([gwenael-hagenmuller](https://github.com/gwenael-hagenmuller))
 - New render pipeline system for post-processes. See documentation [here](https://github.com/BabylonJS/Babylon.js/wiki/How-to-use-PostProcessRenderPipeline) ([michael-korbas](https://github.com/michael-korbas))
 - **Updates**
 - Added parameters to enable or disable a type of texture on all ```BABYLON.StandardMaterial``` ([demonixis](http://www.github.com/demonixis))
 - New ```BABYLON.VertexData.ExtractFromMesh``` function ([deltakosh](http://www.github.com/deltakosh))
 - Cameras can now have sub-cameras (see ```BABYLON.AnaglyphArcRotateCamera``` for example) ([deltakosh](http://www.github.com/deltakosh))
 - New ```BABYLON.Engine.runEvenInBackground``` property. True by default. It allows you to stop rendering when the browser is not the foreground application. ([deltakosh](http://www.github.com/deltakosh))
 - Darkness of a shadow + shadow on transparent meshes ([clementlevasseur](https://github.com/clementlevasseur))
 - New event for materials: ```onCompiled``` and ```onError``` ([deltakosh](http://www.github.com/deltakosh))
 - **Bugfixes**
 - Fixed a bug with collisions cache
 - Fixed a bug with mesh.dispose when called twice ([deltakosh](http://www.github.com/deltakosh))
 - Fixed an issue with Internet Explorer while rendering a RenderTargetTexture outside the engine renderLoop ([nicolas-obre](https://github.com/nicolas-obre))
 - **New demos*
 - [CYOS](http://www.babylonjs.com/cyos)
- 1.10.0:
 - **Major updates**
 - Virtual joysticks canera ([davrous](http://www.github.com/davrous))
 - Oculus Rift support ([davrous](http://www.github.com/davrous)), ([simonferquel](http://www.github.com/simonferquel)), ([deltakosh](http://www.github.com/deltakosh))
 - Support for DDS textures ([deltakosh](http://www.github.com/deltakosh))
 - Constructive solid geometries ([CraigFeldspar](https://github.com/CraigFeldspar))
 - Importer plugin system ([deltakosh](http://www.github.com/deltakosh))
 - Filter postprocess ([deltakosh](http://www.github.com/deltakosh))
 - Convolution postprocess ([deltakosh](http://www.github.com/deltakosh))
 - Added Cheetah3d exporter ([Calebsem](http://www.github.com/Calebsem))
 - New ```BABYLON.ShaderMaterial``` object to simply create custom shaders ([deltakosh](http://www.github.com/deltakosh)) - See [Custom shader - cell shading](http://www.babylonjs.com/index.html?CUSTOMSHADER)
 - New ```BABYLON.VertexData``` object to easily manipulates vertex attributes ([deltakosh](http://www.github.com/deltakosh)) - See [VertexData](http://www.babylonjs.com/index.html?CLOUDS)
 - **Updates**
 - Shaders can be loaded from DOM element alongside .fx files ([deltakosh](http://www.github.com/deltakosh))
 - Adding arcRotateCamera.wheelPrecision ([deltakosh](http://www.github.com/deltakosh))
 - Support for DOMMouseScroll ([nicolas-obre](https://github.com/nicolas-obre))
 - Adding BABYLON.PickingInfo.prototype.getNormal ([deltakosh](http://www.github.com/deltakosh))
 - Adding a new noMipmap parameter to ```BABYLON.CubeTexture``` constructor ([deltakosh](http://www.github.com/deltakosh))
 - Adding ```BABYLON.Color3.FromInts()``` and ```BABYLON.Color4.FromInts()``` ([deltakosh](http://www.github.com/deltakosh))
 - Adding invertY parameter to ```BABYLON.VideoTexture``` constructor ([deltakosh](http://www.github.com/deltakosh))
 - Adding new ```BABYLON.Scene.getCameraByID``` function ([deltakosh](http://www.github.com/deltakosh))
 - Adding new ```BABYLON.Scene.setActiveCameraByName()``` function ([deltakosh](http://www.github.com/deltakosh))
 - Renaming ```BABYLON.Scene.activeCameraByID()``` to ```BABYLON.Scene.setActiveCameraByID()``` ([deltakosh](http://www.github.com/deltakosh))
 - Adding texture wrapping support to Blender exporter ([vousk](http://www.github.com/vousk))
 - Add Gulp for buiding babylon cross platform ([SideraX](http://www.github.com/SideraX))
 - Shadow map improvement on pack method ([clementlevasseur](http://www.github.com/clementlevasseur))
 - **Bugfixes**
 - Fixing multimat naming convention in Blender ([deltakosh](http://www.github.com/deltakosh))
 - Fixing mesh.clone ([temechon](http://www.github.com/temechon))
 - Fixing camera rotation export in blender ([khmm12](http://www.github.com/khmm12))
 - Fixing opacity map bug ([deltakosh](http://www.github.com/deltakosh))
 - Fixing physics objects disposal ([deltakosh](http://www.github.com/deltakosh))
 - Using the hardware scaling when creating a ray ([demonixis](http://www.github.com/demonixis))
 - **New demos*
 - [Hill Valley](http://www.babylonjs.com/index.html?HILLVALLEY)
 - [Custom shader - cell shading](http://www.babylonjs.com/index.html?CUSTOMSHADER)
 - [Constructive solid geometries](http://www.babylonjs.com/index.html?CSG)
 - [Postprocess - Convolution](http://www.babylonjs.com/index.html?PPCONVOLUTION)
 - [VertexData](http://www.babylonjs.com/index.html?CLOUDS)
- 1.9.0:
 - **Major updates**
 - Beta support for scene serialization with ```BABYLON.SceneSerializer.Serialize``` function ([deltakosh](http://www.github.com/deltakosh))
 - Blender exporter now supports 32 bits indices ([deltakosh](http://www.github.com/deltakosh))
 - Flat shading support (From Blender and with ```mesh.convertToFlatShadedMesh()``) ([deltakosh](http://www.github.com/deltakosh))
 - **Updates**
 - New ```mesh.rotate``` and ```mesh.translate``` functions to rotate and translate mesh both locally and globally ([deltakosh](http://www.github.com/deltakosh))
 - New feature for particles: ```ParticleSystem.forceDepthWrite``` ([deltakosh](http://www.github.com/deltakosh))
 - Adding a new parameter to pick in order to be able to pick even on multi views ([deltakosh](http://www.github.com/deltakosh))
 - New ```mesh.lookAt``` function ([professorF](https://github.com/professorF))
 - New postprocess system (independent from cameras) ([michael-korbas](https://github.com/michael-korbas))
 - New ```mesh.setAbsolutePosition``` function ([gwenael-hagenmuller](https://github.com/gwenael-hagenmuller))
 - **Bugfixes**
 - Fixing issue with ```mesh.infiniteDistance``` ([deltakosh](http://www.github.com/deltakosh))
 - Fixing issue with camera caches ([deltakosh](http://www.github.com/deltakosh))
 - Fixing issue with aspect ratio ([deltakosh](http://www.github.com/deltakosh))
 - Fixing arcRotateCamera angle limitations ([deltakosh](http://www.github.com/deltakosh))
 - Fixing a bug with multi-views: depth buffer was not clear between different passes ([deltakosh](http://www.github.com/deltakosh))
- 1.8.5:
 - **Major updates**
 - Visual Studio 2013 templates for Windows 8.1 and nuget packages ([pierlag](http://www.github.com/pierlag))
 - **Updates**
 - New ```matrix.multiply``` function (up to 50% faster) ([deltakosh](http://www.github.com/deltakosh))
 - New matrices cache system for camera (view and projection matrices) ([juliengobin](http://www.github.com/juliengobin))
 - New physics impostor: compound and mesh (still really slow) ([deltakosh](http://www.github.com/deltakosh))
 - Set crossOrigin flag for support CORS ([vbouzon](http://www.github.com/vbouzon))
 - XNA importer: Changes for Right-Left Coordinate Systems & Prefixed Mesh Parts with Mesh Name ([professorF](http://www.github.com/professorF))
 - Fixing getPivotMatrix ([gwenael-hagenmuller](http://www.github.com/gwenael-hagenmuller))
 - New geometry functions: getLocalTranslation, setPositionWithLocalVector, getPositionExpressedInLocalSpace,locallyTranslate ([gwenael-hagenmuller](http://www.github.com/gwenael-hagenmuller))
 - Adding multi mesh import from same file([nicolas-obre](http://www.github.com/nicolas-obre)) 
 - **Bugfixes**
 - Fixing issue when disposing a parent and not its children ([deltakosh](http://www.github.com/deltakosh))
 - Fixing .obj importer ([deltakosh](http://www.github.com/deltakosh))
 - Added guardband checks for impostors' size ([deltakosh](http://www.github.com/deltakosh))
- 1.8.0:
 - **Major updates**
 - Support for [physics engine](http://www.babylonjs.com/index.html?PHYSICS) thanks to cannon.js ([deltakosh](http://www.github.com/deltakosh))
 - New [sandbox tool](http://www.babylonjs.com/sandbox/) ([davrous](http://www.github.com/davrous))
 - **Updates**
 - New ```animation.currentFrame``` property to get current animation frame ([deltakosh](http://www.github.com/deltakosh))
 - New ```animation.floatInterpolateFunction``` property to define custom float interpolation function ([deltakosh](http://www.github.com/deltakosh))
 - New ```animation.vector3InterpolateFunction``` property to define custom vector3 interpolation function ([deltakosh](http://www.github.com/deltakosh))
 - New ```animation.quaternionInterpolateFunction``` property to define custom quaternion interpolation function ([deltakosh](http://www.github.com/deltakosh))
- 1.7.3:
 - **Updates**
 - Support for "file://" moniker ([davrous](https://github.com/davrous))
 - Support for DAE (COLLADA) file format ([gwenael-hagenmuller](https://github.com/gwenael-hagenmuller))
 - Support for "empty" object type in Blender exporter ([deltakosh](http://www.github.com/deltakosh))
 - **Bugfixes**
 - "use strict" is no more included in minified version ([deltakosh](http://www.github.com/deltakosh))
 - Fixing a bug with MSGesture with IE11 on Windows 7 ([deltakosh](http://www.github.com/deltakosh))
- 1.7.0:
 - **Major updates**
 - Support for [lens flares](https://github.com/BabylonJS/Babylon.js/wiki/How-to-use-lens-flares) ([deltakosh](http://www.github.com/deltakosh))
 - Support for [multi-views](https://github.com/BabylonJS/Babylon.js/wiki/How-to-use-multi-views) ([deltakosh](http://www.github.com/deltakosh))
 - **Updates**
 - New ```light.excludedMeshes``` property to exclude specific meshes from light computation ([deltakosh](http://www.github.com/deltakosh))
 - New ```texture.anisotropicFilteringLevel``` property to define the anisotropic level of a texture ([deltakosh](http://www.github.com/deltakosh))
 - New ```mesh.infiniteDistance``` property to make a mesh static from the point of view of the camera ([deltakosh](http://www.github.com/deltakosh))
 - New ```scene.customRenderTargets``` property to add our own renderTargetTexture ([deltakosh](http://www.github.com/deltakosh))
 - Transparent meshes are sorted back to front ([deltakosh](http://www.github.com/deltakosh))
 - **Bugfixes**
 - Fixing a bug when cloning mirrorTexture ([deltakosh](http://www.github.com/deltakosh))
- 1.6.0:
 - **Major updates**
 - Support for [postprocesses](https://github.com/BabylonJS/Babylon.js/wiki/How-to-use-postprocesses) ([deltakosh](http://www.github.com/deltakosh))
 - New builtin postprocesses: Pass, Refraction, Blur, Black and White, Convolution ([deltakosh](http://www.github.com/deltakosh))
 - New builtin postprocess: FXAA ([simonferquel](http://www.github.com/simonferquel))
 - Online [assets converter](http://www.babylonjs.com/converter.html)  ([pierlag](https://github.com/pierlag))
 - **Updates**
 - New features demos: [POSTPROCESS - REFRACTION](http://www.babylonjs.com/index.html?PPPREF) and [POSTPROCESS - BLOOM](http://www.babylonjs.com/index.html?PPBLOOM)
 - Removing the unused depth buffer for postprocesses chains ([simonferquel](http://www.github.com/simonferquel))
 - **Bugfixes**
 - Fixing a memory leak when releasing textures ([simonferquel](http://www.github.com/simonferquel))
- 1.5.3:
 - **Updates**
 - New ```lockedTarget``` for freeCamera in order to allow cameras to track moving targets ([deltakosh](http://www.github.com/deltakosh))
 - Cameras now supports animations (see http://www.babylonjs.com/index.html?TRAIN) ([deltakosh](http://www.github.com/deltakosh)) 
 - New ```angularSensibility``` property for cameras ([deltakosh](http://www.github.com/deltakosh)) 
 - New ```upVector``` property for cameras. Cameras are now not limited to a (0, 1, 0) up vector ([deltakosh](http://www.github.com/deltakosh)) 
 - New ```parent``` property for cameras and lights: Lights, cameras and meshes can be related. For instance a camera can now be attached to a mesh as child and vice versa ([deltakosh](http://www.github.com/deltakosh))
 - **Bugfixes**
 - Fixing a bug when exporting materials from Blender ([deltakosh](http://www.github.com/deltakosh)) 
 - Fixing an issue with IE11 for RT ([deltakosh](http://www.github.com/deltakosh))
 - Fixing an issue with looping animations ([deltakosh](http://www.github.com/deltakosh))
- 1.5.2:
 - **Updates**
 - New ```renderingGroupId``` for SpriteManager ([deltakosh](http://www.github.com/deltakosh))
 - ```BoundingBox``` and ```BoundingSphere``` are prepared with an identity matrix during construction ([deltakosh](http://www.github.com/deltakosh)) 
 - **Bugfixes**
 - Fixing a bug preventing wireframe to be displayed ([deltakosh](http://www.github.com/deltakosh)) 
 - Fixing an issue with last IE update ([deltakosh](http://www.github.com/deltakosh))
- 1.5.1:
 - **Updates**
 - Massive update of typescript files ([jroblak](http://www.github.com/jroblak))
 - **Bugfixes**
 - Fixing an issue with ```SceneLoader.ImportMesh``` ([nicolas-obre](http://www.github.com/nicolas-obre))
 - Fixing an issue with sprites rendering when no mesh is present ([deltakosh](http://www.github.com/deltakosh))
- 1.5.0:
 - **Major updates**
 - New ```DeviceOrientationCamera``` that supports W3C DeviceOrientations events ([deltakosh](http://www.github.com/deltakosh))
 - Incremental loading support for meshes and textures ([deltakosh](http://www.github.com/deltakosh))
 - New API online page to convert .babylon files to .incremental.babylon files ([pierlag](https://github.com/pierlag))
 - New ```mesh.renderingGroupId``` and ```particleSystem.renderingGroupId``` properties to support rendering layers ([deltakosh](http://www.github.com/deltakosh))
 - **Updates**
 - New ```predicate``` parameter for ```scene.pick``` function in order to be able to select pickable meshes ([deltakosh](http://www.github.com/deltakosh)) 
 - New ```mesh.refreshBoundingInfo()``` method ([deltakosh](http://www.github.com/deltakosh)) 
 - New ```onAnimationEnd``` parameter for animations ([deltakosh](http://www.github.com/deltakosh)) 
- 1.4.3:
 - **Updates**
 - New ```mesh.setLocalTranslation``` and ```mesh.getLocalTranslation``` functions ([deltakosh](http://www.github.com/deltakosh))
 - New ```matrix.setTranslation``` function ([deltakosh](http://www.github.com/deltakosh))
 - ```mesh.rotation``` and ```mesh.rotationQuaternion``` are now two separated functions ([deltakosh](http://www.github.com/deltakosh)) 
- 1.4.2:
 - **Bugfixes**
 - Fixing an issue with scene.executeWhenReady ([deltakosh](http://www.github.com/deltakosh))
- 1.4.1:
 - **Bugfixes**
 - Support for Safari ([deltakosh](http://www.github.com/deltakosh))
 - Adding local transformations to Blender exporter ([deltakosh](http://www.github.com/deltakosh))
 - IndexedDB code refactoring to support simultaneous calls ([davrous](https://github.com/davrous))
 - Hardware scaling fix ([Gwena�l Hagenmuller](https://github.com/gwenael-hagenmuller))
 - Fixing a bug with sprites dynamic buffers ([deltakosh](http://www.github.com/deltakosh))
- 1.4.0:
 - **Major features** 
 - Bones support ([deltakosh](http://www.github.com/deltakosh)). Bones and animated bones are now supported. They can cast shadows. Bones can be exported from Blender or from FBX
 - Offline support ([davrous](https://github.com/davrous). You can specify to offline assets (scene and textures) to a local IndexedDB. Assets are then loaded once until you change the version on a server-side manifest
 - N-Level octrees ([deltakosh](http://www.github.com/deltakosh)):
 - **Updates**
 - Adding ```dispose()``` function and a ```disposeWhenFinishedAnimating``` property to sprites ([Cyle](http://github.com/CYle/))
 - Adding a ```applyTransform()``` function to meshes in order to bake a specific transformation into vertices ([deltakosh](http://www.github.com/deltakosh))
 - Adding ```setPivotMatrix()``` and ```getPivotMatrix()``` to meshes to define pivot matrix ([deltakosh](http://www.github.com/deltakosh))
 - ```Mesh.CreateCylinder``` now takes two diameters as parameters to be able to create cone ([deltakosh](http://www.github.com/deltakosh)) 
 - New ```material.Clone``` function ([deltakosh](http://www.github.com/deltakosh)) 
 - **Bugfixes**
 - ```scene.IsReady()``` is more robust now and can be used to detect when the scene is EFFECTIVELY ready :) ([deltakosh](http://www.github.com/deltakosh))
 - Fixing animations timing. Animations should be in sync now ([deltakosh](http://www.github.com/deltakosh))
 - Fixing a bug with orthographic camera ([deltakosh](http://www.github.com/deltakosh))
 - Fixing a bug with ```attachControl()``` function ([deltakosh](http://www.github.com/deltakosh))
 - Fixing a bug with ```scene.pick()``` function ([deltakosh](http://www.github.com/deltakosh))
- 1.3.2:
 - Fixing a bug with camera.detachControl
- 1.3.0:
 - Selection octrees
 - Breaking changes: Meshes now use multi vertex buffers (one for each attribute) instead of a big one. This is for more flexibility. The .babylon file format has changed accordingly (no more .vertices property on meshes but .positions, .normals, .colors, .uvs, .uvs2)
- 1.2.1:
 - Support for PointerLock ()
 - StandardMaterial now supports per-vertex color
 - Blender exporter supports per-vertex color
- 1.2.0:
 - Major rework of the API to remove GC pressure.
 - FreeCamera: Support for QWERTY keyboards
 - New 3D charting demo
- 1.1.0:
 - Shadow Maps and Variance Shadow Maps
 - Shadows Maps and animations are now exported from Blender
 - Hand.js is no longer required for ArcRotateCamera
 - ArcRotateCamera support pinch/zoom gesture on IE
- 1.0.10:
 - Using typed arrays for Matrix
 - Improving IE11 support
 - Support for new mesh primitives : Torus and cylinder
- 1.0.9:
 - Orthographic camera
- 1.0.8:
 - Adding keyboard support to ArcRotateCamera
 - Starting to use git tag
- 1.0.7:
 - New demo: Worldmonger
 - Improved IE shaders
- 1.0.6:
 - Dynamic meshes
 - Skybox
 - Support for high-DPI displays
 - Height maps
- 1.0.5:
 - Adding color tint for sprites and layers
- 1.0.4:
 - Various optimizations
 - Fog
 - TypeScript support
- 1.0.3:
 - Video textures
 - Normal map (bump) 
- 1.0.2:
 - Spot lights
 - Hemispheric lights
