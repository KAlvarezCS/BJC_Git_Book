# The Game of Pong

**In this project, **you are going to model a computer game called Pong, first developed by Atari in 1972. You will write the code for the paddle which will allow it to move up and down based on user keyboard input and also write the code for the ball which will allow it to bounce every time it hits a wall or the paddle. ![](http://bjc.edc.org/bjc-r/img/1-introduction/Pong_img/pongAnimation.gif)

#### For You To Do

1. ![](http://bjc.edc.org/bjc-r/img/icons/talk-with-your-partner.png "Talk with Your Partner")

   Discuss with your partner the mathematics behind the ball bouncing off the paddle. How does the initial direction of the ball as it hits the paddle relate to the final direction of the ball as it bounces off the paddle? The following diagram may help.![](http://bjc.edc.org/bjc-r/img/1-introduction/Pong_img/Bounce.png "Initial and final directions of ball")

2. Create the paddle and the ball sprites and give them their costumes \(filled rectangle and circle\).
3. Write the code to have the paddle move up and down when the user presses the up arrow and down arrow keys. Don't let the paddle move beyond the edges of the stage.
4. Write the code to start the ball moving when green flag is clicked and to bounce off the stage edges and the paddle. Note that there is a built in block to bounce off the edges.

#### Take It Further

1. Add scoring to your game. Every time the paddles bounces off the ball, the player should earn a point and every time the ball hits the right wall, the player should lose a point. You can create a variable to keep track of the score. ![](http://bjc.edc.org/bjc-r/img/1-introduction/Pong_img/ScoreVariable.png "Make variable score")

2. Create a second paddle to allow the game to become multiplayer game. Adjust your code to accommodate keyboard input from two users. ![](http://bjc.edc.org/bjc-r/img/1-introduction/Pong_img/TwoPlayer.png "Multi Player Pong")

3. Create a second paddle \(or use the one from part B if you did that\) and let this paddle be driven automatically by the computer for a "human versus computer" version of the game. Hint: You can automate the second paddle by using the following block from the Sensing menu: ![](http://bjc.edc.org/bjc-r/img/1-introduction/Pong_img/yPositionofBallSensing.png "y Position Sensing")



