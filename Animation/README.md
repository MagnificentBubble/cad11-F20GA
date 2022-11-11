# Animation

## Unreal Import Pipeline
The models made in the previous part were exported from blender as FBX files and imported into Unreal Engine 5's content drawer. While the meshes made it fine, the materials did not. As such they required baking and exporting from blender. To this end, a blender file was created that mapped each material to a plane. The Diffuse, Normal, Roughness, and Displacement values were baked to an image file in the cycles rendering mode and saved externally. This file can be found in ./Appendicies/Animation/Baked Goods along with the baked textures. These textures were then attached to the material in Unreal.
Some materials, such as metals, had to be altered for the bake to work. As such, these properties required restorarion using the options native to Unreal. These were not difficult to find nor accomplish.

## Animation in Unreal
The animations for the objects were created by making blueprints in the unreal engine. The relevant static mesh was then added as well as a timeline. Tracks were added to the timeline that output a value that varies with time. These values were then fed to a linear interpolator widget that fed into various transforms that acted upon the mesh. Multiple tracks and timelines were used simultaneously where appropriate.
The Orrery was created as a nested stack of three blueprints. One to spin the earth, one to turn he arm with earth attatched, and one for the sun with the former attached.

## Cinematic Animation
The cinematic was created using three cameras in a Level Sequence. The first was a stationary camera that had its aperture property changed to bring out of focus objects into focus. The second was a camera attatched to a crane. The crane turned at the same rate as the orrery to track the earth, while the camera rotated at the same rate to keep the earth in view. The last camera was used for a retreating shot where it moved bacwards along its Z axis and had its focal length property changed to bring the entire scene into view.

## Video Export
The video file was exported from unreal using the Movie Pipeline CLI Encoder plugin in the Movie Render Queue and leveraging a the free open source program, ffmpeg to take the rendered out image sequence and string them into an MP4. 
