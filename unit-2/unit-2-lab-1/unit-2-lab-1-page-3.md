# Keeping Score with Global Variables

**On this page, **you will use a _global variable _to keep score in your Click Alonzo game.

In your Number Guessing Game, you used _script variables _to store information \(the value of secret number\) that only one script needed. To keep score in Click Alonzo, more than one script will need access to that information, so you'll use a _global variable_.

If multiple scripts need access to a variable, or if the information in that variable needs to be saved with your file, you'll use a global variable. Otherwise use script variables.

#### For You To Do

1. Open your U1L1-ClickAlonzo project, play the game, and review the code so you remember how it works.
2. Save this as "U2L1-ClickAlonzo Be sure to **rename your project **with "U2" in the filename. If you save this work under the old filename, Snap_! _will overwrite your Unit 1 project. Use "Save as..." to save with the new name. When you load an older project and are about to make a big change, get in the habit of _saving first, before you change anything_.
3. Create a global variable named score. Here's how. **Making a Global Variable**
   1. **Click **![](http://bjc.edc.org/bjc-r/img/1-introduction/make-a-variable.png "make a variable button") **in the Variables palette. **\(It's not a block; you can't drag it into the scripting area.\)
   2. **Type the title **for your variable. In this case, it's score. Click OK.

 
4. Use the score variable to keep track of the player's score:

   1. Initialize score to 0 at the beginning of the game.

   2. Make the program change the score by 1 whenever the sprite is clicked.

5. **Test and debug. **Play the game enough to make sure that the score variable works.

You can use![](http://bjc.edc.org/bjc-r/img/2-complexity/change-score-by-1.png "change score by \(1\)") or ![](http://bjc.edc.org/bjc-r/img/2-complexity/set-score-to-score-plus-one.png "set-score-to-score-plus-one"). The AP CSP Exam represents the same code this way:

```
score ← score + 1
```

![](/assets/pair_programming.png)![](/assets/save.png)

#### For You To Do

1. ![](/assets/talk_with_partner.png) Right now, the game never ends, but you'll change that. Decide on the score that you will use to test whether the player has won.
2. Use a conditional to determine when the player reaches that score. When they do:
   1. Stop all but this script so Alonzo stops jumping around.

   2. Make Alonzo appear again. \(You'll have to reset the ghost effect.\)
   3. Congratulate the player for a few seconds.
   4. If necessary, use another `stop `block to stop the running script. \(Whether you need this will depend on your program structure.\)
3. **Test and debug.** Take turns playing, and fix any bugs.

![](/assets/save.png)

#### Take It Further

1. If the sprite moves without being clicked, make the score go down by 1.



