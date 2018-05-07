# The Software Domain: Libraries

**On this page**, you'll learn how some programmers write _libraries _to help other programmers not have to think about some messy details.  

Suppose an application programmer wants a little picture to be able to move around in a screen that also has other pictures in it. In Snap!, that's built in: import a picture as a costume that can be attached to a sprite, and then move the picture by moving the sprite. The sprite abstraction lets a programmer move a picture \(the sprite's costume\) over other pictures \(the stage background, pen trails, and other sprites' costumes\) without thinking about all the details. Not all languages have the sprite abstraction.

Other common tasks—for example, knowing where the mouse pointer is, doing arithmetic on huge numbers, or managing sound—also have complex parts. If application programmers had to deal with all of these details in every program, no software would ever get developed. And because many languages and apps need the same abilities, it's wasteful to rewrite all that code for each one. So programmers write libraries for other programmers to use.

---

##### Vocabulary

A **library **is a piece of computer code written by another programmer that you can import into your code without having to know any of the details of how it works.

An **application program interface**\(API\) is the documentation of what the _user _of a library needs to know about its contents: a description of their purpose and their inputs and outputs, but not their algorithms.

### Snap! Libraries

You've used libraries in Snap_!_, consisting of blocks \(procedures\) that provide some useful abstraction. For example, every time you![](https://bjc.edc.org/bjc-r/img/icons/import-tools.png "Import Tools"), you are importing a library of additional procedures including `for`, `keep`,`label`,`combine `, and `for each `. Snap_!  _and sentences and one for controlling pen color using different ways of encoding colors.![](https://bjc.edc.org/bjc-r/img/6-computers/libraries-1.png "Snap! File menu opened with cursor over &apos;Libraries&apos;")![](https://bjc.edc.org/bjc-r/img/6-computers/libraries-words.png "Snap! &apos;Import library&apos; dialog box highlighting &apos;Words, sentences&apos; library")

![](https://bjc.edc.org/bjc-r/img/6-computers/libraries-pen.png "Snap! &apos;Import library&apos; dialog box highlighting &apos;Set RGB or HSV pen color&apos; library")

#### For You To Do

1. Read through the libraries listed in Snap! \(as shown above\), and choose one block that interests you and that you have never used. Build a small project that uses that block, and use your project to teach that block to some of your classmates.

### Languages vs. Libraries

Often when people compare what different programming languages can do, they are really comparing libraries. For example, people think they like JavaScript because they can use it to program web pages, but that's not a property of JavaScript. It's actually a web page library built into the browser that lets you program web pages.

