# Binary Timer Project

In this project you will create a timer that reports the number of seconds elapsed in both decimal binary notations.

#### For You To Do

1. First, review this Binary Timer, and then discuss what you know about this binary rotation.![](https://bjc.edc.org/bjc-r/img/4-internet/bin-timer-preview.gif)
   1. You can visit this [wikihow.com](http://www.wikihow.com/Convert-from-Decimal-to-Binary) page and discuss conversion from base 10 to base 2.

   2. Note that there are two methods presented in the link.

      1. The first method \(Short Division by Two with Remainder\), is more general and works for conversion to any base.

      2. The second method \(Descending Powers of Two and Subtraction\), is in tandem with a video you may have watched earlier.

      3. Choose one of the methods described and come up with a simple algorithm for this procedure.
2. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:https://bjc.edc.org/bjc-r/prog/6-computers/U6-BinaryTimer.xml)Several sprites, blocks, and costumes have already been created for you. The `Get Binary Digits `block \(in Timer\) is the only place where you will need to fill in some code.

If you look at the Timer sprite code, you will see that the `timer `block \(from the "Sensing" menu\) is used as a time keeper. The decimal and binary digits are computed and stored in lists, and then a broadcast is made to the sprites representing the digits to put on the appropriate costumes \(0 and 1 for the binary digits and 0 through 9 for the decimal digits.\)

![](https://bjc.edc.org/bjc-r/img/6-computers/BinaryClock_img/TimerCode.png "Timer Code")

The "warp" block is used to ensure that all the computation within the block is completed prior to the refreshing of the screen.The code for extracting the base 10 digits of a given number,`Get Decimal Digits`, is written for you. If you are using method 2 \(_Descending Powers of Two and Subtraction_\) to write `Get Binary Digits `you can ignore the code in `Get Decimal Digits`. If you are using method 1 \(_Short Division by Two with Remainder_\) however, you can use this code as a model to write the `Get Binary Digits `code as it is based on method 1.

#### For You To Do

1. Review and understand the code for the rest of the sprites representing the decimal digits. Check that your timer works in the decimal notation.
2. Now write the code for the `Get Binary Digits` custom block using either conversion method. If you get stuck, you can get some hints here. When you are done, review the code for the sprites representing the 8 binary digits. Check that the timer works in the binary notation.

#### If There Is Time...

1. In this project, you generated the binary number representation of decimal numbers 0 through 255. While it takes only 3 digits to represent the number 255 in base 10, it requires 8 digits to represent the same number in base 2. Can you explain why?   ![](/assets/talk_with_partner.png)
2. Create a Hexadecimal Timer Project in Snap!

#### Take It Further

1. Create a binary clock that shows the current time in base 2. For example:

Hr : Min : Sec

07 : 40 : 16

0111 : 101000 : 010000

You might want to make use of the `current `time block in the "Sensing" menu:![](https://bjc.edc.org/bjc-r/img/6-computers/BinaryClock_img/CurrentTime.png "current time")

1. Create a hexadecimal clock that shows current time in base 16. For example:

Hr : Min : Sec

12 : 40 : 59

C : 28 : 3B

1. Create a reporter in Snap! that converts a given number in a given base to its equivalent in another given base.
   1. ![](https://bjc.edc.org/bjc-r/img/6-computers/BinaryClock_img/BaseConverter.png)
2. Below you see a counter that simultaneously shows each number's representation in bases 2 through 16. Create a Snap! program that will model such a counter. 

![](https://bjc.edc.org/bjc-r/img/6-computers/BinaryClock_img/DG_MultibaseClock.gif)

