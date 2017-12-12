# Processing Each Item in a List

**In this lab, **you will create tools for drawing complex designs from lists of points. To do this, you will use problem decomposition—breaking down the problem into smaller pieces. 

**On this page, **you will create a script that lets you connect the dots \(given by a list of points\) to draw the letter A.

#### Thinking Out Loud

Alphie and Betsy are building a program that will take a list of points \(each of which is a list of _x _and _y _coordinates\) as input and connect the dots. They figure they can use it to draw pictures or graphs of data:

To make a set of starting data, they sketched the letter A on graph paper. They chose a _scale _that they figured would make their picture a good size on the stage.  


![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/AonGraphPaper2.PNG "Letter A drawn of graph paper with corner coordinates")![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/AonGraphPaper3.PNG "Corner coordinates \(-50, 20\) \(-10,120\), ... \(-30,20\)")

Then they listed the coordinates of each vertex, starting at the arrow and going clockwise around the figure. The first point is at \(-50, 20\), the second is \(-10, 120\), and so on. Then they built that list in Snap_! _like this:![](http://bjc.edc.org/bjc-r/img/3-lists/coordinate-list-for-A.png "coordinate-list-for-A")

Now they need a script that will use that list to make the drawing, like this: ![](http://bjc.edc.org/bjc-r/img/3-lists/drawA.gif)

**Betsy:** This list of coordinates outlines an A, so let's name it A.

Betsy clicks`Make a variable`, names it`A`, and builds![](http://bjc.edc.org/bjc-r/img/3-lists/A.png "set A to {{-50,20}, {-10,120}, {10,120}, {50,20}, {30,20}, {20,50}, {-20,50}, {-30,20}}").

Then she clicks that `set `block to run it.

**Alphie: **So, for each of those eight points, we want the sprite to move to it. Hmmm... ![](http://bjc.edc.org/bjc-r/img/2-complexity/go-to-x%28%29-y%28%29.png "go to x:\(\) y:\(\)") won't work, because it needs two separate inputs. We need a block that takes _one _input, a point like ![](http://bjc.edc.org/bjc-r/img/2-complexity/list%28-50%29%2820%29.png "list\(-50\)\(20\)").

\*\*Betsy:\*\*  So we'll make a _new _block. Let's call it `go to point`. It'll work like this ![](http://bjc.edc.org/bjc-r/img/2-complexity/go-to-point%28list%28-50%29%2820%29%29.png "go to point \(list \(-50\) \(20\)\)"). We'll use ![](http://bjc.edc.org/bjc-r/img/2-complexity/go-to-x%28%29-y%28%29.png "go to x:\(\) y:\(\)") or ![](http://bjc.edc.org/bjc-r/img/2-complexity/glide%28.5%29secs-to-x%28%29-y%28%29.png "glide \(.5\) secs to x:\(\) y:\(\)") _inside _it, but we'll have to process the input, ![](http://bjc.edc.org/bjc-r/img/2-complexity/list%28-50%29%2820%29.png "list\(-50\)\(20\)"), to supply `x: `and `y: `separately. Hmmm...

