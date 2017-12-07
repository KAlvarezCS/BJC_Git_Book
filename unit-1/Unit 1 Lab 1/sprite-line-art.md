# Sprite Line Art Project

**In this project,**you are going to simulate the famous children's toy _Etch A Sketch_®.

![](http://bjc.edc.org/bjc-r/img/1-introduction/SpriteLineArt_img/SpriteArt.png "Sprite Art")

#### For You To Do

1. Play with the program [linked here](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/optional-projects/1c-sprite-line-art-interactive.html) to get a feel for how the drawing tool works. Use the up, down, right, left arrow keys and the space bar to see what they do. These are some blocks that may be handy in your work ahead. ![](http://bjc.edc.org/bjc-r/img/1-introduction/SpriteLineArt_img/HintsBlocks.png "Hint blocks: when green flag clicked; when space key pressed; when right arrow key pressed; clear; set pen size to \(1\); set pen color to \(red\); pen up; pen down; go to x:\(0\) y: \(0\); point in direction \(0\); point in direction \(90\); move \(10\) steps")To locate the blocks you will need in the menus, you can match the block and menu colors. For example, the green blocks are in the green colored Pen menu. ![](http://bjc.edc.org/bjc-r/img/1-introduction/SpriteLineArt_img/penMenu.png "Pen menu items: clear; pen down; pen up")

2. Here are some things to do at the start of your program `when green flag clicked`:

   * Clear any previous drawings
   * Place the drawing sprite at the center of the screen
   * Point it in the up direction
   * Set the drawing pen to a color and size of your choice
   * Put pen down to get ready for drawing

3. Write code that will clear the drawings `when space key pressed `by the user.

4. Now you are ready to write the code for what will happen when each of the arrow keys are pressed. Here is what should happen `when right arrow key pressed `by the user.

   * Point to the right.
   * Move a certain amount, say 10 steps, in that direction.

5. Now write the code blocks to enable the remaining arrow keys: left, up, and down.

Here is how Snap! assigns angles for directions:

* 0° is up
* 90° is right
* 180° is down
* -90° \(or also 270°\) is left

Positive angles are measured clockwise from the 0°, up direction, and negative angles are measured counterclockwise from the 0°, up direction.

![](http://bjc.edc.org/bjc-r/img/1-introduction/SpriteLineArt_img/Directions.png "Snap! directions")

#### Take It Further

1. Now, the program will continue drawing past the edge of the screen. Change your code to draw only if the drawing sprite is within the screen dimensions: -240 to 240 in the x direction \(horizontal\) and -180 to 180 in the y-direction \(vertical\). You can create blocks such as the one below to restrict sprite movement. ![](http://bjc.edc.org/bjc-r/img/1-introduction/SpriteLineArt_img/xRestriction.png "if \(x position&amp;lt;240\)")

2. Give your user some coloring options. For example, when “1” key is pressed, the pen color is reset to black, when “2” key is pressed, the pen color is set to red etc. Also consider using some keys to put the `pen up `or `pen down`.

3. Give your user the option to draw diagonal lines. For example, write code to move the drawing sprite at 45°, 135°, 225°, 315°, using the “w”, “s”, “a”, “q” keys.

4. Create some exciting art works using your line art drawing tool. Take screenshots of your work and create a class-wide art gallery. Put it on the web for other classes or schools to see.



