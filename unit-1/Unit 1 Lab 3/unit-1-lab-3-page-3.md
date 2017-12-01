# Block With Inputs

![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/branchesCycle.gif)

**On this page,** you will create many different pictures \(like the ones above\) by creating a single block with an _Input slot: _![](http://bjc.edc.org/bjc-r/img/1-introduction/pinwheel-block.png "pinwheel-block").Input slots allow one block to do many related jobs.

##### For You To Do

1. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/1-introduction/U1L3-Pinwheel.xml)

Make 5 copies of the script and modify those copies so that they make pinwheel designs like these with 3, 4, 5, 6, and 12 branches.

![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/3.png "pinwheel with 3 branches")![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/4.png "pinwheel with 4 branches")![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/5.png "pinwheel with 5 branches")![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/6.png "pinwheel with 6 branches")![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/12.png "pinwheel with 12 branches")

The scripts are essentially all the same; only the \_input values \_change. Instead of having many separate scripts, you can make one more general script that will draw all such designs .Your `pinwheel`block will need an input to specify how many branches you want, ![](http://bjc.edc.org/bjc-r/img/1-introduction/pinwheel-block.png "pinwheel-block")just as the `go to`block has inputs to specify x and y values![](http://bjc.edc.org/bjc-r/img/1-introduction/go-to-empty-inputs.png "go-to-empty-inputs").

![](/assets/pair_programming.png)

1. Create a `pinwheel`block with an input for the number of branches. Instructions below and in the video below right.

#### **Making an Block with an Input**

1. **Type the block name and the label for your variable**  
   in the "Make a block" dialog box, and click OK. For this project, type  
   `pinwheel, branches:`

   [Click here](https://youtu.be/SG6DlrtjEwI?rel=0) to watch a **VIDEO **of these steps. \(If your connection blocks YouTube,[ watch the video here](http://scratch.mit.edu/discuss/youtube/SG6DlrtjEwI).\)

   [![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/YouTubeVideoIcon.png "video of Making an Block with an Input")](https://youtu.be/SG6DlrtjEwI?rel=0)  
   ![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/category.png "Make a block")

   * This block is about \_moving \_your sprite, so you might choose the blue Motion palette. Or just leave it gray.
   * Using a comma and a colon are not requirements; they are here to help with clarity.

2. **Click the + \(plus sign\) after the variable label, type the name of the input**, and click OK to add the variable input slot. For  
   `pinwheel`, click the + after "branches:" and type number of branches as the name of your input variable.

   ![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/plusSign.png "Plus sign")  
   ![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/inputName.png "Creat input name")

3. **Drag in the blocks you need, and use the new input.**

   * Here, drag one of your pinwheel scripts into the Block Editor and snap it to the `pinwheel`block.
   * We use the word "input" for two different but related things:

   * 1. The input name, such as number of branches , which is set in the block definition. This is called a **parameter **\(or formal parameter\).
     2. The input _value, such as 6 for a hexagonal pinwheel, which is given each time the block is used. This is called an argument _\(or actual argument\).
   * The AP CSP framework uses the word "parameter" for both.

   * Then, drag the new input number of branches in to replace the values that change to allow for more general use of the script.

   ![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/blockwith21.png "pinwheel code before replacement")  
   ![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/numberofbranches.png "pinwheel code after replacement")

4. Save your work as U1L3-Pinwheel.

![](/assets/save.png)

#### Take It Further

1. These images were created with the `pinwheel`block  and `set pen color`. Create your own art.
   ![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/Wreath3.png "wreath of rainbow colored pinwheels")
   ![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/Wreath1.png "wreath of rainbow colored pinwheels")
   ![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/Wreath2.png "wreath of rainbow colored pinwheels")
2. Make the animation at the top of this page.



