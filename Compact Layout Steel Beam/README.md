This example resource pack create a steel beam texture using the `compact` connecting texture layout.
To show it, the texture is applied to the iron block.

There are two parts to accomplishing this:
1. The model for the iron block, `assets/minecraft/models/block/iron_block.json`, should be overwritten to use a connecting model with connection predicates to connect to neighboring iron blocks.
2. The iron block texture, `assets/minecraft/textures/block/iron_block.png`, should be replaced with the steel beam texture and appropriate metadata.

More information is available in the directories of the respective files.

The result will look like this:

![steel beam.gif](../images/steel%20beam.gif)
