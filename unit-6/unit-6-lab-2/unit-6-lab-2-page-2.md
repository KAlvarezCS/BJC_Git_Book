* [ ] # Binary Sequences

**On this page,** you will learn more about how information is represented inside the computer as sequences of bits.

So far we've been working with small chunks of data, from Boolean values \(one bit\) to characters \(eight bits\). But of course some information in your computer or smartphone is much bigger than that. For starters, characters aren't generally used one at a time; they're used in text strings such as `"Welcome to the Beauty and Joy of Computing."` These 43 characters occupy 43 bytes of computer memory. But the real champion users of space are media files: pictures, sounds \(mostly music\), and video.

If we could see inside the memory’s bits, a section of the memory might look something like this:

01000001001000000111001101101101011000010111001001110100001000000111000001101000011011110110111001100101001011000010000001101100011010010110101101100101001000000111100101101111011101010111001000100000011011000110000101110000011101000110111101110000001000000110111101110010001000000110010001100101011100110110101101110100011011110111000000100000011000110110111101101101011100000111010101110100011001010111001000101100001000000110001101100001011011100

In many programming languages there's a convention that every text string ends with a null byte, in which all eight bits are zero, a code that's reserved for this purpose. So our "Welcome..." string might actually occupy 44 bytes.

That shows just 449 bits. A 16GB cell phone has sixteen gigabytes \(about 16 billion bytes\) of storage, each byte containing 8 bits. That's 128,000,000,000 bits. Printed on paper as ones and zeros, the 16 GB phone’s memory would take nearly 40,000,000 pages! The information in storage—whether it is a text message, a photograph, a song, a computer program, or a list of phone numbers—looks just the same, a sequence of bits that are either On or Off \(one or zero\).

##### Vocabulary

A **binary sequence** \(also called a bitstream\) is a string of ones and zeros.

#### Sizes

Here are a few rough examples of what kind of data would fit in how much memory:

| **name** | amount | example |
| :--- | :--- | :--- |
| bit |  | 1 |
| byte | 8 bits | 11011001 |
| kilobyte | 2^10 \(1,024\) bytes | a couple of paragraphs |
| megabyte | 2^20\(1,048,576\) bytes | about 1 book |
| gigabyte | 2^30 \(1,073,741,824\) bytes | a little more than 1 CD |
| terabyte | 2^40 \(1,099,511,627,776\) | about 1,500 CDs |
| petabyte | 2^50 \(1,125,899,906,842,624\) bytes | about 20 million filing cabinets of text |
| exabyte | 2^60 \(1,152,921,504,606,846,976\) bytes | about 20% of all the words ever spoken by humankind |

As we write this in 2017, it's common to have a terabyte disk drive on your desk. Web services deal with petabytes or exabytes of data.

Where do these prefixes like "tera-" and "peta-" come from?

When we write big numbers, we put commas every three digits \(counting from the right\). Each group of three has a name: thousand, million, billion, and so on. So, the number 1,234,567,890 is pronounced "one billion, 234 million, 567 thousand, 890." Those group names \("thousand" and so on\) also have prefix names used in metric measurements:

prefix	amount	amount as numeral

kilo-	thousand	1,000

mega-	million	1,000,000

giga-	billion	1,000,000,000

tera-	trillion

\(a million million\)	1,000,000,000,000

peta-	quadrillion	1,000,000,000,000,000

exa-	quintillion

\(a billion billion\)	1,000,000,000,000,000,000

Digits for groupings smaller than one \(fractions\) have metric prefixes too:



prefix	amount	amount as fraction

milli-	thousandth	1/1,000

micro-	millionth	1/1,000,000

nano-	billionth	1/1,000,000,000

pico-	trillionth	1/1,000,000,000,000

femto-	quadrillionth	1/1,000,000,000,000,000

atto-	quintillionth	1/1,000,000,000,000,000,000

The fractional names are used to measure times in the computer, such as a nanosecond memory access time, or distances between wires on a chip, which are measured in nanometers.



#### For You To Do

1. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:https://bjc.edc.org/bjc-r/prog/6-computers/U6L1-TranslatingBinary.xml)
   1. Take a look at these 3 custom blocks that you will use to explore binary sequences:
      1. A reporter that accepts a string of text as input and translates that text into a binary sequence: ![](https://bjc.edc.org/bjc-r/img/6-computers/translate-text-to-binary.png "translate text \(\) to binary sequence")
      2. A reporter that accepts a binary sequence as input and translates it into text:![](https://bjc.edc.org/bjc-r/img/6-computers/translate-binary-to-text.png "translate binary sequence \(\) to text")
      3. A command block that accepts a binary sequence as input and draws a black and white image on the stage where each 0 in the sequence becomes a white "pixel" and each 1 becomes a black "pixel."![](https://bjc.edc.org/bjc-r/img/6-computers/translate-binary-to-text.png "translate binary sequence \(\) to text")
         1. You can use the second and third inputs to control where the block breaks the sequence to start a new line and also how large the image is drawn.
2. Translating a short text string into a binary sequence.

   1. Find the` set `\(output\) `to...` instruction and change the input text to a short text string of your choosing. The reported binary sequence will be stored in the output variable with quotes around it.![](https://bjc.edc.org/bjc-r/img/6-computers/set-output-to-translate-text.png "set \(output\) to \(translate text \(Beauty and Joy of Computing\) to binary sequence\)")

   2. Access the output by right-clicking \(or control-clicking\) on the OUTPUT watcher on the stage and choosing "export..." The binary sequence will download as a text file. Copy the binary sequence out of the file, but not the quotes. ![](https://bjc.edc.org/bjc-r/img/6-computers/exporting-output-watcher.png "image of output watcher on stage storing a binary sequence with the dropdown menu open and the point on &apos;export...&apos;")

      1. The quotes tell Snap! that the binary sequence should be saved "as is." Without some text at the beginning, Snap! will think your binary sequence is a number, and it would remove any zeros at the front, which would change the interpretation of where each byte begins and ends.

      2. Even Snap! has bugs. When you paste this data into Snap!, it may extend beyond the edges of the box. Developers are working to fix this.![](https://bjc.edc.org/bjc-r/img/6-computers/binary-sequences-bug.png "image of output pasted into block and extending past the edges of the block")

3. Paste the outputted binary sequence into the translate binary sequence to text block and run it. \(It may take a moment to report.\)

   1. Is your original text reported back? \(If not, you may have included the quotes or lost a bit or two while copying.

   2. Once you've gotten your original text to report back, try making some changes.

      1. What happens if you change one bit?

      2. What happens if you add a bit somewhere in the middle of the sequence?

      3. What happens if you add a bit at the beginning?

4. Go back to the exported output.txt file and copy your original binary sequence again \(without the quotes\). Paste it into the translate binary sequence to B&W image block and run the block. You are not likely to see anything meaningful. Why not?
5. Try this binary sequence in` translate binary sequence to B&W image` with the second input set to 14 pixels wide:    `00000110000000000001000110000000010000000000001100100110000011111111000001100111100000010010110011000111001111100000100110110000000001000000000000110000000000111000000011000100011000010000000100000110000110000000111111000000`

   1. You should something like the BJC logo:

      ![](https://bjc.edc.org/bjc-r/img/web/bjc-logo.png "Beauty and Joy of Computing logo: a &apos;b,&apos; a &apos;j,&apos; and a &apos;c&apos; with a smile below")
6. What do you get if you translate the same binary sequence into text? Why?

So if pictures, music, and words all look the same in memory—all binary sequences—how can the computer tell what any chunk of memory actually is? For example, should the sequence 01000001 be interpreted as the number 65, the letter A, a rather dark shade of red, or something else?



The meaning of a sequence of bits depends on the context in which it is used. What exactly do we mean by "context"? How does a programming language know whether to interpret a bit sequence as an integer, a picture, a string of characters, an instruction, or something else? There's always another bit sequence somewhere that encodes the **data type** of the bit sequence.

But different languages use data types differently.

In high-level languages, that data type code is attached to the value itself. In lower-level languages, when you make a variable, you have to say what type of value it will contain, and the data type is attached to the variable, so you can't get exact answers when the values are integers and also be able to handle non-integer values of the same variable. So instead of seeing: 

![](https://bjc.edc.org/bjc-r/img/4-internet/varfoo.png "script variables \(foo\)")

you see things like:

![](https://bjc.edc.org/bjc-r/img/4-internet/intfoo.png "integer \(foo\)")

Snap! has strengths that many programming languages do not, and it's very likely that your next year's computer science class will use one of those other languages. For example, if you take the AP Computer Science A course, you will use Java.

#### For You To Do

1. This question is similar to those you will see on the AP CSP exam.
   1. A particular online retail company uses 9-bit binary sequences to identify each unique product for sale. Expecting to increase the number of products it sells, the company is planning to switch to 10-bit binary sequences. Which of the statements below best describes the consequence of using 10-bit sequences instead of 9-bit sequences?
      1. Ten more products can be identified uniquely.
      2. Ten times as many products can be identified uniquely.
      3. Two more products can be identified uniquely.
      4. Twice as many products can be identified uniquely.

#### If There Is Time...

1. Look inside the `translate text to binary sequence` and` translate binary sequence to text` reporters. **Describe how these two reporters work.** There are several custom blocks inside:
   1. `pack 8-bit byte `takes a binary sequence of 8 bits or less and add enough zeros to the front to make a whole byte. How is this used?
   2. `translate decimal to binary `takes a decimal value \(a normal number\) as input and translates it to the binary representation of that number. This block uses recursion. Why is recursion helpful here?
   3. `translate text to Unicode list` takes a text string and outputs a list of each character's Unicode value. Why is a list output helpful here?



