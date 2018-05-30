# Representing Whole Numbers

**On this page,** you'll learn how computers store integers.

As you know, numbers show up everywhere in computer algorithms—even if numbers aren't the topic. For example, the user may be interested in a picture, but that picture is an abstraction over numbers. Numbers are also used to find a specific item in a list. Over the next several pages, you'll look more closely at numbers inside the computer.

#### For You To Do

1. The factorial of a positive integer n \(written "n!"\) is the product of all the integers from 1 to n. For example:    5!=1×2×3×4×5=120'
   1. [Click here to load. Save to your Snap! account](http://snap.berkeley.edu/snapsource/snap.html#open:https://bjc.edc.org/bjc-r/prog/6-computers/U6L2-BigNumbers.xml). Try out these inputs:
      1. ![](https://bjc.edc.org/bjc-r/img/4-internet/bang5.png "\(5\)! reporting 120")
      2. ![](https://bjc.edc.org/bjc-r/img/4-internet/bang10.png "\(10\)! reporting 3628800")
      3. ![](https://bjc.edc.org/bjc-r/img/4-internet/bang20.png "\(20\)! reporting 2432902008176640000")
      4. ![](https://bjc.edc.org/bjc-r/img/4-internet/bang30.png "\(30\)! reporting 2.6525285981219103e+32")

The "e+" means "times ten to the power of" so this notation means 2.6525285981219103 × 1032 = 265,252,859,812,191,030,000,000,000,000,000.

### Fixed Width Computer Hardware

So why did Snap! display 20! in ordinary whole number representation but 30! in scientific notation? Every computer model is designed with a certain **width**, the number of bits that the processor reads from memory or writes into memory at a time. That number of bits is called a **word**. As of 2016, most new computers are 64 bits wide. The first microcomputer, sold in 1971, was four bits wide!

##### Vocabulary

**width: **the number of bits that a CPU processes at a time

**word:** a binary sequences of that many bits

If you got an answer in scientific notation for 20!, you're using a 32-bit computer.

A 64-bit word represents 2^64 different values. We use half for negative numbers, one for zero, and the rest for positives. Half of 2^64 \(which is 2^63 = 9,223,372,036,854,775,808\) is about 9 × 10^18. That means that the 19 digits of 20! just barely fit in a 64-bit word. But the 33 digits of 30! don't. So the computer hardware reports an overflow error, and Snap! computes an approximation.

Are processor widths always powers of two?

Processor widths don't have to be a power of two. Some old computers—the kind you see in old movies that filled a large room—used 12-bit, 36-bit, and 60-bit words. But modern personal computers started at 8 bits and the widths have been doubling with each new generation.

#### For You To Do

1. Experiment in Snap!. What's the first integer whose factorial doesn't fit in a word?

### Bignums

Why can't programming languages just use more than one word to represent an integer? They can. It's just that a single machine language instruction can only add one-word numbers. A programming language must work a little harder to make addition work with multiple-word values. Not all languages do this, but the highest-level languages do.

#### Take It Further

A great example of a high-level programming language is Scheme. You can learn it from the free, online book [Structure and Interpretation of Computer Programs.](https://mitpress.mit.edu/sicp/full-text/book/book.html)

The design of a programming language isn't just a question of taste; it can be a matter of life and death. Between 1985 and 1987, a therapeutic X-ray machine killed four patients and seriously injured two more because of several bugs in its software; one of the bugs was that a counter that was kept in an eight-bit-wide variable would reach its maximum value of 127 and then overflow to zero instead of 128. When the variable was zero, an important safety check was not performed. This would not have happened if the software had been written in a better programming language.

#### For You To Do

1. Click on this block in the scripting area:    ![](https://bjc.edc.org/bjc-r/img/4-internet/bignums-true.png "USE BIGNUMS \(true\)")
   1. You can use bignums in any Snap! project by importing the "Infinite precision integers, exact rationals, complex" library. You learned to import libraries on the Libraries page.
2. Now try `30! `again. ![](https://bjc.edc.org/bjc-r/img/4-internet/bang30-bignum.png "30! reporting 265252859812191058636308480000000")

   1. This \(exactly correct\) value is different from the \(rounded off\) floating point value above. \(More about floating point in a moment.\)

3. Try `200!`. The reported result won't fit on your screen, but you can see it this way:

   1. Hold down the control key; while holding it down, also hold down the shift key \(it has to be in that order\), and then click the![](https://bjc.edc.org/bjc-r/img/6-computers/factorial.png "\(\) !") block.

   2. In the menu that appears, click on the red "script pic with result..." item. \(If a completely different menu appears, just click once outside of that menu.\)

   3. An image will download onto your computer or open in a new tab. You should be able to zoom in on it to read the digits.

4. How many digits are there in` 200!`? \(Don't count by hand; you have a computer.\)



