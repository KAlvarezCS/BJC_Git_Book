# Processing Each Item in a List

**In this lab, **you will create tools for drawing complex designs from lists of points. To do this, you will use problem decomposition—breaking down the problem into smaller pieces.

**On this page, **you will create a script that lets you connect the dots \(given by a list of points\) to draw the letter A.

#### Thinking Out Loud

Alphie and Betsy are building a program that will take a list of points \(each of which is a list of x and y coordinates\) as input and connect the dots. They figure they can use it to draw pictures or graphs of data:

To make a set of starting data, they sketched the letter A on graph paper. They chose a scale that they figured would make their picture a good size on the stage.

![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/AonGraphPaper2.PNG "Letter A drawn of graph paper with corner coordinates")![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/AonGraphPaper3.PNG "Corner coordinates \(-50, 20\) \(-10,120\), ... \(-30,20\)")

Then they listed the coordinates of each vertex, starting at the arrow and going clockwise around the figure. The first point is at \(-50, 20\), the second is \(-10, 120\), and so on. Then they built that list in Snap\_! \_like this:![](http://bjc.edc.org/bjc-r/img/3-lists/coordinate-list-for-A.png "coordinate-list-for-A")

Now they need a script that will use that list to make the drawing, like this: ![](http://bjc.edc.org/bjc-r/img/3-lists/drawA.gif)

**Betsy:** This list of coordinates outlines an A, so let's name it A.

Betsy clicks `Make a variable`, names it `A`, and builds![](http://bjc.edc.org/bjc-r/img/3-lists/A.png "set A to {{-50,20}, {-10,120}, {10,120}, {50,20}, {30,20}, {20,50}, {-20,50}, {-30,20}}").

Then she clicks that `set`block to run it.

**Alphie: **So, for each of those eight points, we want the sprite to move to it. Hmmm... ![](http://bjc.edc.org/bjc-r/img/2-complexity/go-to-x%28%29-y%28%29.png "go to x:\(\) y:\(\)") won't work, because it needs two separate inputs. We need a block that takes one input, a point like ![](http://bjc.edc.org/bjc-r/img/2-complexity/list%28-50%29%2820%29.png "list\(-50\)\(20\)").

**Betsy: ** So we'll make a new block. Let's call it `go to point`. It'll work like this ![](http://bjc.edc.org/bjc-r/img/2-complexity/go-to-point%28list%28-50%29%2820%29%29.png "go to point \(list \(-50\) \(20\)\)"). We'll use ![](http://bjc.edc.org/bjc-r/img/2-complexity/go-to-x%28%29-y%28%29.png "go to x:\(\) y:\(\)") or ![](http://bjc.edc.org/bjc-r/img/2-complexity/glide%28.5%29secs-to-x%28%29-y%28%29.png "glide \(.5\) secs to x:\(\) y:\(\)") inside it, but we'll have to process the input, ![](http://bjc.edc.org/bjc-r/img/2-complexity/list%28-50%29%2820%29.png "list\(-50\)\(20\)"), to supply `x:`and `y:`separately. Hmmm...

**Gamal:** Oh! I know how! I bet we can use ![](http://bjc.edc.org/bjc-r/img/2-complexity/item%28%29of%28list%29.png "item\(\)of\(list\)"). Give it a number as its first input. I bet that the ![](http://bjc.edc.org/bjc-r/img/3-lists/list_input_slot.png "rectangle with two smaller orange rectangles inside") just says that it expects a list as its second input.

**Alphie:** I wonder if we can make _our _`go to point`block show that it expects a list as input....

Yes, _you can make your blocks show what type of data they expect as inputs: a number, a list, or some other type. Some languages require the data type to be indicated. In Snap_! it's an option. It's not necessary but, like assigning a color to a block, it can be a helpful reminder of what the block does and what type of input it expects. You've already seen input slots of several shapes, indicating different expected data types.

#### For You To Do

1. [Click here to load. Save to Your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/2-complexity/U2L2-DrawShape.xml) It contains the list of points, but you need to build their![](http://bjc.edc.org/bjc-r/img/2-complexity/go-to-point-point.png "go to point \(point\) block with list type input named point")**Specifying an Input Type **This animation shows you how to specify the list input type. Other input types are specified the same way. ![](http://bjc.edc.org/bjc-r/img/3-lists/list_input_slot.png "rectangle with two smaller orange rectangles inside") block. ![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/gotopointAnimation.gif)After creating the title and naming the input,

   * Click on the arrow to the right of the input name:

     ![](http://bjc.edc.org/bjc-r/img/2-complexity/create-input-name-right_arrow.png "create input name right arrow")

   * Choose the data type you want for that input.

   * Click OK.

2. Finish building your go to point and test your block with a few points as input to make sure it does what you want it to.

#### Thinking Out Loud

**Alphie:** Great! Now we can use our `go to point`block for each of the points in our list.

**Betsy:** I bet we can use![](http://bjc.edc.org/bjc-r/img/2-complexity/for-each-%28item%29-of%28%29.png "for-each-\(item\)-of\(\)").

Alphie and Betsy design this new script to automate the process of going to each point. ![](http://bjc.edc.org/bjc-r/img/2-complexity/new-for-each-point-script.png "new-for-each-point-script") Then they test it out.

**Alphie:** Yup! `for each`does exactly what we want. But we have a couple of bugs to fix.

#### For You To Do

Build and test the script they used. 

1. Fix the two bugs Alphie noticed.
2. Save this as "U2L2-DrawShape"
3. **Think and write:**
   * For what purposes might you not want to connect the first and last points?
   * For what purposes might you want to have the pen down only when the sprite marks each point, but never when the sprite moves from one point to another?
   * For what purposes might you prefer `go to`over `glide`?

#### Take It Further

Create three new points and a script that draws the complete letter A. You'll have to design a way to indicate in a list of points that they aren't all connected.

