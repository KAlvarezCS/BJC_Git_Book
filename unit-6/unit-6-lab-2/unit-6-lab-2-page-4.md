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

