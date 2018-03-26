# Op Art

In this project, you will write code to create tools to explore an art form called Op Art.

![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/OpArt_phase1.png "Op Art Phase 1")

#### ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/OpArt_phase2.png "Op Art Phase 2")For You To Do

1. Watch this animation to get a feel for how you will use your program to generate Op Art. ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/OpArtAnimation.gif)

2. Play with the program [linked here](https://bjc.edc.org/bjc-r/cur/programming/3-lists/optional-projects/2b-op-art-interactive.html) to get a feel for the type of tools you will be developing. Initially the click-drag-release of the mouse is used to draw rectangles. When you press the space bar, then the drawing phase ends and the mouse click becomes a paint bucket that fills bounded regions with paint. Below you can see examples of phase 1 \(drawing rectangles\) and phase 2 \(filling regions with color\) of the program. ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/OpArt2Phase1.png "Op Art 1 Phase 1")![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/OpArt2Phase2.png "Op Art 1 Phase 2")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/OpArt3Phase1.png "Op Art 2 Phase 1")![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/OpArt3Phase2.png "Op Art 2 Phase 2")The coding in this project is subtle and is all about correct sequencing that match the set of events that take place in the creation of the Op Art. You will first build all the helper  blocks that will help make your coding easier.

3. In phase 1, the drawing phase of the project, you will be drawing many rectangles from corner to diagonally opposite corner defined by the mouse click- drag-release. ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/corner12.png "Opposite corners of a recatngle")  
   So first, create a reporter block that will define a `corner `by storing the x and y coordinates of the corner in a list. ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/cornerxy.png "corner x:\(x\) y:\(y\) {report \(list \(x\)\(y\)\) }")

4. Create also the helper reporter blocks that allow you to retrieve the stored x and y values for a given corner. ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/xofcorner.png "x of corner:\(corner\){ report \(item\(1\) of \(corner\)\) }")![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/yofcorner.png "y of corner:\(corner\){ report \(item\(2\) of \(corner\)\) }")

5. Now create a reporter block that will define a rectangle by storing its two diagonally opposite corners in a list. ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/rectanglecorner12.png "rectangle, corner1:\(corner1\) corner2:\(corner2\){report\(list\(corner1\)\(corner2\)}")

6. Now create a block that will draw a rectangle given its two defining corners. The following blocks may help. ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/drawrectanglecorner12Hint.png "drawRectangle corner1:\(corner1\) corner2:\(corner2\); go to x:\(\) y:\(\); pen down; pen up; x of corner:\(\); y of corner:\(\); corner1, corner2")

7. Now create some variables that will help you store and keep track of important information. ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/variables.png "variables: drawingDone, rectangleList, corner1, corner2")

   1. drawingDone: is a Boolean variable that takes values `true`/ `false `and is used to keep track of which stage of the program \(drawing or paintbucket\) is on. It is initially `false `but when the space bar is pressed—which concludes the drawing phase—it is set to `true`.

   2. rectangleList: is a list that will store all the rectangles created so they can be redrawn after each screen refresh.

   3. corner1: variable to store the mouse x and mouse y values when mouse first clicked

   4. corner2: variable to store and update mouse x and mouse y values as the mouse is dragged until released.

8. Now you have all the helper tools you need to create the Op Art program. It is recommended that you first write down the algorithm detailing the sequence of events in the program and what should happen at each case before you build the actual code.

9. Use your Op Art tool to generate exciting works of art and take screenshots of your creations. Share with your class and post them on your class website if you have one.

![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/OpArt4.png "Op Art example 1")

![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/OpArt5.png "Op Art example 2")

#### Take It Further

1. Create a version of your Op Art program that uses polygons. ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/PolyOpArt1.png "Polygonal Op Art example 1")  
   ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/PolyOpArt2.png "Polygonal Op Art example 2")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/PolyOpArt3.png "Polygonal Op Art example 3")

2. Create a version of your Op Art program that uses circle. ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/CircleOpArt2.png "Circle Op Art example 1")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/CircleOpArt.png "Circle Op Art example 2")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/CircleOpArt3.png "Circle Op Art example 3")

3. Study the works of legendary Op Artists such as Victor Vasarely and Bridget Riley to get a feel for what is possible in this art form. ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/Vasarely1.png "Vasarely 1")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/Vasarely2.png "Vasarely 2")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/Riley1.jpeg "Riley 1")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/Riley2.png "Riley 2") ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/Riley3.jpg "Riley 3")

4. It is possible to fully automate the painting phase by using the following algorithm: for every pixel on the screen find out inside how many rectangles it is enclosed. For each pixel, the number of the enclosing rectangles will be either odd or even. Color each pixel black if the number is odd and white if even \(or vice versa.\) To understand why this algorithm works, use paper and pencil to apply it to simple cases with few overlapping rectangles. Write code to automate your Op Art generation. ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/autoOpArt1.png "Overlapping rectangles")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/autoOpArt2.png "Overlapping counted")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/OpArt_img/autoOpArt3.png "Overlapping regions colored")



