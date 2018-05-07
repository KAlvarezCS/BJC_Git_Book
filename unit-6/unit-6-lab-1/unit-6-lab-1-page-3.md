# The Software Domain: Programming Languages

**On this page,** you will consider why there are different programming languages and look at some of the ways that languages differ.

JavaScript, Python, Snap!, C++, Java, Scheme, Prolog... Why are there so many programming languages? Why don't we just pick the best one, or design a new best one, and stick with that?

Some languages have very narrow purposes; these are called special-purpose languages. For example, Microsoft Word has a programming language built into it called "Word macros" that's just for generating data and formatting in a document. Likewise, HTML \(Hypertext Markup Language\) is just for structuring web pages.

General-purpose languages don't have a narrow purpose in mind. In a sense, these languages are all the same: if an algorithm can be expressed in one language, it can be expressed in all of them. Several basic features are included in nearly all languages including arithmetic operators \(+, -, ×, ÷\) and Boolean operators \(and, or, not\). The differences among languages are mostly about levels of abstraction.

### High-Level and Low-Level Languages

diagram of common programming languages listed in order of abstraction level; there is a vertical double-headed arrow on the right indicating that the first row of languages \(Snap, Scheme, Prolog, Ruby, Lisp\) are 'high level languages,' the second row \(JavaScript, Python, Java, Alice, Scratch\) falls between, and the third row \(C, C++\) are 'low level languages'

A high-level language \(like Snap! or Scheme\) includes many built-in abstractions that make it easier to focus on the problem you want to solve rather than on how computer hardware works. A low-level language \(like C\) has fewer abstractions, requiring you to know a lot about your computer's architecture to write a program.

#### Why do programmers use high-level languages?

High-level languages can produce safer programs—ones that are less likely to have bugs—because the abstractions manage messy details that can trip up programmers.

[Read about how high-level languages reduce bugs in memory use.](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/03-software-languages.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-memory)

High-level languages can also make programming much more convenient because they offer more abstractions. One example is higher order functions \(like map, keep, combine, and for each\), which allow the programmer to write shorter, cleaner code.

#### For You To Do

1. Question 1
   1. This code is similar to a higher-order procedure that you have learned.  ![](/assets/talk_with_partner.png) Identify the procedure that this code imitates:      ![](https://bjc.edc.org/bjc-r/img/6-computers/hard-way.png "script variables \(resul\) \(index\); set result to \(list\); set index to 0; repeat \(length of \(words\)\): change index by 1; add \(join \(item index of words\) s\) to \(result\); report result")
      1. You learned about for each in[ Unit 2 Lab 2: Processing Each Item in a List. ](https://bjc.edc.org/bjc-r/cur/programming/2-complexity/2-data-structures-art/1-the-for-each-block.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment)
      2. You learned about keep in [Unit 2 Lab 3: Keeping Items from a List.         ](https://bjc.edc.org/bjc-r/cur/programming/2-complexity/3-predicates/2-keeping-list-items.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment)
      3. You learned about map in [Unit 3 Lab 1: Transforming Every List Item.         ](https://bjc.edc.org/bjc-r/cur/programming/3-lists/1-introduction-to-lists/4-mapping-over-list.html?topic=nyc_bjc%2F3-lists.topic&course=bjc4nyc.html&novideo&noassignment)
      4. You learned about combine in [Unit 5 Lab 3: Comparing Algorithms.         ](https://bjc.edc.org/bjc-r/cur/programming/5-algorithms/3-timing-experiments/1-comparing-algorithms.html?topic=nyc_bjc%2F5-algorithms.topic&course=bjc4nyc.html&novideo&noassignment)
         1. ![](https://bjc.edc.org/bjc-r/img/6-computers/for-each-s.png)

         2. ![](https://bjc.edc.org/bjc-r/img/6-computers/keep-s.png)

         3. ![](https://bjc.edc.org/bjc-r/img/6-computers/map-s.png)

         4. ![](https://bjc.edc.org/bjc-r/img/6-computers/combine-s.png)

In C, you can do this the long way: ![](https://bjc.edc.org/bjc-r/img/6-computers/hard-way.png "script variables \(resul\) \(index\); set result to \(list\); set index to 0; repeat \(length of \(words\)\): change index by 1; add \(join \(item index of words\) s\) to \(result\); report result")

but C doesn't let you take an expression \(like ![](https://bjc.edc.org/bjc-r/img/6-computers/join-with-s.png "join \(\) \(s\)")or ![](https://bjc.edc.org/bjc-r/img/6-computers/5-times-blank-plus-7.png "\(\(5\) × \( \)\) + \(7\)") \) and stick it into a higher order function like `map`: ![](https://bjc.edc.org/bjc-r/img/6-computers/map-s.png "report \(map \(join \(\) \(s\)\) over \(words\)\)")  
	

#### Why do programmers use low-level languages?

The best reason to use low-level languages is to write operating systems \(like Windows, Mac OS X, Android, or iOS\). You'll learn more about Operating systems on the [The Software Domain: Operating Systems](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/05-software-OS.html?topic=nyc_bjc%2F6-how-computers-work.topic&course=bjc4nyc.html&novideo&noassignment) page.

[Why else would a programmer use a low-level language?](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/03-software-languages.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-low-level-lang)

#### What is machine language?

Both high- and low-level languages are used by_people_to write computer programs. Computer hardware understands a sort of ultra-low-level language, called_machine language._Special programs called_compilers_and_interpreters_are used to translate human programming languages into machine language to be run by the computer.

[Read more about compilers and interpreters.](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/03-software-languages.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-compilers)



#### For You To Do

These questions are similar to those you will see on the AP CSP exam.

1. **Question 2 - **Which of the following statements are correct about a low-level programming language compared with a high-level programming language?

   ---

   1. Low-level language programs are generally harder for people to understand than programs written in a high-level language.

   2. A low-level language provides programmers with more abstractions than a high-level language.

   3. Low-level language programs are generally harder to debug than programs written in a high-level language.

---

* I only
* I and III only.
* II and III only.
* I, II, and III.

1. **Question 3 - **A program is written in a high-level programming language. Identify the correct statement about the program?
   1. The program can also be written in machine language using binary code, but then it will be less easily understood by people.
   2. The program can also be written in machine language using binary code, which will decrease the possibility of mistakes.
   3. The program cannot be written in binary code as only data can be represented by using binary notation.
   4. Simple parts of the program can be written in binary code, but control elements such as conditionals, loops must be expressed in a high-level programming language.

### Code Readability

One of the features that Snap! gives you is that you can put title text int he middle of a block. ![](https://bjc.edc.org/bjc-r/img/6-computers/polygon-30-15.png "polygon, sides: \(30\) side length: \(15\)")Compared to some other languages where the function has one name at the beginning and then all the inputs, this increases clarity and readability of your function. `polygon(30, 15)`

### Parallelism

One reason to create new programming languages is to make it easier to write parallel programs—programs that can use more than one processor at the same time. Today in 2017, computers and smartphones have multicore processor chips that may include 2, 4, or 8 processors all running code at the same time. \(The number of processors will increase even further over time.\) Big companies such as Google use parallelism even more; they have clusters of thousands of computers, all working on the same program.

Functional programming languages \(languages in which programmers never change the value of a variable\) are particularly well suited to parallelism because there's no danger of one processor changing the value of a variable that another processor is using. We've introduced you to functional programming techniques wherever possible throughout this course, including writing reporters and using higher order functions \(`map`, `keep`, and `combine`\).

Snap! isn't a functional programming language, but it would be if the Snap! developers removed just a few procedures, including set \(instead, you'd use input variables of recursive functions\) and these four list commands: `add`, `delete`, `insert`, and `replace `\(instead, you'd use `in front of`,` item 1 of`, and `all but first of `to report a new list with different values instead of changing the old list\).



