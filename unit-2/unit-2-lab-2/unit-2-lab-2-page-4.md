# Mandala Design

**On this page, **you will create a design called a _mandala_.

![](http://bjc.edc.org/bjc-r/img/2-complexity/Mandala_img/MandalaEvolution.gif "Mandala Evolution")

#### For You To Do

1. ![](/assets/twoPeopleThinking.png)Figure out a possible algorithms for drawing this mandala: ![](http://bjc.edc.org/bjc-r/img/2-complexity/Mandala_img/10-gon-with-diagonals.png)

#### Thinking Out Loud

**Alphie:** The outside of the mandala is a 10-sided polygon. We already created a block to draw a polygon, but connecting the vertices will be a pain.

Alphie opens their polygon project.

![](http://bjc.edc.org/bjc-r/img/2-complexity/polygonCode.png "polygon code")

**Betsy: **So let's make our `polygon `block store each vertex as a `point `while it draws the polygon. We listed points as \_we \_clicked on them. This is the same, but with the program generating the points.

**Gamal:** Right! Set up a empty list variable first, and then use ![](http://bjc.edc.org/bjc-r/img/3-lists/add%28%29to%28%29.png "the add block") inside the `polygon `block.

**Alphie:** Global variable or a script variable?

**Gamal:** Well, we need to use it inside `polygon `and in the script that draws the mandala, so I'd make it global so multiple scripts can access it.

**Betsy: **I have an idea for the part of the program that actually draws the diagonals.Betsy sketches this:![](http://bjc.edc.org/bjc-r/img/2-complexity/Mandala_img/Stage2.png "Stage 2 of Mandala")

**Gamal:** Smart! We'll draw all the diagonals from one vertex as a subproblem.

**Alphie:** Perfect! Pick one vertex and use `for each `to connect just that one to each other vertex. After that, it's easy! We can use that block on each vertex.

#### **Problem Decomposition - **Solving a complex problem by building small tools and combining them to make bigger ones.

#### For You To Do

1. Now build your own program to draw
   ![](http://bjc.edc.org/bjc-r/img/2-complexity/Mandala_img/10-gon-with-diagonals.png "10-gon with diagonals")by decomposing the problem into manageable small parts.

#### Take It Further

1. Here are some variations. Create your own.

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/Mandala_img/Mandala4b.png "Denser Mandala")  
   ![](http://bjc.edc.org/bjc-r/img/2-complexity/Mandala_img/Mandala2.png "Four Mandalas")  
   ![](http://bjc.edc.org/bjc-r/img/2-complexity/Mandala_img/Mandala3b.png "Mandala Ring")

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/Mandala_img/ColorMandala3.png "Colored Mandala Ring")  
   ![](http://bjc.edc.org/bjc-r/img/2-complexity/Mandala_img/ColorMandala2.png "Colored Four Mandalas")  
   ![](http://bjc.edc.org/bjc-r/img/2-complexity/Mandala_img/ColorMandala1.png "Colored Denser Mandala")

2. Some cultures see mandalas as symbols of interconnectedness and harmony. Do some research on mandalas across different cultures and present your findings to your classmates. Try writing programs to reproduce some that you find.



