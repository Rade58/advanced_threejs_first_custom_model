# ThreeJS advanced techniques - Loading Blender model (Workshop)

Loading my first model I built in blender

## Exporting from blender

- Select model first
- File --> Export -->  pick this format:  glTF 2.0 (.glb/.gltf)
- you need to pay attention to `include` part
  - we include only `selected objects`
  - transforms `+Y up` is already selected, and keep it that way (we need this because of difference in case of y being up in threejs and z being up in blender)
  - `Data` --> `Mesh` --> select  `Apply modifiers` since we used modifiers (you would had just cubes in threejs, if not selected)
  - unselect `UVs`, we don't need that, since we are not using any textures
  - we also want `Normals`, because lights wouldn't work among other things, if not selected
- We don't need to export vertex colors, unselect that
- Material needs to be exported also, and no image(unselect image)
- if you want draco compression, you can select it
- uncheck animations since we don't have any
- unselect skinning and shape keys

- Save model in our static folder (don't change extension while giving the name while saving)
