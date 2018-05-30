# Binary Representation

We've looked at how the number of bits used to represent an integer affects how big it can be. Now we turn to the specific way a single-word integer is encoded as bits.

The word "bit" is an abbreviation for binary digit. 

People generally use base ten \(decimal\) digits to write numbers. Computers, because of the digital abstraction, use base two \(binary\).

In **base 10**, there are ten digits \(0-9\), and each place is worth ten times as much as the place to its right.

![](https://bjc.edc.org/bjc-r/img/4-internet/decimal-places.jpg "place values in decimal")

In **binary, base 2,** there are two digits \(0 and 1\), and each place is worth two times the place to its right. 

![](https://bjc.edc.org/bjc-r/img/4-internet/binary-places.jpg "place values in binary")

The subscript 2 on 1101\_2 means the 1101 is in base 2. Numbers are normally written in base 10, so a subscript 10 is only used when needed for clarity.

#### For You To Do

1. ![](https://bjc.edc.org/bjc-r/img/icons/talk-with-your-partner.png "Talk with Your Partner")Watch this Binary Timer Snap_! _program run. Write a description of the binary counter's behavior. Explain what you see going on.![](https://bjc.edc.org/bjc-r/img/4-internet/bin-timer-preview.gif)

### Reading Binary

In **base 10 **notation, each place value represents a **power of ten**: the units place \(10^0= 1\), the tens place \(10^1= 10\), the hundreds place \(10^2= 100\), the thousands place \(10^3= 1000\), etc. So, for example:

9827   =   9 × 10^3  +  8 × 10^2  +  2 × 10^1  +  7 × 10^0

**Base 2** uses the same idea but with **powers of two** instead of powers of ten. Binary place values represent the units place \(2^0 = 1\), the two place \(2^1 = 2\), the fours place \(2^2 = 4\), the eights place \(2^3 = 8\), the sixteens place \(2^4 = 16\), etc. So, for example:   
10010\_2   =   1 × 2^4	 +  0 × 2^3  +  0 × 2^2  +  1 × 2^1  +  0 × 2^0   =   16  +  2   =   1810

To translate from binary \(for example, 1011012\) to base 10, **first, write the number out on paper. Then write out the binary place values **by _doubling left from the units place_:

101101\_2 has only six digits, so we don't need powers of two to the left of that.

1	0	1	1	0	1

32	16	8	4	2	1

![](https://bjc.edc.org/bjc-r/img/8-recursive-reporters/r-to-l.png "right-to-left arrow")

This means that this number is, in base 10, 32 + 8 + 4 + 1 = 45. So, 101101_2 = 45\_10_

#### For You To Do

1. Translate these binary representations into base 10 notation:
   1. 101\_2
   2. 111\_2
   3. 1010011\_2
   4. 1000000000\_2

### Writing Binary

To translate from base 10 \(like 8910\) to base 2, **first write out the binary place values** by doubling left from the units place until you get to a value larger than your number \(128 for this example\). **Then think**, "I can take out a 64, so I write a 1 there, and there's 25 left \(89 − 64\). I have 0 thirty-twos, because I only have 25. But I can take out 16, and there's 9 left. So, 8 and 1 are the last nonzero bits.

Either way you are converting \(and between any bases\), always write the place values right-to-left \(just as with units, tens, hundreds, etc.\), and always write the number itself left-to-right.

89

25

9

1

0

![](https://bjc.edc.org/bjc-r/img/8-recursive-reporters/r-to-l.png "right-to-left arrow")

128	64	32	16	8	4	2	1

 	1	0	1	1	0	0	1

Now read the number off: 1011001_2 = 89\_10_

Here's a more precise description of this algorithm to find the base 2 representation of any positive integer:

* First, find the largest power of two that is less than the number.
* Then, subtract that power of 2 from the number, keep the new number, and record a 1 in the place for that power of 2.
* Then, determine if the next largest power of 2 that is less than the new number, and:
  * If it does, subtract that power of 2 from the number, keep the new number, and record a 1 in the place for that power of 2.
  * If it doesn't, keep the same number, and record a 0 for that power of 2.
  * Repeat this whole step with the next largest power of 2 until you have a bit \(1 or 0\) for all the remaining places down to and including the ones place \(by which point you should have nothing left of the original number\).

The string of ones and zeroes you have recorded is the binary representation of your original number.

#### For You To Do

1. Represent these base 10 representations in binary \(base 2\):
   1. 63
   2. 64
   3. 65
   4. 129
   5. 128
   6. 127



