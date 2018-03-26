# Sprite Following the Mouse

**In this lab, **you will program two sprites. One sprite will follow your mouse. The other sprite will chase the first. When they meet, they will have a short conversation

.![](http://bjc.edc.org/bjc-r/img/1-introduction/U1ImageVideoAddendum_img/U1L5-PuppyChase.gif)

**On this page, **you will program the first sprite to follow your mouse and program the second sprite to point in the direction of the first sprite in preparation for following it.

#### For You To Do

1. Start a new project. Save it as "U1L5-SpriteChase"
2. Read and think about this script before you build it. What do you expect it to do? ![](/assets/talk_with_partner.png)![](http://bjc.edc.org/bjc-r/img/1-introduction/follow-that-mouse.png "Follow That Mouse Script")![](http://bjc.edc.org/bjc-r/img/blocks/mouse-x.png "Mouse X Reporter") and ![](http://bjc.edc.org/bjc-r/img/blocks/mouse-y.png "Mouse Y Reporter") report the mouse's location on the stage. They are in the Sensing palette.
3. Now build the script and run it. Move your mouse around the stage while the program is running.

   1. The block at the top of the script is called a **hat **block. Its shape emphasizes that it can be used only at the \_beginning of a script. Hat blocks don't say what the script should do; they say when it should do it. Hat blocks say what **event **should start the script running. In this case, the script starts when the green flag button is clicked. To stop this script, click the red stop sign:![](http://bjc.edc.org/bjc-r/img/1-introduction/stop_button.png "stop button")

4. ![](/assets/twoPeopleThinking.png)Does the program work the way you expected?

5. Create a second sprite by clicking on the ![](http://bjc.edc.org/bjc-r/img/1-introduction/add-a-new-turtle-sprite.png "add a new turtle sprite") button just below the stage. Then use the `point towards `block to make it point towards Sprite. The animation below shows how.![](http://bjc.edc.org/bjc-r/img/1-introduction/newsprite-pointing-to-old-sprite-part1.gif)The new sprite, named Sprite\(2\), appears on the stage. It's brand new, so it has no scripts. The buttons beneath the stage let you select the sprite you want to program.

![](/assets/pair_programming.png)

1. Change your script for Sprite\(2\) so that once the green flag is clicked, Sprite\(2\) will point towards Sprite `forever`. ![](http://bjc.edc.org/bjc-r/img/1-introduction/newsprite-pointing-to-old-sprite-part2.gif)While a script is running, its border lights up. If the running time is short, you may not notice the brief flash.

2. Click ![](http://bjc.edc.org/bjc-r/img/1-introduction/green-flag_button.png "green-flag button") and check that your script does what you intended:

   * Sprite always follows your mouse when you move your mouse around.
   * Sprite\(2\) stays in one place, but always points toward Sprite.

Both sprites' scripts use `When`![](http://bjc.edc.org/bjc-r/img/1-introduction/green-flag_button.png "green-flag button") `clicked`, so both scripts run when ![](http://bjc.edc.org/bjc-r/img/1-introduction/green-flag_button.png "green-flag button") is clicked.  
![](/assets/save.png)

