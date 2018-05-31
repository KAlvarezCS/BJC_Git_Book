# More About Hexadecimal

We can pack four bits \(binary digits\) into one hexadecimal digit because 16 is a power of two \(16 = 2^4\). So, a group of four bits represents a value between 0 and 15, and one hex digit also represents values from 0-15 \(using 0-9 and A-F\). This makes it easier to translate between binary and hex than between other bases.

Hexadecimal is an abstraction over binary: we use hexadecimal to abbreviate binary in a more readable way.

### Translating between Binary and Hex

To translate a binary numeral \(for example, 1101011101\_2\) to hexadecimal,**start by splitting it into groups of four bits**, from right to left \(like this:11 0101 1101\).

Then **determine the value of each group and write the corresponding hex digit **\(look it up on the table at right\).

For example 11_2 = 3\_16, 0101\_2 = 5\_16, and 1101 = D\_16. So 1101011101\_2 = 35D\_16._

You can create a table like this whenever you need one.

binary	hex

00002	016

00012	116

00102	216

00112	316

01002	416

01012	516

01102	616

01112	716

10002	816

10012	916

10102	A16

10112	B16

11002	C16

11012	D16

11102	E16

11112	F16

### For You To Do

1. Translate these **binary numerals** to **hexadecimal** notation:
   1. 111011\_2
   2. 1101111\_2
   3. 10110001\_2

To translate a hex numeral \(like 4E1\_16\) to binary, **write each hex digit as a group of four bits** \(including any leading zeros\).

For example: 4-_16 = 0100-2, E_1-6 = 1110-_2, and 1\__16 = 0001-_2. So, 4E1\__16 = 010011100001_\_2 or just 10011100001_\_2 because we can drop the leading zero once the digits are all in their places.



