Here the model for the grass block is overwritten with a connecting model. The model elements and textures are the same as the vanilla grass block model.

The `block/grass_block_side_overlay` texture should behave as follows:
- It covers the entire side if the block below it or the block in front of the block below it is a grass
- It connects to the bottom right if the block diagonally below and to the right or the block in front of that block is a grass block
- It connects to the bottom left if the block diagonally below and to the left or the block in front of that block is a grass block
- In all other situations, it has just a strip of grass at the top like in vanilla

To accomplish this, this example uses the `full` connecting texture layout with some specifically crafted connection predicates.  
The `full` layout doesn't really allow for connecting to just a corner, but not the neighboring sides. To work around this, we will invert the connection predicates and actually draw the texture as if it only connects to the directions it usually should not connect to.  
Then, since we only care for the bottom directions, we will use a `is_direction` predicate which checks for the bottom, bottom left, or bottom right directions. For these directions, we then want to check whether either the block in that direction or the block in front of that block is a grass block.

This results in the following predicates:
- `not`:
  - `and`:
    - `is_direction` bottom, bottom left, or bottom right
    - `or`:
      - `is_same_block`, i.e. the block is also a grass block
      - `match_block_in_front` for grass block

In the texture we then only need to draw the cases where:
- It connects to every direction, but the bottom
- It connects to every direction, but not bottom left or not bottom right
- It connects to all directions