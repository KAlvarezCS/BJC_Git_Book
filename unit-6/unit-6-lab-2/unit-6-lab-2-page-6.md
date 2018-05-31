1. ---

   # Hexadecimal Representation

Typing long strings of ones and zeros is inconvenient and prone to error. A more efficient method is to use hexadecimal \(base 16\). One hex digit represents any whole number between 0 an 15. So eight digits of binary can be translated into two digits of hexadecimal, which is much easier and much less error-prone for humans.

Eight bits in base two...

| 2^7 | 2^6 | 2^5 | 2^4 | 2^3 | 2^2 | 2^1 | 2^0 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 128s place | 64s place | 32s palce | 16s place | eights place | fours place | twos place | ones place |

is two digits in base 16

| 16^1 | 16^0 |
| :--- | :--- |
| sixteens place | ones place |

For example 121_10 = 01111001\_2 = 79_\_16\_

| 0 | 1 | 1 | 1 | 1 | 0 | 0 | 1 |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |


| 7 | 9 |
| :--- | :--- |


In **base 16**, there are sixteen digits \(0-9 and A-F\), and each place is worth _sixteen _ times the place to its right. One hex digit has 16 possible values, the equivalent of four binary digits \(bits\). ![](https://bjc.edc.org/bjc-r/img/4-internet/hex-places.jpg "place values in hexadecimal")

This stands for 3 x 256 + 11 x 16 + 7 x 1 or 951

#### For You To Do

1. Watch this Hexadecimal and Binary Timer Snap! program run. The top row counts in binary, the middle in decimal, the bottom in hex. Write a description of the hex counter's behavior.
   ![](https://bjc.edc.org/bjc-r/img/icons/talk-with-your-partner.png "Talk with Your Partner")![](https://bjc.edc.org/bjc-r/img/4-internet/hex-timer-preview.gif)

### Reading Hexadecimal

**Base 16** uses **powers of sixteen **instead of powers of two or ten. Place values in hexadecimal represent the units place \(16\__0 = 1\), the sixteens place \(16\_1 = 16\), the two hundred fifty-sixes place \(16\_2 = 256\), the four thousand ninety-sixes place \(16_\_\_3 = 4096\), etc. So, for example:

3B16 = 3 x 16^1 + 11 x 16^0 = 48 + 11 = 59\_10

To translate from hexadecimal \(for example, 7B3\_16\) to base 10, **first, write the digits on paper. Then write out the hexadecimal place values:** start at the right with 1, then write 16 in the next place to the left, then write 256 \(which is 16^2\), and so on. Each new place will be worth 16 times the one to its right.

| 7 | B | 3 |
| :--- | :--- | :--- |
| 256 | 16 | 1 |
|  |  | ![](https://bjc.edc.org/bjc-r/img/8-recursive-reporters/r-to-l.png "right-to-left arrow") |

So, 7B3_16 = \(7 x 256\) + \(11 x 16\) + \(3 x 1\) = 1792 + 176 + 3 = 1971\_10_

Remember: A-F cover the digits after 9:

| 10 | 11 | 12 | 13 | 14 | 15 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| A | B | C | D | E | F |

#### For You To Do

1. Translate these hexadecimal numerals into base 10 notation:
   1. AF\_16
   2. 5D\_16
   3. 18\_16
   4. 3E8\_16

FF\_16

= \(15 × 161 + 15 × 160\)\_10

= \(15 × 16 + 15\)\_10

= 255\_10

A numeral such as 11 means eleven in the usual decimal notation, or three if it is a binary numeral, or seventeen in hexadecimal notation. The only way you know that the "18" in part \(c\) above doesn't mean eighteen is that subscript "16" means hexadecimal.

### Writing Hexadecimal

To translate from base 10 \(for example, 299\_10\) to base 16, **first write out the hexadecimal place values** by multiplying by 16 moving left from the units place until you get to a value larger than your number \(4096 for this example\). **Then think**, "My number is smaller than 4096, so I leave that place blank. But I can subtract two hundred fifty-six once, so I write a 1 there, and there's 43 left. Now, I can subtract two sixteens, and there's 11 left. And 11 is B in hex."

![](https://bjc.edc.org/bjc-r/img/8-recursive-reporters/r-to-l.png "right-to-left arrow")

| 4096 | 256 | 16 | 1 |
| :--- | :--- | :--- | :--- |
|  | 1 | 2 | B |

Now, read the number off: 12B\__16 = 299_\_10.

#### For You To Do

1. Translate these **decimal numerals** to **hexadecimal** notation:
   1. 59
   2. 144
   3. 229
   4. 316

Notice that the algorithms for converting between binary and decimal are the same as the algorithms for converting between hexadecimal and decimal. These algorithms can be used to convert to and from any base.

#### If There Is Time..

1. This algorithm runs into a problem after base 36. What's the problem and what's the solution?
2. Convert 229\_10 to base 7.

![](/assets/talk_with_partner.png)

