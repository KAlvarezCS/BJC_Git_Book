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

   1. The

      for

      block gives you a default variable,

      i\(for index\). You can change the name of this variable by clicking it. Once changed, drag it out and use it just like any variable.



