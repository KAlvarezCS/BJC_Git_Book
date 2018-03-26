# Debugging and Extending Your Number Guessing Game

**On this page, **you will debug a Number Guessing game script, and you will make the computer tell players whether their guesses are too big or too small.

#### For You To Do

1. **Analyze and Debug.**  
   1. This definition for a `Number  guessing game `block has a **bug **—an error in the code that makes the program behave differently than expected. This code, if you keep playing over and over, will mostly work, but _sometimes _\(not often\) it will congratulate you _before you even guess_.

   If you build this to try it out, have it pick its random number just from 1 to 3 to make the bug occur more often.  
      ![](http://bjc.edc.org/bjc-r/img/2-complexity/number-guessing-game-definition.png "Number guessing game block definition")  
      [Click here if you want a hint.](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/1-variables-games/2-debugging-extending.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment#hint-1)

   * **Think and Write:**
     ![](http://bjc.edc.org/bjc-r/img/icons/talk-with-another-pair.png "Talk with Another Pair")
     Analyze the code, or experiment with it, and explain how this can happen.
     1. If it isn't open already, open your U2L1-NumberGuessing project.
     2. There are a few different ways to fix the bug.
        [Click here for one way, after thinking about it yourself.](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/1-variables-games/2-debugging-extending.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment#hint-2)
        If you want to add more script variables, use the right-pointing triangle. \(The left triangle will remove them.\)![](http://bjc.edc.org/bjc-r/img/2-complexity/script-variables-adding.gif)
     3. **Test and debug **your code.

   ### Extending the Program with More Specific Responses

   #### For You To Do

2. 1. Use more conditional blocks and predicates to make the computer tell the player whether a guess is too big or too small: "That's too big. Try again."

      ![](http://bjc.edc.org/bjc-r/img/icons/talk-with-your-partner.png "Talk with Your Partner") Where in the code should these conditionals go?

   2. **Test and debug.**  
      Play your game enough to see if it works the way you want. It should:

      * ask the player to guess its secret number;
      * say whether a wrong guess is too big or too small, and then ask again;
      * congratulate the player for a correct answer.

   Script variables exist only while the script is running, so the secret number variable will not exist after `Number guessing game `finishes running. When played again, the program will create a new secret number variable and initialize it with a random number.

   ![](http://bjc.edc.org/bjc-r/img/icons/save-now.png "Now Is a Good Time to Save")

   In a later unit, you will teach the computer how to guess a secret number that you have chosen.

   #### If There Is Time...

3. Right now, the script always picks a number between 1 and 10. At the start of the game, ask the player what the maximum number should be, and make your program choose a number between 1 and maximum .  
   1. Use another script variable to keep track of how many guesses the player makes before getting the right number. When the player guesses the secret number, say how many guesses it took.  
   2. Find a way to vary the language a bit so that your program does not always repeat exactly the same words in the same situation. For example, if a player guesses too high twice in a row, the program could say "That's still too big. Try another number."



