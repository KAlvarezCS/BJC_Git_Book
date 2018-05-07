# Abstraction Inside the Computer

In Unit 4 [A Hierarchy of Open Protocols](https://bjc.edc.org/bjc-r/cur/programming/4-internet/2-communication-protocols/3-open-protocols.html?topic=nyc_bjc%2F4-internet.topic&course=bjc4nyc.html&novideo&noassignment), you saw that the Internet software is arranged in several levels of abstraction, with application programs \(like your email program\) at the highest level and network hardware protocols such as WiFi and Ethernet at the lowest level. Recall that _higher _levels are closer to what users want to be thinking about; lower levels are closer to the way machines work.

Like the Internet, the way a computer works on the inside also has levels of abstraction.

**In this lab, **you will learn about the levels of abstraction in computer software and hardware.

**On this page, **you will learn get an overview of three groups \(_domains_\) of levels of abstraction.  


There are a lot of levels of abstraction in how computers work. Here they are organized into three overarching domains:![](https://bjc.edc.org/bjc-r/img/6-computers/hardware-abstraction.png "diagram of computer abstraction hierarchy showing three levels of decreasing abstraction: software domain \(including applications, programming languages, libraries, and operating systems\), digital domain \(including architecture, components, integrated circuits, and logic gates\), and analog domain \(including transistors\); there is a dividing line between the software and digital domains labeled &apos;program abstraction barrier&apos; and a dividing line between the digital and analog domains labeled &apos;digital abstraction barrier;&apos; there is a vertical double-headed arrow on the right indicating that the items listed first on the list \(and their sub-lists\) have a &apos;high level of abstraction&apos; and those lower on the list have a &apos;low level of abstraction&apos;")

Different people might draw this diagram slightly differently, so don't try to memorize all the levels. The key abstraction levels to remember are software, digital computer hardware, and underlying analog circuit components.

### Software Domain

The programs you write and use are software, but underneath these programs is more software that helps them work. In this lab, we'll look at four layers of abstraction in the software domain:

* **applications** that you write and use
* **programming languages** that are used to write them
* **libraries** of useful functions that hide messy details
* **operating systems** that interface with the hardware

Software is an _abstraction_—a way of thinking about the computer without thinking about how it works.

Similarly, an automobile driver is operating at a high level of abstraction when using the brake pedal. As long as the engineers and mechanics designed and built the car right, drivers don't need to know the details about how the brake system works—they just use it at a high level.

### Digital Domain

In the software domain, each level of abstraction is a different piece of software, but the levels of abstraction in the digital domain are different ways of thinking about the same physical object. The circuitry inside a computer is complicated, and to make building it possible, engineers think about it at several different levels of abstraction:

* The **architecture** is the instructions that software can send that the hardware will understand.
* The computer has **components** \(such as memory, processors, video cards, etc.\) that implement the architecture.
* Those components are built out of **integrated circuits\(chips\),** which are the black rectangles that you can see on this circuit board.
* Those integrated circuits are designed around **logic gates,** the fundamental building blocks that implement Boolean functions.

You learned about Boolean functions in [Unit 2 Lab 3: Making Decisions by Using Predicates](https://bjc.edc.org/bjc-r/cur/programming/2-complexity/3-predicates/1-adding-questions.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment) . ![](https://bjc.edc.org/bjc-r/img/blocks/and.png "\(\) and \(\)") ![](https://bjc.edc.org/bjc-r/img/blocks/or.png "\(\) or \(\)")![](https://bjc.edc.org/bjc-r/img/blocks/not_small.png "not \(\)")

### Analog Domain

Logic gates, which are the lowest abstraction level of the digital domain, operate on ones and zeros. In physical reality, those logic gates are built out of transistors, a type of circuit component. Transistors aren't like light switches that are either on or off. There can be in-between values \(like "only 23% on"\). So, electrical engineers have to think about the laws of electronics to design digital circuits so that in-between values don't happen.

**Vocabulary: analog vs. digital**

Digital and analog are opposites. **Digital **means information that is represented as _ones and zeros_. **Analog **means information that is represented by signals that _vary continuously_\(that is, including in-between values\).

