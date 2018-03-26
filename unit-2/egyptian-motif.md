## Egyptian Motif

![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/HexalDesign1.png "Hexagonal Design 1")

![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/HexaDesign2.png "Hexagonal Design 2")

Much Islamic art applies principles of geometry and repeats simple patterns to form complex forms. For example, the Egyptian Motif above has six overlapping rectangles.

**In this project,**you will learn how to extend your `pinwheel `code from Unit 1 to create such intricate patterns.

#### For You To Do

1. In this project, you will repeatedly use rectangles, so first recall how to create a `rectangle `block.

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/rectangleCode.png "Code for drawing a rectangle")

   1. Note the use of `pen down `and `pen up `blocks inside the rectangle definition. We don't normally do this but here this is done to simplify the more complex code coming ahead. This will ensure that once a rectangle is drawn, the pen is up and you don’t need to worry about unintended scribbles as your drawing sprite continues moving to execute the rest of the code.

2. Also recall the `pinwheel `code you have written in Unit 1. ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/pinwheelCode.png "Code for drawing pinwheel")

3. In this project, you will replace the _**pinwheel branches **with _**rectangles **as shown below. Note use of color is optional and is used here for clarity.

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/multiColorPinwheel.png "Multicolored pinwheel")

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/multiColorPinwheelwithRectangles.png "Multicolored pinwheel with rectangles")

   1. Now create a `pinwheel with rectangles `block. It will have two more inputs width and length for the width and length of the rectangles.  
      ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/pinwheelWithRectanglesCodeHeader.png "Pinwheel with rectangles hat block")Its code will be identical to the `pinwheel `code except that it has the `rectangle `block inserted in between the two `move `blocks that created the pinwheel branches.

      ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/rectangleInBetween.png "Rectangle block in between two move blocks")

4. Now, use the “Variables” menu to make variables that will allow you to vary all aspects of the designs you create and do not forget to initialize these variables right after the `when green flag clicked `block ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/makeVariables.png "Make variables")

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/initializeVariables.png "Initialize variables")

5. You can turn these variables to alterable sliders by right-clicking on the variable icon that is shown on stage and choosing the “slider” option. And then you can set the minimum and maximum values of a slider as shown. ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/turnToSlider.png "Turn variables to sliders")

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/sliderMax.png "Slider maximum")

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/setSliderMax.png "Setting slider maximum")

   1. The following should be reasonable values for the minimum and maximum of each variable:

      1. | Variable |
         | :--- |

|  | Minimum | Maximum |
| :--- | :--- | :--- |
| number of branches | 3 | 36 |
| size | 0 | 100 |
| backup | 0 | 100 |
| width | 0 | 150 |
| length | 0 | 150 |

1. Click on the animation below to see an example of how you can use the slider functionality in Snap\_! \_to generate and explore a vast number of variations of your designs. ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/sliderAnimationDemo.gif)

2. Your code needs to make sure that the computer is always on the watch in case any of the variables are changed by the user via the sliders. You can do so with a `forever `block.  
   ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/foreverLoop2.png "Forever loop")

   The `warp `block makes sure that the `pinwheel with rectangles `is drawn all at once rather than step by step.

3. Once the code is written check to make sure everything works as intended. You may need to position your drawing spite appropriately to make best use of the stage you have. Now move each of your sliders to generate and explore a vast variety of designs inspired by Islamic art.

   1. Use these buttons to maximize your stage to give enough room for your sliders.

      ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/stagemaximize.png "Stage maximizing buttons")

#### If There Is Time...

1. Add color to your rectangles by inserting ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/setColor.png "Set color block") into the start of the `warp `block in the forever loop and inserting ![](http://bjc.edc.org/bjc-r/img/2-complexity/EgyptianMotif_img/changeColor.png "Change color block") into the `pinwheel with rectangles `code.

#### For You To Do

1. Take screenshots of your creations and share with the class. Put them on a class webpage if you have one. Below are some examples o the types of variations you can generate.



