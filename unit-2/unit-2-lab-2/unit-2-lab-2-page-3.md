# Capturing Clicks as Points

On the previous page, you drew a shape based on a list of points you were given. **On this page, **you will automate the process of getting coordinates by clicking on the desired points on the screen.

#### Thinking Out Loud

Betsy and Alphie are still using coordinate lists to draw letters. ![](http://bjc.edc.org/bjc-r/img/icons/take-turns-speaking-mini.gif "Take turns speaking")

**Alphie:** Typing in all these coordinates is a pain. Let's write a program so that if we have a picture, we can click on the corners and let the program collect the coordinates?

**Betsy:** Great idea. And I know that we can import images as a stage background, so all we have to do is....

#### For You To Do

1. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/2-complexity/U2L2-Capturing-Points.xml) Export your new drawing blocks and abstract data type from your "U2L2-DrawShape" project, import them into this new project and save it again.
2. Select a stage background of your choice.

   #### **Setting the Stage Background**

   1. **Click the Stage button**
      below the actual stage. 
      ![](http://bjc.edc.org/bjc-r/img/2-complexity/stage-button.png "stage button in sprite corral")
   2. **Click the "Backgrounds" tab **near the top of the window. 
      ![](http://bjc.edc.org/bjc-r/img/2-complexity/backgrounds.png "backgrounds tab") 
   3. **Select or import a stage background.**
      In this project, you will find two imported backgrounds:
      * A graph of median U.S. household income by year \(source: Federal Reserve Bank of St. Louis\)
      * A capital "E" \(font: Century Gothic Bold\).
      * The graph is typical of data processing, which is one topic of Unit 3. The E continues the activity from the previous page. Choose either background by clicking on it.

#### Thinking Out Loud

**Alphie:** We'll have to initialize the point list variable to an empty list first.

**Betsy:** And we know how to make the sprite follow the mouse; we did it in [Unit 1](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/5-follow-the-leader/1-following-sprites.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment).

**Gamal:** Yes, and every time we click, we want to add the position to a list as we did in [the Unit 1 "Greet Player" project](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/2-gossip-and-greet/4-learning-names.html).

**Gamal:** When we click, we should give the user some feedback that the click has been processed.

**Alphie:** What do you mean? Like a sound?

**Gamal:** Maybe, but I was thinking we should mark each point somehow so we feel confident the computer is recording our clicks.

**Alphie:** I have an idea! There's a ![](http://bjc.edc.org/bjc-r/img/2-complexity/stamp.png "stamp block \(in Pen\)") block that stamps a picture of the sprite right where it is on the stage.

**Gamal:** Great. And the Turtle sprite will leave stamps pointing right where the user clicks.

Alphie, Betsy, and Gamal develop code to implement their ideas.

![](http://bjc.edc.org/bjc-r/img/2-complexity/U2ImageVideoAddendum_img/drawEAnimation.gif)

#### For You To Do

The project file you loaded contains three unfinished scripts, one for each of these steps. Finish all of these scripts.

If you haven't already, you'll need to go back to the Scripts tab and choose the "Sprite" button under the stage to get back to the sprite's scripts.

1. First, give an appropriate initial value to the point list variable.
2. In the second script, you need a way to tell the sprite to stop following the mouse. Replace the `forever `block with one that will loop only until the user presses the space key.
3. In the third script, the `stamp `block is already in place, but you have to write the code that will add the mouse's position to the list of points. Use your abstract data type.

![](/assets/save.png)

#### Take It Further

For the purpose of entering points interactively, the approach on this page is all you need. But if you wanted to create a more robust point-gathering program, this approach has a couple of weaknesses:

* Even after you tell the sprite to stop following the mouse, the "when I am clicked" script is still ready to run, so if you click directly on the sprite, it will still add points to the list. You may not want that.
* The list of points is always kept in the same global variable. So it's messy to create lists for several different letters.

* Think, and see if you can find your own way to solve one or both of these problems.

* Here is [an alternative approach](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/old/5-click-points.html) that contains a new idea that you might like. There are simpler solutions than this, but the idea behind this slightly more complicated code is a useful one.



