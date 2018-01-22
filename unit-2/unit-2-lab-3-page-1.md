# What's a Predicate?

**In this lab,**you will develop a word puzzle solver that will search through a long list of words and report words with specific characteristics.

**On this page**, you will review predicates and build a few that you can use in other projects.

### Predicates

**Predicates are reporter blocks \(functions\) that always report a**_**Boolean value**_\(they report only the values![](http://bjc.edc.org/bjc-r/img/blocks/true.png "true")or![](http://bjc.edc.org/bjc-r/img/blocks/false.png "false")\). In Snap_!_, they are represented by hexagonal blocks.

You have seen predicates before. Predicates compute the_condition_used by_conditionals_\(such as`if`or`repeat until`\) to decide when to do something. Predicates ask a question such as "Does theplayer listcontain the player's`answer`?" or "Is this sprite touching the sprite called 'Sprite'?"  
[![](http://bjc.edc.org/bjc-r/img/1-introduction/greet-player-skeleton.png "greet player skeleton")](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/2-gossip-and-greet/4-learning-names.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment)[![](http://bjc.edc.org/bjc-r/img/1-introduction/move-tiny-no-comment.png "sprite following sprite code")](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/5-follow-the-leader/2-sprite-interaction.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment)

#### For You To Do

1. Start a new project. Save it as "U2L3-Predicates"
2. In the last lab \(and also way back in [Unit 1 Lab 5](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/5-follow-the-leader/1-following-sprites.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment)\), you made scripts to get the sprite to follow the mouse.  
   ![](http://bjc.edc.org/bjc-r/img/2-complexity/U2-follow-that-mouse.png "go to x: \(mouse x\) y: \(mouse y\)")

   Now create a script that lets you use your mouse to write on the stage in two colors depending on the mouse's position on the stage: ![](http://bjc.edc.org/bjc-r/img/2-complexity/writing-mouse-on-stage.gif)

   Use one of these equality/inequality predicates:  
   ![](http://bjc.edc.org/bjc-r/img/2-complexity/relations.jpg "less than, equal to, and greater than predicate blocks")

   #### If  There Is Time...

3. #### Improve your drawing script so that the sprite always follows the mouse, but draws only when the mouse button is down, so that you can draw disconnected shapes.

   Uncheck the "draggable" box above the scripting area before you try this \(so that Snap_!_

   doesn't think you are trying to drag the sprite when you click\). ![](http://bjc.edc.org/bjc-r/img/2-complexity/draggable-check-box.png "draggable box checked")

   You'll probably want to use the ![](http://bjc.edc.org/bjc-r/img/blocks/mouse-down.png "mouse down? predicate block") block, which you can find in the Sensing palette.

   #### For You To do

4. #### Build a predicate that tells whether an input number is between two other numbers, and test it with several different cases.

  


   ![](http://bjc.edc.org/bjc-r/img/2-complexity/number-between-two-others%28with-result-false%29.png "number-between-two-others\(with-result-false\)")

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/number-between-two-others%28with-result-true%29.png "number-between-two-others\(with-result-true\)")

   #### **Making a Predicate**

   * Choose the hexagonal _predicate _shape.
     ![](http://bjc.edc.org/bjc-r/img/2-complexity/make-predicate.png "Make a block dialog highlighting the predicate button")
   * You must use the ![](http://bjc.edc.org/bjc-r/img/blocks/report.png "report") block to report the result of reporter functions \(including predicate functions\).

   ##### Vocabulary

   * Many languages \(and the AP CS Principles Exam\) use `return `instead of `report `as the name of the command to give a value back at the end of a function call.



   1. Build a predicate that tests for divisibility by following the steps below.
      ![](http://bjc.edc.org/bjc-r/img/2-complexity/15-divisible-by-3-reporting-true.png "\(15\) divisible by \(3\) ? reporting true")
      ![](http://bjc.edc.org/bjc-r/img/2-complexity/15-divisible-by-6-reporting-false.png "\(15\) divisible by \(6\) ? reporting false")
      1. First, experiment with the `mod `block.
         1. **Try various inputs**.
         2. **Keep the second number constant **, and try various inputs for the first number.
         3. **Form a hypothesis. **What do you notice?
      2. The![](http://bjc.edc.org/bjc-r/img/blocks/mod.png "\(\) mod \(\)")block **reports the remainder **when the first input is divided by the second. For example,![](http://bjc.edc.org/bjc-r/img/1-introduction/17-mod-5.png "17 mod 5")reports 2 because when 17 is divided by 5, the remainder is 2. When one number divides another evenly, the remainder is 0. So,![](http://bjc.edc.org/bjc-r/img/1-introduction/15-mod-5.png "15 mod 5")reports 0.

      3. Now, define the ![](http://bjc.edc.org/bjc-r/img/2-complexity/divisible-by.png "\(\) divisible by \(\) ?") predicate using `mod`
         .
   2. Use your`divisible `predicate to build a predicate that tests whether its input is even \(divisible by 2\).
      ![](http://bjc.edc.org/bjc-r/img/2-complexity/even--22-reporting-true.png "even? \(-22\) reporting true")
      ![](http://bjc.edc.org/bjc-r/img/2-complexity/even-7-reporting-false.png "even? \(7\) reporting false")
      ![](http://bjc.edc.org/bjc-r/img/icons/save-now.png "Now Is a Good Time to Save")
      In this picture, the even and odd numbered rows are different. In the next lab, you will use your
      `even?`block to draw a [brick wall](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/4-abstraction/3-brick-wall.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment).![](http://bjc.edc.org/bjc-r/img/abstraction/new-brickwall/wall.png "Sample image of brick wall") 

#### If There Is Time...

Build a predicate that tests whether its input is an integer. You may find ![](http://bjc.edc.org/bjc-r/img/blocks/round-a-number.png "round \(\)") useful.

![](http://bjc.edc.org/bjc-r/img/2-complexity/integer-4%28with-result-true%29.png "integer? \(4\) reporting true") ![](http://bjc.edc.org/bjc-r/img/2-complexity/integer-4-point-1%28with-result-false%29.png "integer? \(4.1\) reporting false")

