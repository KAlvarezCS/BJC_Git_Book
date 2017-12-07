# Build Your Own Clock

**In this project, **you will model a clock that displays the current time. Your code will make the second hand, minute hand and hour hand rotate properly and keep track of time. ![](http://bjc.edc.org/bjc-r/img/1-introduction/Clock_img/ClockAnimation.gif "Clock animation")

#### For You To Do

1. To build a clock, you will need to figure out how many degrees the second hand must turn every second. How should the minute hand rotate every minute? From one hour to the next, how many degrees must the hour hand rotate?
2. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/1-introduction/U1L5-build-your-own-clock-student.xml) This starter file gives you three sprites with costumes for the second, minute and hour hands. The red second hand also contains a sound file for “clock ticking”. You may find these blocks useful while writing the code for the second hand. ![](http://bjc.edc.org/bjc-r/img/1-introduction/Clock_img/goToFrontBlock.png "go to front block") ![](http://bjc.edc.org/bjc-r/img/1-introduction/Clock_img/playTickBlock.png "play sound Tick block") Time sensors in Sensing Menu will report the actual current time. For example when the current time is **10:45:20 **these blocks will report:![](http://bjc.edc.org/bjc-r/img/1-introduction/Clock_img/currentHour.png "current hour")![](http://bjc.edc.org/bjc-r/img/1-introduction/Clock_img/currentMin.png "current minute")![](http://bjc.edc.org/bjc-r/img/1-introduction/Clock_img/currentSec.png "current second")
3. Try, on your own, to write code for each sprite, telling it where to point at the current time. Look at the [hints](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/optional-projects/2b-clock-hints.html) only if you are really stuck.

#### Take It Further

1. On most clocks with hands, the hour hand moves continuously rather than jumping all at once at each new hour? For example, the hour hand points between 12 and 1 when the time is **12:26:36**. If your hour hand jumps from hour to hour, adjust your code to implement this more realistic movement. ![](http://bjc.edc.org/bjc-r/img/1-introduction/Clock_img/hourHandinbetween.png "Clock hands at 12:26:36")

2. Choose or draw costumes for the hands and clock to build a designer’s clock/watch in your own style. You can draw images, or find them on the web and use an image editing software such as Adobe Photoshop to edit and properly orient them. You will need to anchor the costumes properly by setting the rotation center at the appropriate point. ![](http://bjc.edc.org/bjc-r/img/1-introduction/Clock_img/rotationcenter.png "Sprite rotation center assigned")

3. Create an alarm clock that takes some input from the user and beeps or rings when the time is up. To store the user input, you will need to learn how to make a variable using the Variables menu. ![](http://bjc.edc.org/bjc-r/img/1-introduction/Clock_img/alarmHourVariable.png "Make variable alarm Hour")

4. Build a “Grandfather Clock” with a swinging pendulum in its mechanism. Or a “Cuckoo Clock” that has an animated bird that shows up at regular intervals.



