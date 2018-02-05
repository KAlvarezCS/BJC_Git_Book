# Remembering the Moves

**In this lab**, you will continue[the Tic-Tac-Toe project](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/4-abstraction/4-building-tic-tac-toe.html)from Unit 2 to allow the program to_analyze_the game board to detect wins and ties.

**On this page**, you'll prepare for the analysis by giving the program a global memory of what moves have been made.

#### For You To Do

1. Open your project **U2L4-TicTacToe** and save it as **U3L2-TicTacToe.** That preserve the old version while you modify it here.
2. It was easy to detect illegal moves \(a move in a square that's already occupied\) because each sprite could test that without knowing anything about the board as a whole. But for the analysis in this lab, you need a _global _picture of the state of the game. \(It's "global" not just in the sense of using a global variable, although that's true too, but rather that you need one single idea of the board, not nine local ideas about one square each.\)

   1. Make a global variable board and, when the game starts, set it to a list containing the word "Empty" nine times. ![](http://bjc.edc.org/bjc-r/img/2-complexity/TTT1_img/BoardInitialize.png "set \(board\) to {&apos;Empty&apos;, &apos;Empty&apos;, &apos;Empty&apos;, &apos;Empty&apos;, &apos;Empty&apos;, &apos;Empty&apos;, &apos;Empty&apos;, &apos;Empty&apos;, &apos;Empty&apos;}")  
      As the game progresses, you're going to record each move by modifying this list, so that its value always reflects the actual state of the visible board.

   2. Create **sprite-local variable** square number:  ![](http://bjc.edc.org/bjc-r/img/3-lists/square-number-var.png "variable name dialog box with &apos;for this sprite only&apos; selected") A

      **sprite-local variable **is like a global variable in that it doesn't belong to a particular _script, _but it does belong to a particular _sprite. _When the initial sprite is cloned nine times, each clone will have its own version of this variable. That's how a sprite will "know" which square it is on the board.

   3. As you create the clones, give each the correct square number:![](http://bjc.edc.org/bjc-r/img/2-complexity/TTT1_img/SquareNumbersonTTT.png "3 by 3 square grid with numbers 1 through 9") [Click here if you want a hint.](http://bjc.edc.org/bjc-r/cur/programming/3-lists/2-tic-tac-toe/1-find-ties.html?topic=nyc_bjc%2F3-lists.topic&course=bjc4nyc.html&novideo&noassignment#hint-1)

   4. When a square is clicked, replace that square's entry in the board list with X or O as appropriate.

3. ![](/assets/save_use_later.png)



