# Animation

## Unreal Import Pipeline
The models made in the previous part were exported from blender as FBX files and imported into Unreal Engine 5's content drawer. While the meshes made it fine, the materials did not. As such they required baking and exporting from blender. To this end, a blender file was created that mapped each material to a plane. The Diffuse, Normal, Roughness, and Displacement values were baked to an image file in the cycles rendering mode and saved externally. This file can be found in ./Appendicies/Animation/Baked Goods along with the baked textures. These textures were then attached to the material in Unreal.
Some materials, such as metals, had to be altered for the bake to work. As such, these properties required restorarion using the options native to Unreal. These were not difficult to find nor accomplish.
