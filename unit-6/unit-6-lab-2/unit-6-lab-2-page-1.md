# Bits

**In this lab, **you will explore how different kinds of information are represented in a computer.

**On this page, **you will learn about a central idea:_bits_, the basic units of data in computing.

As you know, information travels over wires inside the computer, and because of the digital abstraction, each wire is either on or off, with no intermediate states allowed. This small piece of information is called a **bit**, the smallest possible unit of information in the digital domain.

---

##### Vocabulary

A **bit **is a single unit of data that can only have one of two values. We usually represent the two values as 0 and 1.

---

What does the value of a bit mean? By convention, the two states of a bit are interpreted as 0 and 1, but that doesn't mean they have to represent numbers. A single bit can represent:

* False and True
* Off and On, simulating a light switch
* Red and Green, simulating a traffic light
* ...and many more

But what if the traffic light also needs a yellow value? It's tempting to say that, for example, 0 volts on the wire means red, 1 volt means yellow, and 2 volts means green. But then we would have all the problems of electrical noise that the digital abstraction was designed to avoid: a low or high input signal is interpreted as a clear on or off, but an in between value is too easily misinterpreted. \(See Unit 6, Lab 1: The Analog Domain: Transistors.\)

Instead, we use more than one bit if we need to represent more than two possible values. So, for the traffic light, we could use two bits: first bit

| first bit | second bit | meaning |
| :--- | :--- | :--- |
| 0  |  0 |  red |
| 0  |  1 |  yellow |
| 1  |  0 |  green |
| 1  |  1 |    \(unused\) |

There are four possible combinations of two bits, so with two bits we can represent up to four different values, even though we only need three for the traffic light.

#### For You To Do

1. Convince yourself that there aren't any more combinations of two bits.
2. Write down all the possible combinations of three bits. How many are there?
3. How many combinations of four bits are there?
   1. Each added bit doubles the number of values you can represent. This means that representing complex situations doesn't cost a lot of hardware; ten bits is enough to represent over 1000 distinct values.
4. How many values, exactly, can be represented by ten bits?
5. How many bits do you need to represent the days of the week?
6. How many bits do you need to represent one decimal digit \(that is, to specify a digit 0-9\)?

Bits aren't expensive, but what is expensive is the circuitry to let the programmer use exactly the smallest number of bits for a particular problem. Instead, modern computers generally allow memory allocation in only two sizes: the byte, which is standardized at eight bits, and the word, which is defined by the number of wires that connect the processor to the memory. As of 2017, words can be 32 bits or 64 bits wide.

---

##### Vocabulary

A **byte **is eight bits.

A **word **is the number of wires that connect the processor to the memory. As of 2017, words can be are 32 or 64 bits.

---

How many distinct values can be represented in 32 bits? You don't have to memorize the answer, because you can quickly approximate it using the fact that 210 = 1024, which is about 1000. This means that every ten bits of width multiplies the number of values that can be represented by about 1000. So, 10 bits allows about a thousand values, 20 bits is about a million values, 30 bits is about a billion, and 32 bits allows over four billion values \(because we double the billion two more times for the difference between 30 and 32\).

The exact answer for 32 bits is 4,294,967,296 so this approximation is pretty close.

You might find this trick helpful on the AP exam.

Four billion values sounds like it ought to be enough, but it's not if you're an astronomer or a banker \(or Google or Facebook\). And you learned in Unit 4 that 32 bits are not enough to give every computer an Internet address. That's why we now have 64-bit computers.

#### For You To Do

1. About how many different values can be represented in a 64-bit word? \(Don't use a calculator; use the trick!\)

### Bytes and Characters

The main use of eight-bit bytes is to represent characters of text.

1. How many bits do you need to represent the 26 letters in English and the ten digits 0-9?

Computers used six-bit-wide character codes for many years, but to have both UPPER CASE and lower case letters and punctuation requires seven bits. The first officially recognized character encoding was the seven bit ASCII \(American Standard Code for Information Interchange\) character set. It included an optional eighth bit for error detection, which was taken over to include accented characters in Spanish, French, German, and some other European languages. For example, there is an accented character in the name of the main developer of Snap!, Jens Mönig, who is German. \(The closest English sound is the "u" in "lunch."\)

As the use of computers and the Internet spread around the world, people wanted to be able to write Chinese, Japanese, Arabic, Kabyle, Russian, Tamil, etc. The Unicode character set supports about 1900 languages, using 32 modern alphabets and 107 historical alphabets that are no longer in living use. The complete Unicode character set includes 136,755 characters

The widespread use of eight-bit ASCII is the main historical reason why the eight-bit byte became standard. \(Another reason is that computer circuitry can most easily deal with widths that are powers of two.\)

#### For You To Do

1. What's the minimum number of bits needed to represent any Unicode character?
   1. The actual computer representation of Unicode is complicated.
      The most straightforward representation of Unicode uses one 32-bit word per character, which is more than enough. But program developers consider that an inefficient use of computer memory, and also, a lot of old software still in use was written when eight bits per character was standard. So Unicode characters are generally represented in a multi-byte representation in which the original 128 ASCII characters occupy one byte, while other characters may require up to four bytes. \(It's also possible to use a multi-byte sequence to tell your word processing software that you want to use one-byte codes to represent a particular non-Latin alphabet.\)
2. This question is similar to those you will see on the AP CSP exam.
   1. Which of the following CANNOT be expressed using one bit?
      1. The state of an ON/OFF switch
      2. The value of a Boolean variable
      3. The remainder when dividing a positive integer by 2
      4. The position of the hour hand of a clock



