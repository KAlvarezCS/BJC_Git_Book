# Floating Point

**On this page, ** you'll learn how computers store numbers that are not integers.

The way computers store numbers that are not integers is called floating point.

Where did that funny name come from?

This non-obvious name is used because there used to be a fixed point non-integer notation with a fixed number of digits after the decimal point. For example, a fixed point notation with two digits after the decimal point was used to represent an amount of money in dollars and cents: $82.47. But today's computers always use floating point for non-integer values, including money.

Floating point allows computers to store very large numbers and also decimals, but the format still has a specific number of bits, and that limits the range of floating point values and mathematical operations just as with integers. However with floating point, values that exceed the limitation may result in round off errors instead.

#### For You To Do

1. For example, try ![](https://bjc.edc.org/bjc-r/img/4-internet/one-third.png "1 / 3") once with bignums on and once with bignum off.
   1. The decimal representation of 1/3 is 0.33333.. It has infinitely many digits, so the closest you can come in floating point isn't exactly 1/3; it gets cut off after a while because your computer doesn't have enough memory.
   2. Roundoff errors can result in some pretty non-intuitive results...
2. Try ![](https://bjc.edc.org/bjc-r/img/4-internet/0.2+0.4.png "\(0.2\) + \(0.4\)") and then try ![](https://bjc.edc.org/bjc-r/img/4-internet/7.6+8.7.png "\(7.6\) + \(8.7\)").

This isn't a bug in Snap_!_, which is correctly reporting the result computed by the floating point hardware.

How can such simple computations get wrong results?

These results seem surprising because a fractional value such as 0.2 can be represented exactly in decimal \(unlike the example of ⅓\). But in binary, only fractions whose denominator is a power of 2 can be represented exactly. So 2/16 can be represented exactly, but 2/10 can't. The binary floating point representation of 0.2 is just slightly too big, and so is the binary representation of 0.4. Adding two slightly-too-big values produces an error big enough to get to the next higher representable value.

No matter how good the hardware is, certain kinds of computations are likely to give severe errors in floating point. One simple example is subtracting two numbers that are almost equal in value. The correct answer will be near zero, and if it's near enough, it will underflow and an exact zero might be reported.

Floating point errors can be very expensive and can even kill people.

A notorious example is the fate of the Ariane rocket launched on June 4, 1996 \(European Space Agency 1996\). In the 37th second of flight, the inertial reference system attempted to convert a 64-bit floating-point number to a 16-bit number, but instead triggered an overflow error which was interpreted by the guidance system as flight data, causing the rocket to veer off course and be destroyed.

The Patriot missile defense system used during the Gulf War was also rendered ineffective due to roundoff error \(Skeel 1992, U.S. GAO 1992\). The system used an integer timing register which was incremented at intervals of 0.1 s. However, the integers were converted to decimal numbers by multiplying by the binary approximation of 0.1, 0.00011001100110011001100\_2 = 209715/2097152.

As a result, after 100 hours \(3.6 x 10^6 ticks\), an error of

$$(1/10 - 209715/2097152)(3600 * 100 * 10) = 5625/16384 ≈ 0.3433 seconds$$

had accumulated. This discrepancy caused the Patriot system to continuously recycle itself instead of targeting properly. As a result, an Iraqi Scud missile could not be targeted and was allowed to detonate on a barracks, killing 28 people.

From Analog and Digital Conversion, by Wikibooks contributors, [https://en.wikibooks.org/wiki/Analog\_and\_Digital\_Conversion/Fixed\_Wordlength\_Effects](https://en.wikibooks.org/wiki/Analog_and_Digital_Conversion/Fixed_Wordlength_Effects)

Computer arithmetic on integers is straightforward. Either you get an exactly correct integer result or, if the result won't fit in \(non-bignum\) integer representation, you get an overflow error and the result is, usually, converted to floating point representation \(as 30! was\).

By contrast, computer arithmetic on floating point numbers is hard to get exactly right. Prior to 1985, every model of computer had a slightly different floating point format, and all of them got wrong answers to certain problems. This situation was resolved by the IEEE 754 floating point standard, which is now used by every computer manufacturer and has been improved several times since it was created in 1985.

There are alternatives to floating point.

If the subtle errors in floating point computation turn out to be unacceptable in a particular application, software can use alternative representations:

* **Exact rationals.** Two bignums, one for the numerator and one for the denominator, can be used to represent any fractional value exactly.
* **Binary coded decimal**. A decimal digit can be represented in four bits, with a few four-bit combinations left over for a minus sign and a decimal point. A sequence of decimal digits of any length can be used to create decimal bignums, representing exactly any fractional value that takes a finite number of decimal digits. This would avoid the 02.+0.4 problem, but wouldn't work for problems involving 1/3.
* **Decimal floating point.** If the binary coded decimal notation is extended with a four-bit code for "times ten to the power," numbers in \(base 10\) scientific notation can be represented exactly.

With bignums turned off, when a result is too large to be an integer, it is converted to floating point.![](https://bjc.edc.org/bjc-r/img/4-internet/bang30.png "\(30\) ! reporting 2.6525285981219103e+32")



#### For You To Do

1. Try 200! again with bignums off. ![](https://bjc.edc.org/bjc-r/img/4-internet/200bang-fixnum.png "\(\(200\) !\) reporting infinity")

**What's going on?** Although 200! is very large, it's not "infinity." This report is caused by the size limitation of the floating point format. If the result of a computation is bigger than than the range of numbers that can be stored, then the computer returns a special code that languages print as Infinity or ∞.

In floating point, there are special codes for infinity, –infinity \(smaller than any finite value\), and "Not a Number," which is the notification used for illegal computations such as 0/0.![](https://bjc.edc.org/bjc-r/img/4-internet/zero-div-zero-reporting-NaN.png "\(0\) / \(0\) reporting NaN")

#### Take It Further

* Imagine a decimal floating point representation with one significant digit, and a range of exponents from 10^-2 to 10^2. The smallest positive number representable in this notation is 0.01 \(1×10^-2\) and the largest is 900 \(9×10^2\). Sketch a number line from 0 to 1000 and mark all of the positive values representable in this notation. What can you say about the spacing of values? How many fractional values are representable? How many integer values less than 1000 are not representable? What are the strengths and weaknesses of this choice of representable values? \(Real floating point has many more representable values, of course, but the way they're spaced on the number line is similar to this.\)

**How does a programming language know whether to interpret a bit sequence as an integer, a floating point, a text string of Unicode characters, an instruction, or something else?**

Programming languages differ in how they do this, but there's always some extra bit sequence that encodes the data type of any sequence of bits that tells the computer how to interpret it.

At the lowest level of software abstraction, everything in a computer is represented as a binary sequence. For example:

* A Boolean value is a single bit, 0 for `false `and 1 for `true`.
* A text string is a sequence of Unicode character codes, each of which is stored as a separate integer.
* Lists and blocks are binary sequences too.

But different languages use data types differently.

In well-designed languages \(those based on Scheme, for example\), that data type code is attached to the value itself. In other languages, when you make a variable, you have to say what type of value it will contain, and the data type is attached to the variable, so you can't both get exact answers when the values are integers and also be able to handle non-integer values of the same variable. So instead of seeing

![](https://bjc.edc.org/bjc-r/img/4-internet/varfoo.png "script variables \(foo\)")

you see thing like 

![](https://bjc.edc.org/bjc-r/img/4-internet/intfoo.png "integer \(foo\)")

We're telling you all these things because Snap! has strengths that many programming languages do not, and it's very likely that your next year's computer science class will use one of those other languages.

#### For You To Do

This question is similar to those you will see on the AP CSP exam.

1. A particular program uses 4 bits to represent whole numbers. When that program adds the numbers 9 and 7, the result is given as 0. Identify the best explanation of the result.
   1. Data was corrupted during the operation due to a technical glitch.
   2. The result was due to a round-off error.
   3. The result was due to an overflow error.
   4. A floating-point representation was used to approximate the result.



