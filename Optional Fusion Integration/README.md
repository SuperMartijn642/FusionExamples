This example resource pack shows how to use different assets when Fusion is and is not installed.

In the `pack.mcmeta` file the `overrides_folder` property is set to the `fusion-overwrites/` folder. This means any resources in `fusion-overwrites/` will overwrite regular resources when Fusion is installed.
To demonstrate this, the stone texture is replaced with a red texture at `assets/minecraft/textures/stone.png` and with a blue texture at `fusion-overwrites/assets/minecraft/textures/stone.png`.
Now when Fusion is not installed, Minecraft will use the red texture and when Fusion is installed, Minecraft will use the blue texture.

More information is available in the directories of the respective files.
