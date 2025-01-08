Here, we create an item model modifier targeting the stick item which will overwrite the model whenever the stack size is above a given value.
In an item model modifier, the first model for which all conditions are met is used.  
This example uses two entries for both created models each with a `count` condition to apply the model when the stack size is above the given value.