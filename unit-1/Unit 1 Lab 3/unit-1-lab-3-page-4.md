# Modify Your Pinwheel

**On this page,** you will modify your existing pinwheel block so that you can use it to draw a variety of shapes.

![](http://bjc.edc.org/bjc-r/img/1-introduction/assorted-pinwheels.png "assortment of pinwheels")

### Adding Multiple Inputs

Recall how you first generalized your original pinwheel script: you added an input variable called branches that controlled the turning angle of the sprite. By adding more input variables, you can generalize other aspects of your program...

1. If it isn't already open, open your U1L3-Pinwheel project.

2. Experiment with the input for the _second _`move`block inside your `pinwheel`block as shown below.

   1. ![](/assets/talk_with_partner.png) First predict. What do you think will happen? ![](/assets/u1l3p4.png)
   2. Then try several inputs between -100 and 0.
   3. ![](/assets/twoPeopleThinking.png)What happened? How does it compare to what you predicted? How does this input value impact the sprite's behavior? How does it impact the resulting image on the sta![](http://bjc.edc.org/bjc-r/img/1-introduction/Blockswith-Inputs_img/asteriskpolygonCycleBW.gif)

3. Add a second input variable to control the amount of "backing up" that the sprite does before each turn through the full 360°.

   1. Edit your `pinwheel`block, then click the "+" sign at the end to add an input **label **\(**choose "Title text"**\). Type `backup:`as shown below, and click "OK".![](http://bjc.edc.org/bjc-r/img/1-introduction/create-input-name.jpg)

   2. Then click the "+" sign at the end \_again \_to add an input **variable **\(**choose "Input name"\)**, and call it backup.

   3. Drag off the new backup variable, place it where it belongs in the `pinwheel`code, and press "OK" or "Apply."

   4. Check that the new input slot in the `pinwheel`block behaves like the changes in your experimentation above.

4. Change the `pinwheel`script so that it will accept a positive value \(between 0 and 100\) for backup.

![](/assets/pair_programming.png)

1. Add a third input called size to control the input to the _first _`move`block. ![](http://bjc.edc.org/bjc-r/img/1-introduction/U1ImageVideoAddendum_img/U1L3-PinwheelwithInputs.png)

2. Try out a variety of inputs to your `pinwheel`program...

   1. ![](http://bjc.edc.org/bjc-r/img/1-introduction/U1ImageVideoAddendum_img/U1L3-PinwheelwithInputs1.png "setup; pinwheel, branches: \(6\) size: \(80\) backup: \(20\)")

      ![](http://bjc.edc.org/bjc-r/img/1-introduction/pinwheel-80-6-20-result.png "image of result pinwheel, branches: \(6\) size: \(80\) backup: \(20\)")

   2. ![](http://bjc.edc.org/bjc-r/img/1-introduction/U1ImageVideoAddendum_img/U1L3-PinwheelwithInputs2.png "setup; pinwheel, branches: \(5\) size: \(80\) backup: \(60\)")

      ![](http://bjc.edc.org/bjc-r/img/1-introduction/pinwheel-80-5-60-result.png "image of result of  pinwheel, branches: \(5\) size: \(80\) backup: \(60\)")

3. ![](/assets/talk_with_partner.png)Discuss what input values will give you a polygon or an asterisk.![](http://bjc.edc.org/bjc-r/img/1-introduction/polygon-result.png "polygon")![](http://bjc.edc.org/bjc-r/img/1-introduction/asterisk-result.png "asterisk")You may want to reduce the input value for the `wait `blocks inside the `pinwheel `script so you don't have to wait so long between trials.

![](/assets/save.png)

#### If There Is Time...

1. Find inputs to pinwheel that make the result look like a circle

##### Take It Further

Make a picture that looks more like a real pinwheel:

  


![](http://bjc.edc.org/bjc-r/img/1-introduction/pinwheel.png "pinwheel photo")

  


Copyright 2010 [Victoria Hudgins](http://asubtlerevelry.com/a-pinwheel-tutorial-the-easiest-ever/). Used by permission.

\(Save your project first; you'll need the`pinwheel`block you already have later.\)

It doesn't have to look exactly like the photo. But each arm of a pinwheel is essentially two triangles. You may find the![](http://bjc.edc.org/bjc-r/img/1-introduction/fill.png "fill block")block helpful.



