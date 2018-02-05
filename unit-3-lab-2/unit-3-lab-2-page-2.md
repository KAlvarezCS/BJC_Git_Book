# Detecting Wins and Ties

**On this page**, you'll teach the program to detect and report wins and ties.

#### For You To Do

1. Open our project **U3L2-TicTacToe** if it isn't open already.
2. Each winning combination is a list of three tile numbers \(a _triple_\). For example, this winning combination:![](http://bjc.edc.org/bjc-r/img/3-lists/win456.png "horizontal win in the second row")is represented as ![](http://bjc.edc.org/bjc-r/img/3-lists/list456.png "\(list 4 5 6\)") in the program.

   1. How many winning combinations are there?
   2. Which triples are winning combinations?
   3. Create a reporter that outputs a list of all possible winning triples. It will look something like this: ![](http://bjc.edc.org/bjc-r/img/3-lists/TicTacToe-wins.png "TicTacToe wins partial block definition")

3. Find out if a winning triple has actually happened:

   1. Click ![](http://bjc.edc.org/bjc-r/img/1-introduction/green-flag_button.png "green flag button") to clear your tic-tac-toe board and initialize board. Play _one _game, _deliberately letting _**x **_win_.

   2. Try this: ![](http://bjc.edc.org/bjc-r/img/3-lists/map-item-board.png "map \(item \( \) of \(board\)\) over \(list 1 2 3\)")

      1. **Note **that the first input to `item `is empty.

   3. What does the result of the above tell you about the state of the game?
   4. If `{1, 2, 3} `isn't the triple in which **x **won the game, try part \(b\) again for that winning triple.

4. Make a block ![](http://bjc.edc.org/bjc-r/img/3-lists/status-of-triple.png "status of triple \( \)") that takes a list like `{1, 2, 3} `as input and reports a list of which of those squares are occupied by whom.

5. Use `map `and `TicTacToe wins `to make a block that reports the status of _all possible _winning triples, as a list of lists.

6. Make a block ![](http://bjc.edc.org/bjc-r/img/3-lists/wonQ.png "won? \( \)") that takes the letter **X **or **O **as input,  and reports `True `if and only if that player has won the game.

7. Modify your program so that when a layer wins the game, the program _notifies_ the players.

8. The definition of a tie game is that there are no more empty squares, and neither player has won. Declare a tie \(switch the sprite's costume to Turtle and have it `say `"TIE GAME!"\) when there are no empty squares after a move. Be sure to make this test _after _the test for a win.

   1. [Click here if you want a hint.](http://bjc.edc.org/bjc-r/cur/programming/3-lists/2-tic-tac-toe/2-find-wins.html?topic=nyc_bjc%2F3-lists.topic&course=bjc4nyc.html&novideo&noassignment#hint-target)

9. Why does it matter about the order of the tests? ![](/assets/twoPeopleThinking.png)

10. ![](/assets/save_use_later.png)'

#### If There Is Time...

1. There are many small improvements you could make. For one thing, when a player wins, you might want to prevent any further moves. What else might you want to change or improve?

#### Take It Further

1. Your program can be smarter about detecting ties. If there is only one empty square on the board, and filling that square with the player whose turn is next wouldn't cause a win, then the game is already tied. The challenge here is that you'll have to test for a win on a board that isn't the current board.

2. Instead of just having the sprite say something like "X wins," it'd be more satisfying to the players if you draw a thick line through the three squares that generate a win. This is a little tricky because by the time you know there's a win, you no longer know which triple triggered it. Try not to uglify your existing code while solving this problem.



