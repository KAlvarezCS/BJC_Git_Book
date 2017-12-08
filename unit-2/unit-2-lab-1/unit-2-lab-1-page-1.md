# Developing a Number Guessing game with Script Variables

**In this lab,**you will use two kinds of variables to store information:

* _Script variables _\(a kind of _local _variable\) that can be used only within a single script, and
* _Global variables _that can be set, used, or changed anywhere in the program.

**On this page,**you will develop a number guessing game that uses a script variable to keep track of a secret number.

## Using a Script Variable \(a.k.a. Local Variable\)

You have created variables as inputs to blocks that you made:  


![](http://bjc.edc.org/bjc-r/img/2-complexity/input-variable-for-pinwheelbranches-commented.png "block definition for pinwheel and setting &apos;number of branches&apos; input variable for pinwheel")

You have also used the variable that the `for `block gave you:  


![](http://bjc.edc.org/bjc-r/img/2-complexity/local-variable-created-by-for-block-commented.png "local variable created by for block")

Input variables and `for `variables are kinds of **local variables**; they work only within the script in which they're created. If you drag one into a different script, it won't work. Sometimes you need to create _more _variables to hold information temporarily while your script is running. The `script variables `block lets you do that. ![](http://bjc.edc.org/bjc-r/img/prog/scriptvar.png "script variables")

For example, imagine a number-guessing game in which the player tries to guess the computer's secret number. The computer needs to store the secret number so that it can compare the player's guesses to it, but once the game is over, the secret number is no longer needed. If you play the game again, you want a new secret number.

**Vocabulary: Local Variable**

A variable that can be set or used only in the environment in which it is defined. This is the usual computer science term for variables that are defined as inputs to procedures or \(in Snap_! _and some other languages\) created by `for `or `script variables`.

#### For You To Do

1. Start a new project. Save it as "U2L1-NumberGuessing"
2. Create a new command block called `Number guessing game`.

3. Inside this block, create a script variable called secret number \(instructions below\), and set it to a random number between 1 and 10. **Making a Script Variable**

   1. **Move a**
      1. **`script variables `block into the Scripting Area. **You can find it in the Variables palette.![](http://bjc.edc.org/bjc-r/img/prog/scriptvar.png "script variables")
      2. **Name the variable **by clicking on the orange a at the end and typing the name you want. Here, it should be called secret number.

      **Later, you will use the script variable **by dragging it out of the `script variables `block, the way you drag an input variable, and placing it where you need it in your code.



