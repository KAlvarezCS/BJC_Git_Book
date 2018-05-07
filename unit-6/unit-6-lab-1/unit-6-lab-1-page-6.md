# The Digital Domain: Architecture

**On this page**, we shift from software to hardware, starting with the _architecture, _which is essentially the hardware as it looks to the software.

The software in a computer would be useless without the computer's _hardware: _the actual circuitry inside the box. Just as there are layers of abstraction for software, hardware designers also think in layers of abstraction.

![](https://bjc.edc.org/bjc-r/img/6-computers/hardware-abstraction-mini.png "simplified diagram of computer abstraction hierarchy showing three levels of decreasing abstraction: software domain, digital domain, and analog domain; there is a dividing line between the software and digital domains labeled &apos;program abstraction barrier&apos; and a dividing line between the digital and analog domains labeled &apos;digital abstraction barrier;&apos; there is a vertical double-headed arrow on the right indicating that the items listed first on the list have a &apos;high level of abstraction&apos; and those lower on the list have a &apos;low level of abstraction&apos;")

Everyone talks about computers representing all data using only two values, 0 and 1. But that's not really how electronic circuits work. Computer designers can work _as if _circuits were either off \(0\) or on \(1\) because of the **digital abstraction**, the most important abstraction in hardware. Above that level of abstraction, there are four more detailed levels, called the **digital domain**. Below the digital abstraction, designers work in the **analog domain**, in which a wire in a circuit can have any voltage value, not just two values.

On the next four pages, we'll explore four levels of the digital domain.

### The Stored Program Computer

As you'll see in Lab 3, there have been machines to carry out computations for thousands of years. But the modern, programmable computer had its roots in the work of Charles Babbage in the early 1800s.

Babbage was mainly a mathematician, but he contributed to fields as varied as astronomy and economics. Babbage lived about 150 years ago from 1791-1871. Electricity as a source of energy was unknown. The steam engine came into widespread use around the time he was born. The most precise machinery of his time was clockwork—gears.

#### The Difference Engine

Babbage's first computer was the Difference Engine. He used gears to design a complex machine that would compute and print tables of numbers \(like the tables of log or trig functions you may have in the back of a math textbook\). But these gears needed to be so precise that each one had to be handmade. The project became so expensive that the government stopped funding it, and Babbage never finished a full-scale version.

| ![](https://bjc.edc.org/bjc-r/img/6-computers/babbage-difference-engine.jpg "The Difference Engine at the London Science Museum: the image shows a large mechanical device with many gears and a large crank on the side.") The Difference Engine at the London Science Museum Image by Wikimedia user geni. Copyright 2008. License: GFDL, CC BY-SA. |
| :--- |


| ![](https://bjc.edc.org/bjc-r/img/6-computers/closeup-difference-eng.jpg "A closeup showing the gears of the Difference Engine more clearly") A closeup showing the gears more clearly Image by Carsten Ullrich. Copyright 2005. License: CC-BY-SA-2.5. |
| :--- |


[Learn more about the history of the Difference Engine.](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/06-digital-architecture.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-difference)

#### The Analytical Engine

The Difference Engine could be used to compute many different functions by manually setting the starting position of various gears. But it had **only one algorithm**: the one built into the hardware design. In 1833, Babbage began working on the Analytical Engine, which was based on the general idea of the Difference Engine but **could carry out instructions **in a primitive programming language prepared on punched cards.  


Punched cards used to program the Analytical Engine Karoly Lorentey. Copyright 2004. License: CC-BY.

![](https://bjc.edc.org/bjc-r/img/6-computers/punched-cards-analytical-engine.jpg "punched cards used to program the Analytic Engine")

These days, we are surrounded by programmable computers, and having software seems obvious now. But it wasn't obvious, and before Babbage, all algorithms were implemented directly in hardware.

So, 150 years ago, Babbage created plans for what is essentially a modern computer, although he didn't have electronics available. His underlying idea for hardware was entirely mechanical, but it turned out not to be possible for him to build it with then-current technology. We didn't get _usable _computers until there was an underlying technology small enough, inexpensive enough, and fast enough to support the software abstraction. You'll learn about this technology, transistors, soon.

The abstraction of _software _\(a program stored in the computer's memory\) is what makes a computer usable for more than one purpose.

[Learn more about the Analytical Engine.](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/06-digital-architecture.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-analytical)

[Learn about Ada, Countess Lovelace's invention of symbolic computing.](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/06-digital-architecture.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-ada)

### What's an Architecture?

The Analytical Engine \(described above\) was the first programmable computer architecture. The processor in the computer you are using today understands only one language, its own_machine language_—not Java, not C, not Snap_!_, not Python, nor anything else. Programs written in those other languages must first be translated into machine language.

The most important part of the architecture is the machine language, the set of ultra-low-level instructions that the hardware understands. This language is like a contract between the hardware and the software: The hardware promises to understand a set of instructions, and the software compiles programs from human-friendly language into those instructions.

---

##### Vocabulary

**Machine language **is the lowest-level programming language; it is directly understood by the computer hardware.

**Architecture **is an abstraction, a specification of the machine language. It also tells how the processor connects to the memory. It doesn't specify the circuitry; the same architecture can be built as circuitry in many different ways.

One important part of an architecture is the number of wires that connect the processor and memory. This is called the _width _of the architecture, measured in _bits_\(number of wires\). A wider computer can process more data in one instruction.

[What does machine language look like?](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/06-digital-architecture.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-machine-language)

Learn about:

* [PC/Mac architecture](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/06-digital-architecture.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-architecture)
* [smartphone architecture](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/06-digital-architecture.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-architecture-phone)
* [embedded architecture and the "Internet of Things"](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/06-digital-architecture.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-architecture-iot)
* [hobbyist computer architecture](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/06-digital-architecture.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-architecture-hobby)
* [computer architecture in general](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/06-digital-architecture.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-architecture-general)



#### Take It Further

1. Learning enough about the Analytical Engine to be able to write even a simple program for it is quite a large undertaking. Don't try it until after the AP exam, but if you are interested, there are extensive online resources available here:
   1. [The Analytical Engine Table of Contents](http://www.fourmilab.ch/babbage/contents.html)
   2. [Web Analytical Engine Emulator](http://www.fourmilab.ch/babbage/emulator.html)



