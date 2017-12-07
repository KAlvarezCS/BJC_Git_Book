# Sprite Following a Sprite

**On this page, **you will change the script so that the sprites don't move forever, but only `repeat until `they touch.

#### For You To Do

1. Change Sprite\(2\)'s code to point towards Sprite only until it is touching Sprite. \(The following instructions and animation show how.\)

   1. Select Sprite\(2\) by clicking its button below the stage.
   2. Replace the `forever `block with  a `repeat  until `block.
   3. Drag ![](http://bjc.edc.org/bjc-r/img/blocks/touching.png "touching sprite") into the hexagonal space in the `repeat until `block. Set it to repeat until it is touching Sprite.![](http://bjc.edc.org/bjc-r/img/1-introduction/replacing-code.gif)

2. Do the same for Sprite. Change its code to follow your mouse only until it is `touching `Sprite\(2\).

3. Test your program to see if it does what you want:

   * When you click ![](http://bjc.edc.org/bjc-r/img/1-introduction/green-flag_button.png "green-flag button") , Sprite \(the gray one\) should follow your mouse and Sprite\(2\) should keep turning to face Sprite.
   * If you bring Sprite close enough to touch Sprite\(2\), both sprites should stop moving.

4. So far, Sprite\(2\) points toward Sprite, but doesn't move toward it. Add a line of code to Sprite\(2\)'s script so that it chases Sprite. Here's the idea: ![](http://bjc.edc.org/bjc-r/img/1-introduction/move-tiny.png)

5. Test your program a few times.![](/assets/pair_programming.png)

6. Right now, when the sprites meet, they just stop. Make them have a conversation when they stop. You can do that by adding code like this to Sprite\(2\)'s script. Make up your own conversation. You can use any language you can type.Sprite\(2\) does things itself. It also tells Sprite what to do and when to do it. This code puts Sprite\(2\) in charge of Sprite.![](http://bjc.edc.org/bjc-r/img/icons/import-tools.png "Import Tools")

   In the current version of Snap, the `tell `block isn't installed automatically. Click on the File![](http://bjc.edc.org/bjc-r/img/sys/button-file-menu.png "File menu icon") menu at the top of the Snap window and select "Import Tools." The `tell `block will appear toward the end of the Control palette. You'll need to import tools once into each new Snap project where you need `tell`. ![](http://bjc.edc.org/bjc-r/img/1-introduction/simpledialogue-going-to-lunch.png)To prevent the two sprites from being stuck to each other unable to move, the sprites will need some space between them and some time apart before the chase starts. Blocks such as these may help.  ![](http://bjc.edc.org/bjc-r/img/1-introduction/U1ImageVideoAddendum_img/U1L5p2-PuppySeparation.png "Blocks for delaying chase")![](/assets/save.png)

#### If There Is Time...

1. Give the sprites costumes.

   1. You can use a picture from the Internet by dragging the picture into the costume area for that sprite.

2. Change the background on the stage. ![](http://bjc.edc.org/bjc-r/img/1-introduction/U1ImageVideoAddendum_img/U1L2-GossipBackground.gif)



