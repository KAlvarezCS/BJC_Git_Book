# Building a Graphing App

**On this page**, you will learn how to scale values so that you can graph any data set on the Snap_! _stage. Blocks to do the calculations are already written for you but you can, if you like, examine them to see how they work.

Plotting a single point, given its two coordinates, should feel this basic:

![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/plotpointxy.png "plot point x: \(x\) y: \(y\)")  


Then you could graph a list of data points by inventing a block like![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/Graph%20datapoints.png "Graph datapoints: \(\)")just like your work in Unit 2 Lab 2. Depending on the kind of graph you want, you can connect the dots or not.

That seems like all you should need. But what if the _scale _of your data does not fit on the Snap_! _stage \(between -240 and 240 in the _x _direction and between -180 and 180 in the _y _direction\)? For example, what if you want to plot the popularity of a baby name over time, like this? ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/SnapStageCoordinates.png "Snap Stage Coordinates")

![](https://bjc.edc.org/bjc-r/img/5-algorithms/PercentageOfDerekByYear.png "percentage of births named Derek by year")

  
The years can't be plotted on the horizontal because those values are completely off Snap_!_'s stage. And the percent values 0, 0.1, 0.2, 0.3, etc., are so close to each other that they would all look the same. We wouldn't see the increase in popularity between 1960 and 1980 at all. We need a way to_convert_between Snap_!_**stage coordinates**and the values—we'll call them the**graph coordinates**—for a given set of data points.

  
A good grapher needs to let the user set the **scale **of the screen, to specify where to focus attention—where to zoom in.

#### For You To Do

1. [Click here to load. Save to your Snap! account. ](http://snap.berkeley.edu/snapsource/snap.html#open:https://bjc.edc.org/bjc-r/prog/3-lists/U3L4-GraphingApp.xml)It contains several blocks already built for your convenience.
   1. Click the set graph scale block with the inputs it already has \(-2, 4, 30, 300\) to see what it does. In addition to drawing on the screen, it sets several variables that your other blocks will need so that they know the intended screen dimensions.
   2. The following two blocks report the Snap_! **stage **_coordinates given the _**graph **_coordinates of a point. Experiment with inputs to these two blocks to get them to report 0. ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/xStageforxGraph.png "xStage for xGraph: \(\)")

      ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/yStageforyGraph.png "yStage for yGraph: \(\)") How do your input numbers relate to the graph scale?

   3. Use![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/gotoxStageyStage.png "go to x: \(xStage for xGraph: \(\)\) y: \(yStage for yGraph: \(\)\)")with those same input numbers. Where does it put the sprite?

   4. Without changing the sprite's position, click ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/xGraphatxStagexposition.png "xGraph at xStage: \(x position\)")
      and explain the result you get.

   5. Use the

      ![](https://bjc.edc.org/bjc-r/img/blocks/when-I-am-dropped.png "When I am dropped") block to create a script that tells the sprite to say its correct _**graph **_coordinates \(not its _**stage **_coordinates\) wherever it is dropped. Move the sprite to a few places on the stage to test your script.

   6. For this graph, a sprite at the bottom right corner of the stage should say \(4, 30\), not \(240, -180\). To see the full display of coordinates use ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/roundto2decimal.png "round \(\) to \(2\) decimal places")

      block \(in the Operators palette, built for this project\) to round the coordinates reported to the decimal places you want to see. A display of ![](https://bjc.edc.org/bjc-r/img/3-lists/sprite-saying-two-decimal-places.png "sprite-saying-two-decimal-places") makes more sense than ![](https://bjc.edc.org/bjc-r/img/3-lists/sprite-saying-too-many-decimal-places.png "sprite-saying-too-many-decimal-places") in this context.
2. Experiment with various inputs to `set graph scale `to see where it puts the axes and how it represents the substitutes for the axes, when the point \(0, 0\) would not appear on the stage. Drag the sprite a few places to see if the sprite says what you expect. Then change the inputs of `set graph scale `to fit the range of years and percents in name data and click it to reset the scale of the screen. Again, check to see if your sprite says what you expect when you move it around the stage. ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/setgraphscale.png "set graph scale xMin:\(1927\) xMax:\(2014\) yMin:\(0\) yMax:\(0.5\)")

3. Build the following block which takes the _**graph **_coordinates of a data point and have the sprite go to the corresponding _**stage **_coordinates. ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/gotoxGraphyGraph.png "go to xGraph:\(x\#\) yGraph:\(y\#\)")On the baby name graph for Derek, the point \(1971, 0.25\) is roughly in the middle of the screen. Check to see if

   ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/gotoxGraph1971.png "go to xGraph:\(1971\) yGraph:\(0.25\)") is working as you expect it to. ![](https://bjc.edc.org/bjc-r/img/5-algorithms/PercentageOfDerekByYear.png "percentage of births named Derek by year")

4. Then, build ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/plotpointxGraphyGraph.png "plot point xGraph:\(\) yGraph:\(\)")so that it uses  
  


   ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/gotoxGraph.png "go to xGraph:\(\) yGraph:\(\)") instead of plain ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/gotoxy.png "go to x: \(\) y: \(\)")

   . Check it to make sure it works as you expect it to.

5. Finally, build ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/Graph%20datapoints.png "Graph datapoints: \(\)") to make a dot at every datapoint. \(For this graph, you will want the points connected. For the data on the next page you will want them separate. Make sure you design this block in a way that makes that feature easy to change.\) Apply it to `DerekData1927to2015`. The points of your graph may or may not be connected and the axes won't have labels, but it should otherwise look like the graph above.![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/ScatterPlotDerek.png "Scatter Plot of Derek Data unconnected")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/ScatterPlotDerekConnected.png "Scatter Plot of Derek Data connected")

6. Save your work as "U3L4-GraphingApp".

![](/assets/save.png)

#### If There Is Time...

1. Invent a way to tell your grapher, for each graph you make, whether to connect the points or not. You will want to have a Boolean input type for indicating if points are connected.  ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/Graphdatapointsconnected.png "Graph datapoints:\(DerekData1927to2015\) connected: \(true\)")



