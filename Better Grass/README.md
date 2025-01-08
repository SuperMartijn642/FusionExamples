This example resource pack makes the grass on grass blocks connect to other grass blocks below or diagonally below itself.

There are two parts to accomplishing this:
1. The model for the grass block, `assets/minecraft/models/block/grass_block.json`, should be overwritten to use a connecting model with connection predicates to connect to glass blocks below itself.
2. The side grass texture, `assets/minecraft/textures/block/grass_block_side_overlay.png`, should be replaced with a connecting texture and appropriate metadata.

More information is available in the directories of the respective files.

The result will look like this:

![better grass.png](../images/better%20grass.png)
