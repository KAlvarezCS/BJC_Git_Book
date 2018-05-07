# The Software Domain: Operating Systems

**On this page**, you'll learn about the software that directly manages the computer's hardware, the _operating system._

Your computer came with an operating system \(OS\) installed. Operating systems are the underlying programs that your apps interact with to communicate with the computer. For computers with keyboards, it's probably Linux, macOS, or Windows. For phones and tablets, it's probably Android or iOS.

Roughly speaking, the operating system handles the basic tasks that your applications depend on, including:

* the window system, which allows more than one window to be open on your screen
* the file manager, that displays the contents of folders and lets you select files to read or manipulate
* communications with external devices like your keyboard or printer
* utilities such as a simple text editor or a calculator

In a computer, there are many applications and operating system tasks all wanting to run at once. Every operating system has a kernel that manages when all these processes run.

### The Kernel

The kernel deals directly with hardware \(keyboard, mouse, microphone, camera, hard drives, memory, printer, speakers, screen, etc.\). So the kernel is generally written in a low level language so it can control that hardware. It handles several important tasks:

* **Scheduling**. The kernel has access to the time clock that's built into the hardware and lets each program run for a small amount of time \(typically about 1/10 second\) and then switches to the next program in line.
* **Security**. Those many application programs may have bugs or malicious code. The kernel, which has access to the memory where programs and data are stored, ensures that each program is assigned a separate location in memory and doesn't interfere with other programs. The kernel also controls which data files a program can use based on file protection settings that users or applications specify for each file.
* **Input and output**. Many devices can be attached to your computer. The kernel knows how the computer's hardware reads or writes to each device. Only the kernel is allowed direct access to these devices, and it carries out authorized transfers of information for the applications.

These days, OS kernels are remarkably similar. Of the five systems listed earlier \(Linux, macOS, Windows, Android, and iOS\), four of them \(all but Windows\) are based on variants of a single kernel, called Unix.

[Read more about Unix.](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/05-software-OS.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-unix)

#### If There Is Time...

1. Explore the programs running on your computer right now.
   1. Find out how to list all the programs that are running right now on your computer, and collect such a program list in a text file.
   2. Count how many of them are programs you asked the computer to run.
   3. Of the rest, can you figure out from the names what they do?
   4. Which ones are part of the operating system \(not the OS kernel\)?
   5. See if you can figure out the purpose of some oddly-named ones by doing a web search.



