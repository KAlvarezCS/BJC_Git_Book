# Developing a Number Guessing game with Script Variables

**In this lab,**you will use two kinds of variables to store information:

* _Script variables _\(a kind of local variable\) that can be used only within a single script, and
* Global variables that can be set, used, or changed anywhere in the program.

**On this page, **you will develop a number guessing game that uses a script variable to keep track of a secret number.

## Using a Script Variable \(a.k.a. Local Variable\)

You have created variables as inputs to blocks that you made:

![](http://bjc.edc.org/bjc-r/img/2-complexity/input-variable-for-pinwheelbranches-commented.png "block definition for pinwheel and setting &apos;number of branches&apos; input variable for pinwheel")

You have also used the variable that the `for `block gave you:

![](http://bjc.edc.org/bjc-r/img/2-complexity/local-variable-created-by-for-block-commented.png "local variable created by for block")

Input variables and `for `variables are kinds of **local variables**; they work only within the script in which they're created. If you drag one into a different script, it won't work. Sometimes you need to create more variables to hold information temporarily while your script is running. The `script variables `block lets you do that. ![](http://bjc.edc.org/bjc-r/img/prog/scriptvar.png "script variables")

For example, imagine a number-guessing game in which the player tries to guess the computer's secret number. The computer needs to store the secret number so that it can compare the player's guesses to it, but once the game is over, the secret number is no longer needed. If you play the game again, you want a new secret number.

**Vocabulary: Local Variable**

A variable that can be set or used only in the environment in which it is defined. This is the usual computer science term for variables that are defined as inputs to procedures or \(in Snap! and some other languages\) created by `for `or `script variables`.

#### For You To Do

1. Start a new project. Save it as "U2L1-NumberGuessing"
2. Create a new command block called `Number guessing game`.

3. Inside this block, create a script variable called secret number \(instructions below\), and set it to a random number between 1 and 10. **Making a Script Variable**

   1. **Move a **`script variables `**block into the Scripting Area. **You can find it in the Variables palette.![](http://bjc.edc.org/bjc-r/img/prog/scriptvar.png "script variables"). **Name the variable **by clicking on the orange a at the end and typing the name you want. Here, it should be called secret number.

      **Later, you will use the script variable **by dragging it out of the `script variables `block, the way you drag an input variable, and placing it where you need it in your code.

4. Use `set `to set the initial value of the variable. The down triangle lets you select the variable you want. Create code that sets secret number to a number randomly chosen from 1 through 10. ![](http://bjc.edc.org/bjc-r/img/2-complexity/set-secret-number-menu.jpg "set block menu selecting secret number")

The variable secret number is available in the `set `block only when you snap it into the same script that has the `script variables `block.

**Vocabulary: Initialize**

Setting the initial value of a variable is known as **initializing **the variable.

### Checking the Player's Guess

You'll want the computer to ask players to guess again and again until they get it right. To do that, you will use the `repeat until `block. `Repeat until `is a [loop](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/3-drawing/6-the-for-block.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment) \(just like `repeat`,`forever`, and `for`\) that **repeats until a certain **_**condition **_**is met**. In this case, the code should repeat until the player's answer equals the secret number.

`Repeat until `is a _conditional \_block \(like _`if`_\). Conditionals make choices based on a **condition **in the form of a **Boolean value **\(either_![](http://bjc.edc.org/bjc-r/img/blocks/true.png "true")_ or _![](http://bjc.edc.org/bjc-r/img/blocks/false.png "false")_\). The condition is checked by a predicate_, a true/false question such as ![](http://bjc.edc.org/bjc-r/img/2-complexity/a-gt-7.png "a&amp;gt; 7"). Predicates always report Boolean values. And they fit into hexagonal input slots, such as in ![](http://bjc.edc.org/bjc-r/img/blocks/if.png "if block") and ![](http://bjc.edc.org/bjc-r/img/blocks/repeat-until.png "repeat until"). Predicates help conditionals _decide when to do something_.

**Vocabulary: Boolean**

The word Boolean is capitalized because it's named after a person, George Boole, who invented the branch of mathematics dealing with Boolean operations \(such as `and`, `or`, and `not`\).

![](/assets/pair_programming.png)

#### For You To Do

1. Use `repeat until `to `ask `the player to guess the secret number until their `answer `equals the `secret number`.

   1. The ![](http://bjc.edc.org/bjc-r/img/blocks/ask-empty.png "ask \(\) and wait") and ![](http://bjc.edc.org/bjc-r/img/blocks/answer.png "answer") blocks go together. If you use `ask `to ask a question, the user's answer will be reported by `answer`.

2. After the player guesses the secret number, make the computer congratulate the player.

3. **Test and debug. **Take turns playing the game, and fix any problems with the code before moving on.

Checking that these pieces of your program work correctly before you go on will help make sure that you have a correctly working program at the end.

#### If There Is Time...

1. When the computer congratulates the player for guessing correctly, have the computer say the number. For example, it might say, "You guessed it! My secret number was 7."

Use `join `to merge the text "You guessed it! My secret number was" with the value of the secret number variable.

