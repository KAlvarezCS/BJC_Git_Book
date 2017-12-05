# Looping with a Counter

You've seen these ways to repeat a set of commands:

* ![](http://bjc.edc.org/bjc-r/img/blocks/forever.png "the forever block") repeats the same commands _forever_. \(You used it to [make Alonzo keep moving](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/1-building-an-app/6-keeping-score.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment).\)

* ![](http://bjc.edc.org/bjc-r/img/1-introduction/repeat.png "the repeat block")repeats them _a specific number of times. _\(You used it to [draw shapes](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/3-drawing/1-exploring-motion.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment).\)

**Vocabulary**

Computer scientists describe this program structure as looping, repetition, or **iteration**. [Sequencing, selection](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/2-gossip-and-greet/4-learning-names.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment#AP), and iteration are building blocks of algorithms.

The `forever`block generates an infinite loop that goes on forever. An infinite loop can sometimes be the result of a bug, but in some interactive programs, you want the program to keep running until stopped by the user.

**On this page, **you will use `for`loops to repeat \_and count the repetitions \_so you can use that counter to draw shapes with repeated patterns...![](http://bjc.edc.org/bjc-r/img/prog/spiral.png "spiral")![](http://bjc.edc.org/bjc-r/img/1-introduction/nested-squares.png "nested squares")

You can use ![](http://bjc.edc.org/bjc-r/img/prog/for.png "for") to name a variable \(here, ![](http://bjc.edc.org/bjc-r/img/blocks/variable-i.png "i")\) that counts each repetition, and you can use that counter variable in the repeating script. For example, the `for`block lets you simplify long scripts like:

![](http://bjc.edc.org/bjc-r/img/looping/for-loop-equivalent.png "say \(1\) for \(2\) secs, say \(2\) for \(2\) secs, say \(3\) for \(2\) secs... say \(10\) for \(2\) secs")   to![](http://bjc.edc.org/bjc-r/img/looping/for-loop-drag-i.gif "for \(i\) \(1\) to \(10\) \[say \(Hello!\) for \(2\) secs")Each time the `for`block runs the script inside, it changes the value of the variable by 1, counting from the first input number to the second.$$$$

![](http://bjc.edc.org/bjc-r/img/icons/import-tools.png "Import Tools")In the current version of Snap!, the `for`block isn't installed automatically. You'll need to import tools once into each new Snap project where you need `for`and some other important tools.

![](http://bjc.edc.org/bjc-r/img/1-introduction/import-tools.png "select &apos;Import tools&apos; from the Snap! file menu")

#### For You To Do

1. Click on the File![](http://bjc.edc.org/bjc-r/img/sys/button-file-menu.png "File menu icon") menu at the top of the Snap! window and select "Import Tools."

   1. The for block gives you a default variable, i\(for index\). You can change the name of this variable by clicking it. Once changed, drag it out and use it just like any variable.

2. Build this script that makes the sprite say the numbers 1 through 10.v![](http://bjc.edc.org/bjc-r/img/1-introduction/for-i-1-10-say-i.png "for \(i\) = \(1\) to \(10\) \[say \(i\) for \(2\) secs\]")

   1. Then modify it so that the sprite says 0, 2, 4, 6, 8, ... up through 30.
   2. Discuss your solutions with another pair.

3. Experiment with spirals.

   1. Build this script and try it out: This design got the nickname "squiral" because it's a square spiral.  
      ![](http://bjc.edc.org/bjc-r/img/looping/squirral-script.png "squiral script")

   2. ![](http://bjc.edc.org/bjc-r/img/icons/talk-with-your-partner.png "Talk with Your Partner")Make sure you can explain why the squiral spirals outward.

   3. Try switching the order of the 100 and the 1 in the `for`block in the squiral script. What is the result?
   4. Try changing the turning angle in the squiral script to other numbers such as 92, 126, etc.
   5. Change the inputs to `turn`and `move`to get as close as you can get to a smooth spiral:

      ![](http://bjc.edc.org/bjc-r/img/prog/spiral.png "spiral")

4. Save this as "U1L3-Squiral"

#### If There Is Time...

1. Open your U1L3-Pinwheel project, and build a `nest squares`block that uses `for`and your `polygon`block to draw nested squares. Give it an input so that it will draw whatever number of squares you specify, with each square larger than the previous: ![](http://bjc.edc.org/bjc-r/img/1-introduction/nested-squares.png)
2. Build `nest polygons`that accepts the number of polygons and the number of sides for the polygons.

3. Build a script that draws 12 regular polygons, each with one more side than the previous one, as shown below. ![](http://bjc.edc.org/bjc-r/img/1-introduction/polygons.png)

4. Predict what this script will do before you try it: ![](http://bjc.edc.org/bjc-r/img/1-introduction/nested-fors.png)



#### Take It Further

1. Build a script that counts down by 10 from 100 to 0 \(that is, 100, 90, 80, etc.\).

2. Find a way to use `for `to nest squares this way. Build your _block _with two inputs that let you specify how many squares the design will contain and how much bigger each square will be than the previous one.![](http://bjc.edc.org/bjc-r/img/icons/tough-stuff.png "Tough Stuff")
   ![](http://bjc.edc.org/bjc-r/img/1-introduction/concentric-squares.png "concentric squares")
3. Below are two animations that use the `pinwheel `code with inputs. Find out how to create your own artistic animations.![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/pinwheelArray "Array of pinwheels animation")

   ![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/PinwheelWreathAnimation.gif "Pinwheel wreath animation")The following code may give you ideas about how to create animations. Make sure to remove all`wait`0.5`secs`blocks from your`pinwheel`code so they don't slow it down. The`warp`block allows the drawing of the pinwheel all at once.

   ![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/animationCode.png "Code for creating animation")

1. ![](/assets/u1l3p6.png)![](http://bjc.edc.org/bjc-r/img/icons/tough-stuff-mini.png)![](http://bjc.edc.org/bjc-r/img/icons/tough-stuff-mini.png) This block is like the squiral, but instead of changing the input to `move`, it changes the input to `turn`: ![](http://bjc.edc.org/bjc-r/img/1-introduction/inspi.png)
   1. Try sketching what it will draw with an angle of 2.
      Then build it, and try each of these tests:
      You can stop each test with the stop button \(![](http://bjc.edc.org/bjc-r/img/1-introduction/stop_button.png "stop button")\) when you're sure nothing new will happen, but don't decide that too quickly!
      ![](http://bjc.edc.org/bjc-r/img/1-introduction/inspi-tests.png "inspi with \(1000,10,80\), \(1000,5,1\), \(1000,5,7\), \(1000,5,13\), \(1000,10,77\)")
   2. What's going on? Can you work out a theory to predict anything about the shape it draws for a particular angle input? \([Don't click unless you really, really need a super big hint.\)](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/3-drawing/6-the-for-block.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment#hint-1)



