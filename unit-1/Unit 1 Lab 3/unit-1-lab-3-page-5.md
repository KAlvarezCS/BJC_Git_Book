# Remix Your Pinwheel

**On this page,** you will use your existing `pinwheel `block to make `asterisk `and `polygon `blocks.

![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/asteriskpolygonCycle.gif "Animation cycle from Asterisk to Polygon")

You can use your _general_-purpose pinwheel procedure to create other, simpler _special_-purpose procedures that each do a particular job.

### For You To Do

1. If it isn't open already, open your U1L3-Pinwheel project from the previous page.
2. Use your `pinwheel `block to create a more specialized `asterisk `block.

   1. First, [make a new block](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/2-gossip-and-greet/3-making-a-new-block.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment) called `asterisk `with two variables: one for the number of branches and one for the length of each branch.![](http://bjc.edc.org/bjc-r/img/1-introduction/asterisk-using-pinwheel.png)

   2. Now fill in the three inputs to `pinwheel `so that it correctly draws an asterisk.![](/assets/pair_programming.png)

   3. Similarly, write a `polygon `block that uses `pinwheel `with appropriate inputs to draw a polygon with a given number of sides and side length.

      **Vocabular**y

      Using a block you've already written to help write another block is an example of **abstraction**. Abstraction is arguably the most important idea in computer science, but it doesn't have a simple definition. Here, abstraction means using a more general block \(`pinwheel`\) to create two more specific blocks \(`asterisk `and `polygon`\). There are other kinds of abstraction too, and we'll point them out as they come up. In the meantime, if you find yourself wanting to copy code from one place to another, consider _abstracting _by writing a general block to use in both places instead.

3. If you look inside of `pinwheel `and see how you're using it in `polygon`, you'll see that there are steps that you don't really need for the case of a polygon. Write another version of `polygon `built directly out of primitive blocks \(`move`, `turn `and so on\). How simple can you make it?

![](/assets/save.png)

#### If There Is Time...

1. Use your `pinwheel `block code one last time to create a `circle `block that accepts one input for the size.
2. Use the `random `block together with `set pen color `and `set pen size `to draw a variety of shapes.
 
   ![](http://bjc.edc.org/bjc-r/img/1-introduction/assorted-pinwheels.png "assortment of pinwheels")



##### Take It Further

1. Challenge:** **Create a script that draws a blue square of size 100 and then draws a red circle that fits perfectly inside it.
   ![](http://bjc.edc.org/bjc-r/img/1-introduction/red-circle-in-blue-square.png "red circle in blue square")
2. In each of the puzzles below you will need to write code that will allow a car to travel from its starting point \(A\) to its final destination. Click on each of the images to load each Snap_! _project.
   [![](http://bjc.edc.org/bjc-r/img/1-introduction/PolygonalRacetracks_img/ArchTess1.png "Triangle and square tesselation path")](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/1-introduction/U1L6-archimedean-racetrack1-student.xml)
   [![](http://bjc.edc.org/bjc-r/img/1-introduction/PolygonalRacetracks_img/ArchTess2.png "Triangle, square and hexagon tesselation path ")](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/1-introduction/U1L6-archimedean-racetrack2-student.xml)
   [![](http://bjc.edc.org/bjc-r/img/1-introduction/PolygonalRacetracks_img/ArchTess3.png "Octagon and square tesselation path")](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/1-introduction/U1L6-archimedean-racetrack3-student.xml)











