# More About Hexadecimal

We can pack four bits \(binary digits\) into one hexadecimal digit because 16 is a power of two \(16 = 2^4\). So, a group of four bits represents a value between 0 and 15, and one hex digit also represents values from 0-15 \(using 0-9 and A-F\). This makes it easier to translate between binary and hex than between other bases.

Hexadecimal is an abstraction over binary: we use hexadecimal to abbreviate binary in a more readable way.

### Translating between Binary and Hex

To translate a binary numeral \(for example, 1101011101\_2\) to hexadecimal,**start by splitting it into groups of four bits**, from right to left \(like this:11 0101 1101\).

Then **determine the value of each group and write the corresponding hex digit **\(look it up on the table at right\).

For example 11_2 = 3\_16, 0101\_2 = 5\_16, and 1101 = D\_16. So 1101011101\_2 = 35D\_16._

You can create a table like this whenever you need one.

binary    hex

00002    016

00012    116

00102    216

00112    316

01002    416

01012    516

01102    616

01112    716

10002    816

10012    916

10102    A16

10112    B16

11002    C16

11012    D16

11102    E16

11112    F16

### For You To Do

1. Translate these **binary numerals** to **hexadecimal** notation:
   1. 111011\_2
   2. 1101111\_2
   3. 10110001\_2

To translate a hex numeral \(like 4E1\_16\) to binary, **write each hex digit as a group of four bits** \(including any leading zeros\).

For example: 4-_16 = 0100-2, E\_1-6 = 1110-\_2, and 1\_\_16 = 0001-\_2. So, 4E1\_\_16 = 010011100001_\_2 or just 10011100001\_\_2 because we can drop the leading zero once the digits are all in their places.

#### For You To Do

1. Translate these **hexadecimal numerals** to **binary **notation:
   1. 18\_16
   2. 5D\_16
   3. F8\_16

In practice, you rarely change number bases by hand, except of course on the AP exam. Once you understand the basic principles of these representations, it's perfectly fine to use a

[Binary to Decimal to Hexadecimal Converter](https://www.mathsisfun.com/binary-decimal-hexadecimal-converter.html)

### Hexadecimal Colors

Computers have several ways of representing color depending on the purpose. For example, three-color **RGB **\(red, green, blue\) is used for screen display, and four-color **CMYK **\(cyan, magenta, yellow, black\) is used for printing. On a computer screen, each **pixel **that makes up a picture is assigned an RGB color code that defined by the intensity of red, green, and blue in that color. These three color intensities each range from 0 to 255 \(one byte is used for each of the three colors\), which is 00 to FF in hex notation.

If \(R, G, B\) = \(128, 0, 255\), the color is purple: some red and as much blue as possible, but no green at all. If all three colors are as bright as possible \(all are 255\), we see white; if they are as dark as possible \(all are 0\), we see black. Instead of writing \(255, 255, 255\) for white and \(128, 0, 255\) for purple, we often use hex notation: FFFFFF and 8000FF. And this color is red 255, green 127, and blue 0, which is FF7F00 in hex.

Learn more about color codes.

Sometimes a fourth number is used to represent the color transparency, like the ghost effect you used in your very first BJC project in [Unit 1 Lab 1](https://bjc.edc.org/bjc-r/cur/programming/1-introduction/1-building-an-app/6-keeping-score.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment).

**RGB works well for lights,** such as the tiny lights \(pixels\) in your computer screen, so it is great for computers. But it's not good for printers: no combination of Red, Green and Blue sprayed on paper would quite make black, zero of each would leave the paper white \(not black\), and artists know that mixing red and green paint does not make yellow \(but that's how you make yellow with light: FFFF00\). **Ink or paint colors are measured in CMYK**: Cyan, Magenta, Yellow, and Black. And some colors such as brown and brick-red \(darker than pure red\) are hard to figure out in RGB units, even for display in lights. Another color system is called **HSB,** for hue, saturation, brightness.

Snap!'s system is similar to HSB. "Pen color" is hue \(location on the rainbow\), and "pen shade" is more or less saturation \(zero means black, 100 means full rainbow color\).

#### For You To Do

1. Represent these colorsi n hex notation:
   1. red 0, green 149, and blue 235
   2. red 128, green 90, and blue 0
   3. red 163,green 0, and blue 84
2. Predict what this RGB color will look like based on its values: red 145, green 0, blue 226.
3. Predict what this hex RGB color will look like: 04FF61.
4. Another way to represent colors is by their names. For example, the color 4B0082 is called Indigo and tnje color 8B4513 is called SaddleBrown. Compare these two representations \(hex RGB codes vs. color names\) in terms of: space required, ease of understanding, and ease of use.
5. Why do we use binary, decimal, and hexadecimal? Why not just one?
6. In earlier units, we used abstraction to describe creating custom blocks and abstract data types. Here, we use abstraction to talk about hexadecimal vs. binary. how can abstraction describe these very different things? What do these things have in common?

#### If There Is Time..

1. Explore this RGB/HEX color converter: [http://hex.colorrs.com](http://hex.colorrrs.com/)
2. Play with this[ Interactive Color Wheel](http://www.mathsisfun.com/numbers/color-wheel-interactive.html)
3. Read more about [RGB colors and hexadecimal notation.](http://www.mathsisfun.com/hexadecimal-decimal-colors.html)

#### Take It Further

1. Load the Snap!_ _RGB library into one of your projects to explore RGB color further. In the File menu, choose "Libraries..." and then choose "Set RGB or HSV pen color" as shown on the [Libraries](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/04-software-libraries.html?topic=nyc_bjc%2F6-how-computers-work.topic&course=bjc4nyc.html&novideo&noassignment) page. This will give you a new "Pen" block:

   ![](https://bjc.edc.org/bjc-r/img/4-internet/set-pen-color-RGB.png "set pen color to r: \(\) g: \(\) b: \(\)")![](https://bjc.edc.org/bjc-r/img/6-computers/libraries-pen.png "Snap! &apos;Import library&apos; dialog box highlighting &apos;Set RGB or HSV pen color&apos; library")

As in all Snap! blocks, the numeric input slots take values represented in base 10 \(not hex\). Each color component has a value between 0 and 255.



