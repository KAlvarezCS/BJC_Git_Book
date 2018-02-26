# Creating Bar Graphs

**In this project, **you will create a \_general purpose \_data visualization tool that can generate bar graphs for a variety of data sets. You will practice using \_abstraction \_and the higher order function `map`.

![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/CO2Table.png "Table of CO2 Emissions by Country")

![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/BarGraphAnimation.gif "bar graph of 2011 Top CO2 Emissions")

#### For You To Do

1. Technology has come at the cost of environmental pollution around the world. In collaboration with your partner, examine the data table given on [this link](http://www.ucsusa.org/global_warming/science_and_impacts/science/each-countrys-share-of-co2.html#.WVqJI9PytE5).

   1. What countries have the highest Carbon Dioxide \(CO2\) emissions?
   2. What countries have the highest CO2 emissions per capita \(per person\)?

   3. Which of these measures do you think is a better indicator a country's contribution to global environmental pollution?

   4. You can gain knowledge and insights by talking to others \(in person or online\) as you form questions and hypotheses about data.

2. [Click here to load. Save to your Snap! account. ](http://snap.berkeley.edu/snapsource/snap.html#open:https://bjc.edc.org/bjc-r/prog/3-lists/U3L4-BarGraph.xml)This file contains

   1. A \_constructor \_of a new ADT \(Abstract Data Type\) called `data-record`with two fields `label`and `value`.![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/datalabelvaluewithResult.png "data-record ADT")

   2. Two \_selectors \_for the new ADT, to extract specific data from a `data-record`input.

      ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/getlabelwithResult.png "label from data-record selector")  
      ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/getvaluewithResult.png "value from data-record selector")

   3. A `max of list `reporter that finds the largest element of a list. ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/maxoflistwithResult.png "max of list reporter")

   4. Explore these blocks already written for you and understand how they work.

3. Develop code for the draw axes block. It should draw the horizontal and vertical axes based on the given stage coordinates or the origin x0, y0 and the given length, height information.

   ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/drawAxis.png "draw axes block")This diagram may help you understand how the given information will determine the _horizontal _and _vertical _axes. As you will be graphing only positive values, the axes should meet in the lower left corner as shown in the diagram. There should not be any labels or tick marks at this point. The markings in the diagram are shown for clarity.![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/axeshorizvert.png "x-y axes")In the `draw axes `block also make sure that the coordinates of the origin is stored in global variables x-origin, y-origin. In the upcoming steps of this project, other blocks will need this information to properly align the bars and labels.![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/globalx0y0.png "Variables x-origin, y-origin")![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/setXYOrigin.png "Set x-origin, y-origin")

4. Explore the basic `label `block included in the starter project. Try changing the location and direction of the drawing sprite.![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/labelofsize.png "Basic label block")  
   Note that the `label `block does not need to have `pen down `in order to do its writing. Having `pen down `with the `label `block may cause some undesired effects.You're not required to look inside the `label `block, but if you do, you'll see something unfamiliar. 

   You can import the basic `label `block in your new projects via the "Import tools" option of the File menu:

   ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/importTools.png "Import tools option")[Click here for more.](https://bjc.edc.org/bjc-r/cur/programming/3-lists/4-graphing/1-bar-graphs.html?topic=nyc_bjc%2F3-lists.topic&course=bjc4nyc.html&novideo&noassignment#hint-1)You don't need to know how the `label `block works to be able to use it. By hiding its inner complexity from its users, the `label `block is a perfect example of _abstraction._

5. Use the basic `label `block to develop code for the more elaborate `label `block that will place a label with the inputted specifications \(text, size and direction.\) ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/labelChina.png "label block")![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/China.png "China label")Note that the orientation directions should follow Snap!’s convention for directions \(0 degree up, 90 degree right, 180 degree down, 270 degree left\). Test your new `label `with the four directions. ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/ChinaLabels.png "China label in 4 directions")

6. Develop code for the `draw bar `block. It should draw a vertical bar \(a line with the given width and height\) straight up from the current location with a label placed underneath the bar. You may wish to review your earlier [Brick Wall](https://bjc.edc.org/bjc-r/cur/programming/2-complexity/4-abstraction/3-brick-wall.html) project to remind yourself how to draw bars with a pen of a given width. You don't need to import `set flat line ends to `block from that project but make sure that you have "Flat line ends" selected from the Settings menu to draw rectangular bars. You can see below the difference in two types of lines drawn.

   ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/FlatLineEnds.png "Flat line ends option")![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/FlatLineBar.png "Flat line bar")![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/RoundedBar.png "Rounded line bar")

7. Develop code for the `draw bars `block, which should draw a series of labelled bars of the desired width and an appropriate height that start on the left and continue to the right. In order to properly level the bars and the labels you may need to refer to the global variables x-origin, y-origin. ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/drawthebars.png "draw bars block")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/bars.png "Country bars")

  
  
   Note that given a maximum bar height, the heights of all the bars can be computed as a fraction of this maximum bar height. Using the following proportion, you can derive each country's bar height: country bar height / max bar height = country data value / max data value

   For example, if maximum bar height=240 and you want to find how tall the bar for USA should be, you first find the largest value in the data set which is 8715 \(from China\) and do the following computation

   USA bar height = max bar height \* \(USA data value/ max data value\) = 240 \* \(5491/8715\) ≈ 151

   While finding the maximum of the data values, first you need to get a list of values and then apply the `max of list `block. The following block which uses the selector `value from data-record `will extract a list of _values _from the given data list.  
   ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/mapgetvalue.png "map value from data-record\(\) over \(data list\)")  

8. Develop code for the `label vertical axis `block so that it labels the vertical axis based on the specified inputs. For simplicity, you can assume that the labels will always split the vertical axis into 10 equal parts \(using 11 tick marks\) like this:![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/labelyaxis.png "label y-axis block")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/yaxislabels.png "y-axis labels")  

9. Now you are ready to put everything together and develop code for the `Bar Graph `drawing block for a given data list input. Fill in the blanks. ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/BarGraphdata.png "Bar Graph block")

10.  When everything is done, the following code, with a few extra labels for the graph title, should produce a bar graph as shown below: ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/codeCO2EmissionsData.png "Code for Bar Graph CO2 Emissions data") ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/CO2bargraph.png "Bar Graph of CO2 Emissions")

11. Your coding should be general enough to accommodate a new set of data \(also included in your starter file\): ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/codeCO2EmissionsPerCapita.png "Code for Bar Graph CO2 Emissions per capita data")

  


    ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/CO2EmissionsPerCapita.png "Bar Graph CO2 Emissions per capita")Note: "per capita" means "per person". So, for example for China, the total CO2 emissions was divided by the population: 8715 Million metric tons / 1.337 Billion persons = 6.52 metric tons per persons. These values are already given to you in the starter file as `CO2 Emissions per capita Data`.

12. In collaboration with your partner, compare the two bar graphs. What insights does each graph provide about CO

  
    ![](/assets/save.png)![](/assets/talk_with_partner.png)  
 

#### If There Is Time...

1. **Data Processing:** Look at the Variables palette to locate the `Country-GDP-Population Data `block. When you examine its contents you will notice that it is a list of lists containing data on the GDP \([Gross Domestic Product](https://en.wikipedia.org/wiki/Gross_domestic_product)\) and population size for each of the countries you studied in this project. _Process _the data so you can create a bar graph for the GDP **per capita **of each country. ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/Country-GDP-Population.png "Country-GDP-Population Data")Click here for a [hint](https://bjc.edc.org/bjc-r/cur/programming/3-lists/4-graphing/1-bar-graphs.html?topic=nyc_bjc%2F3-lists.topic&course=bjc4nyc.html&novideo&noassignment#hint-2) on how to _process _data quickly using the higher order function `map`.
2. Now collect some data in your class or from the internet on a topic you care about that would lend itself to visualization with a bar graph. Use your Snap! program to visualize your data. Share your work with your classmates.

#### Take It Further

1. Sometimes it is more convenient to present your bar graph with horizontal bars instead of vertical ones. Modify your code so that it takes an input indicating which type of bar graph \(horizontal or vertical\) is to be generated. ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/HorizontalBarGraph.png "Horizontal Bar Graph")

2. Histograms display _numerical _data grouped into ranges \(called bins\) and plotted as bars. For example, the histogram below shows the number of students in each age group at a summer camp. Learn about histograms and create a data visualization tool in Snap_! _for displaying histograms. ![](https://bjc.edc.org/bjc-r/img/3-lists/BarGraph_img/Histogram.JPG "Histogram")

  
  

####  

#### 

  
  
  


  


  




