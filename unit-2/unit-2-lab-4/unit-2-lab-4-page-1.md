## Robot in a Maze

**In this project,**

you will program a robot to get through several mazes.

![](http://bjc.edc.org/bjc-r/img/2-complexity/Robot_img/RobotinaMazeTitle2.png "Robot in A Simple Maze")

Five mazes have been created for you. The code you write to escape each maze should be as_simple_,_concise_, and_elegant_as possible.

For example, this solution works for Maze 1:  
![](http://bjc.edc.org/bjc-r/img/2-complexity/Robot_img/1c_escapeMaze1Code1.png "escapeMaze1 code")![](http://bjc.edc.org/bjc-r/img/2-complexity/Robot_img/1b_Maze1Path.png "Maze 1 path")

But nesting one `repeat `block inside another makes the code more concise and, most programmers would agree, more elegant:

![](http://bjc.edc.org/bjc-r/img/2-complexity/Robot_img/1c_escapeMaze1Code2.png "escapeMaze1 code improved")

This works because once the Robot reaches the destination, we don’t care which direction it's facing.

#### For You To Do

1. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/2-complexity/U2L4-RobotMaze.xml) Examine both the `Robot `and the `Board `sprites. For each of the given mazes, write the _shortest _and _most elegant _code to help the robot escape. Use only these four custom Motion blocks \(along with whatever Control blocks you need\):![](http://bjc.edc.org/bjc-r/img/2-complexity/Robot_img/0_NewMotionBlocks.png "Motion blocks")![](http://bjc.edc.org/bjc-r/img/2-complexity/Robot_img/1b_Maze1Path.png "Maze 1 path")
   ![](http://bjc.edc.org/bjc-r/img/2-complexity/Robot_img/2b_Maze2Path.png "Maze 2 path")

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/Robot_img/3b_Maze3Path.png "Maze 3 path")

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/Robot_img/4b_Maze4Path.png "Maze 4 path")

   ![](http://bjc.edc.org/bjc-r/img/2-complexity/Robot_img/5b_Maze5Path.png "Maze 5 path")

2. **Analyze this code.** On graph paper, draw the maze this code was written for. Do not use Snap!.![](http://bjc.edc.org/bjc-r/img/2-complexity/Robot_img/EscapeCodeFindMaze1.png "Given the code draw the maze")

3. ![](/assets/talkpair.png)Share your drawing with other students, and discuss how you made it.

![](/assets/save.png)

#### Take It Further

1. Create your own maze and a robot escape code for that maze.
   1. **Analyze** the Draw Your Maze code in the Board sprite\(shown below\).
   2. **Experiment.** If you change some of the zeroes to ones, you can create a path for the robot to travel.
   3. The board matrix variable contains a **list of lists**. Each separate list of zeros and ones will correspond to a row of squares in the maze.

   4. Edit the board matrix to make a maze you like, then write the Escape Your Maze code for the robot. ![](http://bjc.edc.org/bjc-r/img/2-complexity/Robot_img/6_YourMazeCode.png "Draw Your Maze code")



