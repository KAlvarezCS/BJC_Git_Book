# Brick Wall

I**n this project, **you will use abstraction to draw a brick wall.

![](http://bjc.edc.org/bjc-r/img/abstraction/new-brickwall/wall.png "Sample image of brick wall")

#### **Abstraction**

Any good programming language might have many tools for drawing and moving, but it wouldn't make sense to have special tools for drawing bricks because most programs don't involve bricks. That's the sort of tool you make yourself when you need it.

Creating a special![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/drawBrick.png "drawBrick length:\(\) width:\(\) block")block lets you use procedure names related to the problem you are solving \(like `draw brick`\), rather than the general-purpose procedures \(like `move`\) that the computer uses for all kinds of tasks.

### Drawing One Brick

A picture of a brick is just a rectangle with a brick red color. However, there's no `draw rectangle `block in Snap. One way to draw one is by thinking of a rectangle as a very thick line. Here's the idea:  
![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/simpleBrickCode.png "draw brick, length:\(\) width:\(\) block definition")

The![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/setFlat.png "set flat line ends to &amp;lt;&amp;gt;")block isn't built into Snap_!_. In projects without it, you can set the "Flat line ends" in the![](http://bjc.edc.org/bjc-r/img/sys/settings.png "Settings")menu.

Ordinarily, Snap! draws thick lines with rounded ends:![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/round-ends.png "line with round ends"). That's often the best choice, and you can see why below. But for bricks, we want flat line ends:![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/flat-ends.png "flat line ends").

![](http://bjc.edc.org/bjc-r/img/2-complexity/flat-line-ends-why.jpg "Square with flat line ends versus square with round line ends")

**flat** vs. **rounded** line ends

#### For You To Do

1. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/2-complexity/U2L4-brickwall.xml) It includes the complete draw brick block shown below. Read the code; then try it out.![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/drawBrickCode.png "draw brick, length:\(\) width:\(\) block definition")

### Using Problem Decomposition

You'd like the "top level" block to be something like this:  
![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/draw-brick-wall-7.png "draw-brick-wall-7")  
Getting there involves **problem decomposition**: breaking the problem into smaller pieces.

There are two kinds of rows, so we make blocks that specialize in each:

* **Row A**
  :
  ![](http://bjc.edc.org/bjc-r/img/abstraction/new-brickwall/row-a.png "Row A")
* **Row B**
  :
  ![](http://bjc.edc.org/bjc-r/img/abstraction/new-brickwall/row-b.png "Row B")

#### For You To Do

1. Use `draw brick `to make blocks ![](http://bjc.edc.org/bjc-r/img/abstraction/new-brickwall/rowa-block.png "Row A") and ![](http://bjc.edc.org/bjc-r/img/abstraction/new-brickwall/rowb-block.png "Row B").
2. The two kinds of rows should be exactly the same length. Your first try at drawing Row B is probably a little too long. **Debug it.**

   1. Should Row B have different-size bricks, different-size gaps, or just different-size bricks on the end?

   2. If you're not sure, try all the possibilities and see which looks right int he finished wall.

   3. Or think "What would make the most sense in a real brick wall?"

Once you have rows A and B the same length, you are ready to write the ![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/draw-brick-wall-7.png "draw-brick-wall-7")block.

#### For You To Do

1. [Import](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/1-variables-games/4-importing-exporting.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment) your [`even?`block](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/3-predicates/2-keeping-list-items.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment) and use it to write the ![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/draw-brick-wall-7.png "draw-brick-wall-7") block. Read the Debugging Dependencies section below and **test **your new block to make sure it works properly.

#### **Debugging Dependencies**

![](http://bjc.edc.org/bjc-r/img/2-complexity/even-obsolete.png "even? \(number\) block definition with Obsolete! block")

You created your `even?`block using another custom block,`divisible by?`. You must export both blocks in order for `even?`to work properly when you import it into your Brick Wall project.

If you ever see this red `Obsolete!`block in code you have imported, it means that a required block was not exported. You'll want to go back to the original project and export again being sure to select all of the blocks needed by your custom blocks.

![](/assets/save.png)

#### If There Is Time...

1. Use your brick wall in another project by exporting and importing your brick wall blocks.

#### Take It Further

* Add more inputs to `draw Brick Wall`\(and as needed to `row A`and `row B`\) for:

  * Number of bricks per row

  * length and width of a brick

  * Gap thickness

![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/drawBrickWallwithManyInputs.png "draw a Brick Wall with \(8\) Rows with Bricks per Row: \(7\) of Brick Length: \(40\) Width: \(20\) Gap Thickness: \(5\)")Add these one at a time, not all at once! When you modify the length of a brick, that should also change the length of a row B end brick. When you modify the gap thickness, that should also change the distance between the rows.

