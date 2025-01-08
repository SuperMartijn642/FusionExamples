To create the animated conveyor belt, we create an image which of a belt and then use the `scrolling` texture type to have a frame go over the image to make it seem like it is moving.
To make the animation look smooth, it is important that the last frame matches the frame that should come before the first.

In the metadata file, we specify the `scrolling` texture type, that the frame should scroll from top left to bottom left (left or right doesn't matter in this case), and that each frame is displayed for 10 ticks.
