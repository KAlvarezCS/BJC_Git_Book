# Improving Your Graphic App

**On this page **, you'll work with a dataset on a classroom of 27 sixth-graders. You will create a graph of height vs. weight, showing the boys and girls in different colors that also allows you to examine individual data points to see their approximate values, like this: ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/GraphingDataSet.gif "animation of a data set being graphed")

#### For You To Do

1. Load your grapher from before; it should have been saved as "U3L4-GraphingApp."
2. Look in the Variables palette for this dataset on a classroom of 27 sixth-graders:![](https://bjc.edc.org/bjc-r/img/5-algorithms/Gr6-age-height-weight-gender-stats.png "Gr6-age-height-weight-gender-stats"). Each data point in this set represents a person and contains _four _items:![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/persondata2.png "list \(137.4\)\(146.52\)\(40.52\)\(F\)")

   1. age in months

   2. height in centimeters

   3. weight in kilograms

   4. gender

   Your grapher was written to expect only _two_ numbers in each datapoint. Will it even work with this dataset? Try it. What does it do?

3. Create a selector `age `which extracts the age of an input person. ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/ageperson.png "age, person: \(person\){report\(item\(1\) of \(person\)\)}")

4. Similarly, create selectors height, weight, gender which extract the height, weight, and gender of an input person.

5. Now use the above selectors to create custom blocks that report:

   1. ages - a list containing only the 27 ages

   2. heights - a list containing only the 26 heights

   3. weights - a list containing only the 27 weights

   For example: you can use the Higher Order Function `map `together with the selector `age `to extract a list of ages from the data:

   ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/agesdata.png "ages, data: \(data\){report\(map\(age, person\(\)\) over\(data\)}")  

6. Create a block that takes a list of numbers as input and reports the

7. Create a block, female data, using keep, that reports a list containing all the data points of only the girls, and another block, male data, that does the same for the boys.
8. You now have everything you need to create a graph of height vs. weight, showing the boys and girls in different colors that also allows you to examine individual datapoints to see their approximate values, as shown in the animation above. Build it.

   1. The following blocks may help you extract the information you need from the data set. ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/hintblocks.png "map \(\) over \(\); list\(height, person:\(\)\)\(weight, person:\(\)\); male data, data: \(\); Gr6 age-height-weight-gender stats")  

9. You will need to`set graph scale `for each of these graphs. Searching through the data to find the lowest and highest values can be a nuisance. Create tools to do that for you.![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/minoflist.png "min of list \(\)")![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/maxoflist.png "max of list \(\)")

10. Use the tools you have built to create a few separate graphs: age against height or weight, height against weight, separated or not separated by gender—and _also mark the averages _in each case. What can you say about this particular class of sixth-graders based on the data?

Collaboration is vital to solving data driven problems because it allows the application of multiple perspectives and skill sets to gain insights and knowledge about data that may not be possible when working alone. ![](/assets/talkpair.png)

#### Take It Further

1. The graph above shows _three _aspects of each child in the class \(height, weight, and gender\). Find some suitable way to give some information about the fourth element of the data \(age\). Pen size is one possibility, but you might find a different way. ![](https://bjc.edc.org/bjc-r/img/3-lists/U3ImageVideoAddendum_img/agebyPensize.png "Graph of height versus weight with gender by color and age by pen size")

  

  




