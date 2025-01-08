This example resource pack gives the lapis lazuli block a complex connecting texture using the `full` connecting texture layout.

There are two parts to accomplishing this:
1. The model for the glass block, `assets/minecraft/models/block/lapis_block.json`, should be overwritten to use a connecting model with connection predicates to connect to neighboring lapis lazuli blocks.
2. The lapis lazuli texture, `assets/minecraft/textures/block/lapis_block.png`, should be replaced with a connecting texture and appropriate metadata.

More information is available in the directories of the respective files.

The result will look like this:

![lapis pattern.png](../images/lapis%20pattern.png)
