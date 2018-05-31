# Data Compression

**On this page**, you learn about different data compression algorithms used in common picture file formats.

This picture of the BJC logo \(shown below\) is 158 pixels wide and 186 pixels tall, for a total of 29,388 pixels. The BMP \(bitmap\) format includes each of those pixels in the picture file, at four bytes per pixel, so the file size is about 120kB.

![](https://bjc.edc.org/bjc-r/img/6-computers/bjc-logo-original.png "BJC logo uncompressed")



### Lossless Compression

That is an inefficient way to store the information. Think about the 158 pixels in the top row. The first 60 or so are white. Then come five pixels of yellowish orange \(the top slice of the "b"\). And the rest of that row is white.

...![](https://bjc.edc.org/bjc-r/img/6-computers/top-row-of-pixels-in-bjc-logo.png "top-row-of-pixels-in-bjc-logo")...  
Instead of storing all 158 pixels individually, we could compress them with run-length encoding and just store six values \(three numbers and three colors\):

| pixel count | color code |
| :--- | :--- |
| 60 | FFFFFF |
| 5 | E5A84A |
| 93 | FFFFFF |

These days, the size of one picture isn't so significant, but think about every frame of a movie, and think about the time required to send the information over the Internet. Compression makes it easier to stream that movie to you.

#### For You To Do

1. Use the Color Mixer at RGB colors and hexadecimal notation to check the result of the hex code E5A84A.

Run-length encoding is a** lossless compression** format; it doesn't lose any information. The original picture can be reconstructed with every pixel exactly correct. But run-length encoding doesn't do well if the picture is a photograph where every pixel may be \(at least slightly\) different in color from its neighbors. If the length of each color run is just one pixel, both run length and color will take twice as much space as just storing the color of each pixel. Another lossless image format you may have heard of is PNG \(Portable Network Graphics, pronounced "ping"\).

**Lossless compression **means that _no _information is lost.

The PNG algorithm is complicated and uses several different strategies depending on how color varies in each small chunk of the image. The thing to remember is that PNG is lossless.

### Lossy Compression

**Lossy **means that_some_information is lost.

**Lossy compression **algorithms let file sizes be even smaller, but the original picture can't be perfectly reconstructed; information is _lost_. This would be terrible if these algorithms were used to compress a computer program or a novel, but people's perception of images do not require extreme precision.

The most commonly used lossy compression algorithm for pictures is called JPEG \(or JPG, both pronounced "jay peg" for "Joint Photographic Experts Group," the committee that invented it\). Lossy algorithms usually let you _control the degree of precision_.

Below are an original, lossless BMP and a highly compressed JPG of a picture measuring 256×192 pixels. Can you tell which is which?

![](https://bjc.edc.org/bjc-r/img/6-computers/pond.bmp "pond pebbles")![](https://bjc.edc.org/bjc-r/img/6-computers/pond.jpg "pond pebbles")

| format | size |
| :--- | :--- |
| BMP encoding every pixel individually \(shown above\) | 148 kB |
| PNG | 106 kB |
| JPEG with least compression | 94 kB |
| JPEG with most compression \(shown above\) | 5 kB |

##### Vocabulary: Lossy vs. Lossless

**Lossless **compression \(like PNG\) is reversible \(no loss in quality\); you can reconstruct the original data. It works by removing redundant data.

**Lossy** compression \(like JPG\) is not fully reversible; you can only reconstruct an approximation of the original data. It works by removing details that people aren't likely to notice.

### Abstraction and Security

Something like a picture file is an abstraction built on other abstractions. For example, a file is an abstraction. Also, you can include a picture in an email or text message, in which case, the_message_includes a_picture_, which is a kind of_file_, which is a kind of_bitstream_.

In Unit 1, Lab 4, you learned about privacy. If you post a picture of you and your friends to a website, you are making information public about where you were and what you were doing, which may violate both your own privacy and that of your friends. Also, if your phone is lost or stolen, someone else might get access to pictures you thought were private. That's why data on cell phones is normally encrypted so that it can't be recovered without your password. Having to type your password is an example of a trade-off between convenience and security.

#### For You To Do

These questions are similar to those you will see on the AP CSP exam.

1. A film student is recording a movie on his smartphone. When the recording is done, he decides to save a copy on his computer. The student then notices that the saved copy is of much lower image quality than the original. Which of the following could NOT be a possible explanation for the lower image quality?
   1. The movie was saved using fewer bits per second than the original movie.
   2. The copy of the movie file was somehow corrupted in the process of saving.
   3. The movie was saved using a lossy compression technique.
   4. Whenever a file is saved from one place on a computer to another, some information is always lost.
2. A visual artist is processing a digital image and overwriting the original. Which of the following describe lossless transformations of the digital image from which the original image can be recovered? Choose two answers.
   1. Creating a vertically flipped copy of the image.
   2. Blurring the edges of an image.
   3. Creating the negative of an image, where colors are reversed and dark areas appear light.
   4. Creating a grayscale copy of an image.



