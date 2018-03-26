# Building a Tic-Tac-Toe Board

![](http://bjc.edc.org/bjc-r/img/2-complexity/TTT1_img/Three States of TTT.png "Three states of Tic Tac Toe: in progress, win, tie")

**In this **_**year long **_**project,**you will develop a program that plays Tic-Tac-Toe as well as you do.

**On this first page,**you display a Tic-Tac-Toe board and let two human players enter moves.

One approach to this problem uses multiple sprites to make an "active" Tic-Tac-Toe board, in which each square is actually a separate sprite. Each sprite knows which square it's in, because once the board is set up, the sprites never move. You click in a square, and the sprite that you clicked on changes its costume to display the move. It doesn't have to compute the square number based on the mouse coordinates.

#### For You To Do

1. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/2-complexity/U2L4-Tic-Tac-Toe.xml)
2. A sprite has already been created for you with three costumes: Empty, X, and O. Click on the `next costume `block at the top of the scripting area a few times to see all of them.![](http://bjc.edc.org/bjc-r/img/2-complexity/TTT1_img/Costumes.png "Costumes of a square: Empty, X and O")

3. You will be using the **clone** feature in Snap.

   1. Why "under control of your program"? It's possible to make a copy of a sprite by hand; right-click on the sprite's icon in the sprite corral and choose "Duplicate." That's useful if you only want one copy, but in this project you're going to need nine copies, one for each square of the Tic-Tac-Toe board. So you'd like to say something along the lines of ![](http://bjc.edc.org/bjc-r/img/2-complexity/9-copies.png "repeat 9 \[create a clone of myself\]")

      The actual code in the project will be slightly more than this, but this is the central idea.

   2. A clone is a complete copy of the sprite you say to copy. It has the same position, costumes, scripts, and so on. But...

      1. The clone doesn't appear in the sprite corral.

      2. Once you've made the clone, any changes you make _ later _ to the original sprite \(such as adding or modifying a script\) is _not_ copied to the clone.

      3. Clones are temporary. Clicking  the stop button will delete all clones in the project.

   3. So the ideas is that you write your program completely, then make whatever clones you need.

4. In the starter project is this demonstration script: ![](http://bjc.edc.org/bjc-r/img/2-complexity/TTT1_img/WhenIamClicked.png "when I am clicked, create a clone of myself, glide \(1\) secs to x: \(random...\) y: \(random...\)")You're going to use this script \_right now \_to learn more about clones, but it isn't going to be part of \_the finished project. **Read **\_the script together with your partner and talk over what you think will happen when you click on the sprite. Then click on the sprite on the stage and compare what happens with what you expected.

   1. Notice that is the clicked sprite that moves to a new random position after cloning itself. \(You can tell because it's the one that says "You clicked me."\)

   2. Note that both copies are _active_ sprites. Both are clickable \(try it\) and draggable \(try that too\).

   3. The `create a clone `block takes an input because it can copy any sprite, but in this project there's only one "starter" sprite, so you can use `myself `or  `Square `as the input.

The next script in the starter project is this:

![](http://bjc.edc.org/bjc-r/img/2-complexity/TTT1_img/delete-clone.png "when flag clicked, delete this clone")

The block is called `delete this clone `rather than `delete this sprite `because it works only for clones. So when you click the green flag, the original sprite and all its clones will run the script, but only the clones will be deleted. There will then be one sprite left on the stage. \(Clicking the stop sign automatically deletes clones, but this script is insurance in case you run the program and then run it again without clicking stop first.\)

#### For You To Do

1. Delete the `when I am clicked `script from problem 3. It was just for demonstration, and shouldn't be in the actual project. \(You'll make your own different one soon.\) Also, at the bottom of the scripting area, there's an additional `when`⚑ `clicked `block near, but separate from, the script just below it. They're separated because this script isn't part of the demonstration in problem 2, but it is part of the Tic-Tac-Toe game, so click the two pieces together now.

   1. Read that script and notice:

      1. The `wait `block is needed to ensure that the _other _`when`⚑ `clicked `script has time to delete old clones before we make new ones.

      2. `makeBoard `is an empty script. You're going to write it in the next problem.

      3. The variable X's turn? will be `true `when it's X's turn to play, or `false `when it's O's turn. When alternating between two values, it's convenient to use `true `and `false `because you can use ![](http://bjc.edc.org/bjc-r/img/2-complexity/TTT1_img/setXsturn.png "set X&apos;s turn? to \(not X&apos;s turn?\)") to switch between them, and just ![](http://bjc.edc.org/bjc-r/img/2-complexity/if-x-turn.png "if \(x&apos;s turn?\) ...") to test the variable.

2. Edit the block `makeBoard `to set up nine clones in three rows of three: ![](http://bjc.edc.org/bjc-r/img/2-complexity/TTT1_img/Row1.png "One row of squares")

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/TTT1_img/Row2.png "Two rows of squares")

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/TTT1_img/Row3.png "Three rows of squares")

   1. Hint: ![](http://bjc.edc.org/bjc-r/img/2-complexity/TTT1_img/for-row-column.png "for row = 1 to 3, for column = 1 to 3")

   2. The costumes are all 50 steps tall and wide.

   3. make sure the clones start out with the empty square costume.

   4. Be sure to

      `show `the original sprite before cloning it, so that the clones will be visible. After cloning nine times to create the board, `hide `the original sprite so it does not interfere with the game as a tenth square.

3. Now write a `when I am clicked `script that will allow each clone to put on the proper costume when clicked: X or O depending on whose turn it is. Also decide how a square should behave when it is clicked while already wearing an X or O costume.

4. ![](/assets/save_use_later.png)

This project hints at two important modern ideas in computer science. One is **object oriented programming**: Instead of a single sequence of instructions, the program has several\_independent\_objects \(also called "agents" or "actors"\), each of which has its own behavior. In this project, you can only click on one sprite at a time, and it then carries out a very quick task \(changing costume\) before you click another sprite. But a more complicated program might have one sprite send a\_message\_to another sprite, which would respond with its own behavior, while the first sprite continues with its own script.

The other idea is **parallelism **or **distributed computing**. Your project is running on a single computer, and the apparent ability of sprites to run simultaneously is an illusion provided by Snap_!_, which runs one script for a little while, then switches to a different script, and so on, then updates the display, then continues the first script. But you \_could \_have nine separate computers, one for each sprite. That would be overkill for this small project, but large web servers such as Google or Twitter have many thousands of computers all cooperating to handle the large amounts of data they require.

