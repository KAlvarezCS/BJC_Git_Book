# Abstract Data Types

**On this page, **you will create an abstract data type `point`to make your U2L2-DrawShape code easier to read, debug, and use:![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/drawShapewithPointList.png "list of points for the letter A")Just as the name suggests, a **data type **is what type of data something is \(number, text string, list, etc.\). Each programming language provides some **primitive **\(built in\) **data types**. Snap\_! \_provides numbers, text \(words and sentences\), lists, Booleans, and some you haven't yet used as data: ![](http://bjc.edc.org/bjc-r/img/3-lists/isa-menu.png)

An**abstract data type**\(or**ADT**\) is a kind of data that's meaningful to your program but not built into the language. You develop it as you program.

For example in this lab, you'll create a\_point\_data type with:

* ![](http://bjc.edc.org/bjc-r/img/3-lists/point%28%29%28%29.png "point constuctor block") to \_construct \_the ADT
* ![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/xcoordinateof.png "x coordinate of") and ![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/ycoordinateof.png "y coordinate of") to \_select \_either coordinate of a point

The word "abstract" is often used casually to mean something \_harder \_to understand or more complex, but in computer science, its meaning is almost the opposite. ADTs are things that you, the programmer, create to make your program \_easier \_for you and others to read, debug, and improve.

#### Thinking Out Loud

Gamal joins Betsy and Alphie's [ongoing discussion](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/2-data-structures-art/1-the-for-each-block.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment) about using a list of coordinates to draw a letter.

**Gamal:** I was looking at our ![](http://bjc.edc.org/bjc-r/img/2-complexity/go-to-point%28%29.png "go-to-point\(\)") block and thought of a way to make it much easier to read.

Betsy: Yeah, expressions like![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/item2ofpoint.png "item\(2\)of-point")are hard to read. Even after I wrote it to find the \_y \_coordinate, I had to think twice to understand it. Gamal is suggesting **data abstraction**: creating a new ADT to hide the details. When using the `point`ADT, you won't have to think about how points are represented as lists.

**Gamal:** That's what I mean. Let's make it clearer. We can define a ![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/ycoordinateofpoint.png "y coordinate block") block to use instead of `item 2 of.`

`Betsy:` But that block would do just the same thing as `item 2 of`, so what's the use? It won't make the program shorter.

**Gamal:** Yes, but it'll make the program easier to read and _easier to think about_. We can use `x coordinate`and `y coordinate`instead of `item of`as inputs to the `go to`block.

They build two blocks: ![](http://bjc.edc.org/bjc-r/img/2-complexity/xcor.png "x coordinate of \(point\); report item 1 of \(point\)") and ![](http://bjc.edc.org/bjc-r/img/2-complexity/ycor.png "y coordinate of \(point\); report item 2 of \(point\)")

**Betsy:** Hmmm... And if we make a ![](http://bjc.edc.org/bjc-r/img/3-lists/point%28%29%28%29.png "point \(\) \(\)") block, then we can write ![](http://bjc.edc.org/bjc-r/img/3-lists/point-list-for-A.png "point-list-for-A") instead of ![](http://bjc.edc.org/bjc-r/img/3-lists/coordinate-list-for-A.png "coordinate-list-for-A"). That would make it clearer what this list really is.

Betsy builds this block. She marks the `x`and `y` input variables as Numbers, the same way they marked the ![](http://bjc.edc.org/bjc-r/img/3-lists/point.png "point\(X\#\)\(Y\#\){report\(list\(X\)\(Y\)}")

Don't type the`#`symbol in the `point`block's input names. Just like the `⋮`symbol for inputs that you declared to be lists, the`#`is not part of the input's name, but is a **type hint **that you create when you select the Number input type: ![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/input-type-number.png "selecting the Number input type") Type hints change the appearance of the input slot, to indicate what kind of input is expected.

The ![](http://bjc.edc.org/bjc-r/img/3-lists/point%28%29%28%29.png "point \(\) \(\)") block is called the **constructor **of this new abstract data type. The ![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/xcoordinateof.png "x-coordinate-of-\(\)") and ![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/ycoordinateof.png "y-coordinate-of-\(\)") blocks are called the **selectors **for the `point`ADT because they each \_select \_one component of a point.

#### For You To Do

1. If your U2L2-DrawShape project is not already open, open it now.

2. ![](http://bjc.edc.org/bjc-r/img/icons/save-mini.png "Save Your Work")Improve your `go to point`block \([from "U2L2-DrawShape"](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/2-data-structures-art/1-the-for-each-block.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment)\) by using selectors inside the `go to point`block as Betsy and Gamal described.

3. Convert that script into a general ![](http://bjc.edc.org/bjc-r/img/2-complexity/drawShape.png "drawShape") block that takes as input a list of points and draws that shape.

#### If There Is Time...

1. Make a new list of points to draw a different letter or shape. This time use your point constructor in the list of points. Check to see that you draw shape \(\) block works with the new list. 
2. If you made other letters, write a `draw message () `block that takes a _list of letters _as input and uses `draw shape ()`several times to draw a message. ![](http://bjc.edc.org/bjc-r/img/3-lists/hi_new.gif)

Notice the use of abstraction. Representing the message "HI" as ![](http://bjc.edc.org/bjc-r/img/3-lists/list-h-i.png "list \(H\)\(I\)") hides all the complexity of the lists of coordinates used to draw the shapes.

![](/assets/save.png)

#### Take It Further

Change your project so that draw message draws the letters next to each other instead of replacing one with another.

![](http://bjc.edc.org/bjc-r/img/2-complexity/HI.png)



