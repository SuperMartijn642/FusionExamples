This example resource pack makes the glass block texture connect to neighboring glass blocks.

There are two parts to accomplishing this:
1. The model for the glass block, `assets/minecraft/models/block/glass.json`, should be overwritten to use a connecting model with connection predicates to connect to neighboring glass blocks.
2. The glass texture, `assets/minecraft/textures/block/glass.png`, should be replaced with a connecting texture and appropriate metadata.

More information is available in the directories of the respective files.

The result will look like this:

![connected glass.png](../images/connected%20glass.png)
