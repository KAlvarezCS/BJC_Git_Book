## Mastermind

**In this project, **you will begin to build the game Mastermind™. In this game, one player selects a sequence of four secret colors, and the other player tries to guess it.

![](http://bjc.edc.org/bjc-r/img/1-introduction/mm-snapshot.png "Snapshot of game")

#### For You To Do

1. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/1-introduction/mastermind-starter.xml)
   1. Look at the scripts. there are six sprites, four for the player's guess and two for the feedback to the guesser.
   2. **Feedback to the guesser** is to numbers \(as shown in each row of the game in the image above\):
      1. How many colors are in the correct positions? \( The goal is to have all four correct.\)
      2. How many correct colors are in incorrect positions?

  
2. Play a game of Mastermind with your partner on paper.

   1. **Mastermind Rules**

      1. **Each player should write down a sequence of four colors **without letting your partner see it.

         1. For convenience, you can use the first letter of each color name to represent that color: **r**ed, **o**range, **y**ellow, **g**reen, **b**lue, **v**iolet. \(For now, don't use the same color more than once, though people also play that way.\)

      2. **Take turns guessing your partner's colors**. When your partner makes a guess, give two numbers as feedback as described above.

         1. For example, if your secret colors are **royg **and your partner guesses **goby **you reply "one and two," because one color \(orange\) is in the correct position, and two colors \(yellow and green\) are in the secret sequence but not in the correct positions.

      3. **Use the information you have from earlier guesses **to make the best guesses you can.

         1. For example, after **goby **in the example above, you might think, "One of my colors is in the correct position, and two other colors are correct. I'm going to guess that green is in the correct position, and orange and blue are somewhere in the list. So a good next guess would be **grob **because that has green in the same place as before, and orange and blue moved over." Your partner will reply "zero and three," which sounds like negative progress because now none are in the correct place, but it isn't because now you know for sure that green wasn't the correct-position color, so on your next guess you might try orange in the second position, and so on.

3. You'll build the Mastermind program in stages over the course of the year. Now your goal is to support two human players using the computer as a notepad to record guesses and feedback:

   1. Find out the two players' names so you can use them to keep track of whose turn it is.
   2. Ask one player to make a guess \(using four letters like **goby **above\).![](http://bjc.edc.org/bjc-r/img/2-complexity/mm1.png "first guess interaction")

   3. Display that guess on the screen. ![](http://bjc.edc.org/bjc-r/img/2-complexity/mm2.png "four colors displayed")

   4. Ask the other player for feedback, as two numbers. ![](http://bjc.edc.org/bjc-r/img/2-complexity/mm3.png "asking interaction")![](http://bjc.edc.org/bjc-r/img/2-complexity/mm4.png "four colors 2 points")

   5. Keep doing that until the guesser gets the correct answer. 

      1. You'll find it useful for a script to be able to tell a particular sprite what to do. There's a tool to do that: the

         ![](http://bjc.edc.org/bjc-r/img/1-introduction/tell.png "tell \(sprite\) to \(action\)")block.

         For example: ![](http://bjc.edc.org/bjc-r/img/1-introduction/tell-alonzo.png "tell \(Alonzo\) to \(say ...\)") ![](http://bjc.edc.org/bjc-r/img/1-introduction/tell-correct.png "tell \(correct position\) to \(show value \(\# correct\)\)")

4. Save this as "U2-Mastermind"

### Take It Further

1. Instead of asking the guesser to type in four letters, you could have six color buttons that the guesser could click in order. To do this, make six more sprites, each with a color, and put them off on the side of the stage so they won't be confused with the recorded guesses. You should also have an "erase" sprite with this character as its costume: ⌫ and an "okay" sprite, maybe with a check mark: ✓. Make sure that these buttons update the display appropriately.
2. Let both players have secret color sequences, and take turns guessing each other's list. You'll have to add a second column of guesses toward the right side of the stage, and a second set of sprites. The game ends when either player guesses correctly.



