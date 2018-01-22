# Fractal Art

**In this project, **you will nest `repeat `blocks inside `repeat `blocks to generate complex pictures.  
![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/RecursiveTriangleSteps.gif "Recursive triangle in steps")

![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/RecursiveSquareSteps.gif "Recursive square in steps")

![](http://bjc.edc.org/bjc-r/img/1-introduction/two-color-sierpinski-code.png "repeat \(3\) \(set pen color to \(red\), move \(100\) steps, repeat \(3\) \(set pen color to \(blue\), move \(100\) steps, turn right \(120\) degrees\), turn right \(120\) degrees\)")

#### For You To Do

1. Start a new project. Save it as "U2L4-FractalArt"
2. Build a script that draws a red triangle, duplicate it twice, and make the two new scripts draw a blue triangle half the size of the red and green one half the size of the blue.

   * To duplicate a script, right-click\(or control-click\) on the first block of the script\(int this case, the repeat block\) and choose "duplicate".

   * Then, change the inputs as the video shows:![](http://bjc.edc.org/bjc-r/img/1-introduction/duplicating-a-script.gif).

  

3. Try each script by itself to be certain what it does. Then clear the stage.

4. Now, insert the entire script for the blue triangle between the move and turn block of the red triangle, like this. ![](http://bjc.edc.org/bjc-r/img/1-introduction/embedding-one-script-in-another.gif)

5. ![](/assets/talk_with_partner.png)Predict what will happen when you run this ![](/assets/pair_programming.png) script.

6. Then, try this script to see what it does.

7. Using the scripts you have, find a way to make this picture. ![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/three-color-sierpinski.png "Red triangle with blue children and green grandchildren")

#### If There is Time...

If you like, embed one more triangle, half the size of the last one, in the same way.



#### Using Abstraction to Nest Triangles

Does all this copying and pasting of code feel awkward to you? You know a better way:_abstraction_. In Unit 1 you used a`pinwheel`block to implement`asterisk`and`polygon`, rather than copying the code. Here, you can use a block to manage the abstraction too, but in this case, we want very similar code \(a smaller triangle\) nested inside, so we will actually_use the same block inside itself_.



#### For You To Do

1. Create a nested triangle block.
   1. Design the block with one input, size. For now, leave out the part about changing colors. ![](http://bjc.edc.org/bjc-r/img/2-complexity/nested-tri-no-color-proto.png "nested triangle, size: \(size\)")
   2. Use your first unnamed triangle script from problem 1 as a model. But add one condition: draw the triangle only if it's big enough: ![](http://bjc.edc.org/bjc-r/img/2-complexity/triangle.png "if\(size&amp;gt;9\){repeat\(3\){move 100 steps; turn clockwise 120 degrees}}")
   3. Click the "Apply" button in the Block Editor so that the block appears in the palette on the left.
   4. **Try out this block** giving at least the inputs 9,18,20 and 100 to make sure it works as you expect.
2. In problem \#4, you dragged a copy of the script between the `move `and `turn `blocks. You can do a similar thing with your _block_.

   1. From the palette, drag a copy of that `nested triangle `block into the editor and insert it _in _the definition of `nested triangle `between the `move `and `turn `blocks. Make its size input half the current value of size. ![](http://bjc.edc.org/bjc-r/img/2-complexity/nested-tri-recur-no-color.png "nested triangle, size: \(size/2\)")

   2. Again try out your block with at least the inputs 9,18,20 and 100 to make sure it works as you expect. You are using

      `nested triangle `in its own definition. When a block refers to itself, the block is said to be _recursive_. Recursion is one of the most powerful techniques in computer science and you will learn more about it in later projects.

3. Use nested triangle as a model to define a recursive nested square block.

![](/assets/save.png)

#### If There Is Time...

1. Try adding a color input and using ![](http://bjc.edc.org/bjc-r/img/2-complexity/set-pen-color-to-number.png "set-pen-color-to-number") instead of ![](http://bjc.edc.org/bjc-r/img/2-complexity/set-pen-color-to-color-selector.png "set-pen-color-to-color-selector") so that you can vary the color as you draw. In the "recursive call"—the block that is embedded _inside _and that has the half-size input—try adding 10 to the color. Before you try this block, use ![](http://bjc.edc.org/bjc-r/img/2-complexity/set-pen-color-to-color-selector.png "set-pen-color-to-color-selector") to pick a colorful color, not nearly white or nearly black. Then you can use any color number as input to your new block.

2. Examine this code without running it:  


   ![](http://bjc.edc.org/bjc-r/img/2-complexity/blue-square-embedded-in-red-square.png "blue-square-embedded-in-red-square")

  






