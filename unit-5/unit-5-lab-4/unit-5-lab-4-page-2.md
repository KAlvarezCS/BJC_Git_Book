# An Undecidable Problem

**On this page,** you will consider a problem that _can't _have an answer.

By this point in the course, you've experienced the frustration of debugging a program. It would be great if there were a general-purpose debugging program that could read any code and determine if there were bugs. Unfortunately, we can use proof by contradiction \(as Alphie, Betsy, and Gamal did on the previous page\) to prove that this can't be done.

---

##### Vocabulary

An **infinite loop** is a sequence of computer instructions that repeats forever.

An **undecidable problem** is one for which no algorithm can ever be written that will always give a correct true/false answer for every input value.

---

First, we'll assume that it's possible to write a function to determine if there are infinite loops in a program \(situations in which a function runs forever without reporting a value\). Then, we'll use that function in a program especially designed to create a contradiction \(a logical incompatibility\) to prove that the assumption is wrong—**no general-purpose debugging program program can exist**. "Does this program have bugs" is an undecidable problem; no algorithm can ever be constructed that always solves it correctly for every program.

### Assuming That a Halts? Function Exists

#### Making the Assumption

First, we _assume _there exists a function called `halts? `that determines whether a given reporter will report a value in a finite time. \(If so, we say that the reporter _halts. _\) It takes two inputs: a function and an input value for that function. It reports `true `if the function would report a value when given that input; it reports `false `if the function would run forever \(in an infinite loop\). 

We can't show the code inside halts?; we are proving that it can't be written at all, no matter what code implements it.

![](https://bjc.edc.org/bjc-r/img/5-algorithms/halts.png "halts? \(function\) \(input\)")

For example, the function `round `will not run forever when given the input 7.5; it will report 8.

![](https://bjc.edc.org/bjc-r/img/5-algorithms/halts-reporting.png "halts?\(round\(\)\)\(7.5\) reporting true") because ![](https://bjc.edc.org/bjc-r/img/5-algorithms/round%287-5%29.png "round \(7.5\)") reports a value.

The gray ring around the input function means that the `halts? `code will treat the input function as data instead of running it.

On the other hand, imagine we had a function that will get stuck in an infinite loop when given the inputfoo; it would never report \(never halt\).   
![](https://bjc.edc.org/bjc-r/img/5-algorithms/halts-reporting-false.png "halts?\(program with an infinite loop \(\)\)\(foo\) reporting false") because  ![](https://bjc.edc.org/bjc-r/img/5-algorithms/program-with-loop%28foo%29.png "program with an infinite loop \(foo\)") loops infinitely.

#### Reviewing the Plan for the Proff

We'll use proof by contradiction to show that the following question _can't _be answered _in general:_

_**Will a certain computer program, given a certain input, report a result in a finite amount of time?**_

---

#### For You To Do

1. ![](/assets/talk_with_partner.png)
   1. Describe the process of proof by contradiction.
   2. Describe what the halts? function does.
   3. Describe how you are going use the halts? function in this proof by contradiction process.

---

### Showing How This Creates a Contradiction

### Constructing a Program For Which Halts Won't Work

To prove there can be no such function, we need to create a contradiction. We need to show that there has to be at least one function and one input to that function for which`halts?`fails to work the way we assumed it does. So, we can make up a block,`tester`, specifically for the purpose of breaking`halts?`: ![](https://bjc.edc.org/bjc-r/img/5-algorithms/tester-halting.png "tester\(reporter\){if\(halts?\(reporter\)\(reporter\){forever{}}else{report\(It doesn&apos;t matter what value is reported.\)}}")

---

Just like the`#`and`⋮ `symbols for inputs declared to be _numbers _or _lists _, the `λ `is not part of the input's name but is a **type hint **that was created when selecting the _reporter _input type:![](https://bjc.edc.org/bjc-r/img/5-algorithms/input-type-reporter.png "selecting the Reporter input type")Recall that selecting an input type changes the appearance of the input slot so that it indicates what kind of input is expected.  The input slot for `tester `will have a rounded gray ring to indicate that the input should be a reporter: ![](https://bjc.edc.org/bjc-r/img/5-algorithms/tester%28%29.png "tester \(\)")

---

The `forever `block in this script creates an infinite loop. If the `tester `code ends up in this part of the `if `statement, it will never report anything. So whether `tester `_itself _will halt depends on the output of the `halts? `predicate in the`if`statement inside it.

The expression ![](https://bjc.edc.org/bjc-r/img/5-algorithms/halts-reporter-reporter.png "halts? \(reporter\) \(reporter\)") asks what will happen if we call the inputted function \( reporter\) with _itself _ statement I'm making _right now _is false."

![](https://bjc.edc.org/bjc-r/img/icons/tough-stuff-mini.png "Tough Stuff") This _is _challenging. Stick with it! We are _creating a contradiction _to prove that the `halts?`function called inside `tester `can't exist.

#### Using Self-Reference to Lead to Contradiction

To make the situation _exactly _like what Betsy said \("The statement I'm making _right now _is false."\), we'll call `tester `on _itself_:![](https://bjc.edc.org/bjc-r/img/5-algorithms/testertester.png "tester\(tester\(\)\)") Now, the `if `statement inside the `tester `block will ask if `tester `will halt \(not run forever\) if it's called with `tester `as it input. The predicate in the `if `statement will become `halts? (tester) (tester)`.

![](https://bjc.edc.org/bjc-r/img/5-algorithms/tt-t-htt.png "tester\(tester\) -&amp;gt; reporter input in tester definition -&amp;gt; halts? \(tester\) \(tester\)")So, just as in the examples above,

![](https://bjc.edc.org/bjc-r/img/5-algorithms/halts-tester-tester-reporting-true.png "halts \(tester\) \(tester\) reporting true") would mean that ![](https://bjc.edc.org/bjc-r/img/5-algorithms/testertester.png "tester\(tester\(\)\)") returns a value.

![](https://bjc.edc.org/bjc-r/img/5-algorithms/halts-tester-tester-reporting-false.png "halts \(tester\) \(tester\) reporting false") would mean that ![](https://bjc.edc.org/bjc-r/img/5-algorithms/testertester.png "tester\(tester\(\)\)") loops infinitely.

#### Understanding the Contradiction

When we call ![](https://bjc.edc.org/bjc-r/img/5-algorithms/testertester.png "tester\(tester\(\)\)") , we run into the contradiction. To see how, look back at the `tester `definition: ![](https://bjc.edc.org/bjc-r/img/5-algorithms/tester-halting.png "tester\(reporter\){if\(halts?\(reporter\)\(reporter\){forever{}}else{report\(true\)}}")

Showing that **the result has to be wrong **involves a _case analysis _like the ones used to solve the logic puzzles on page 1. Consider the two possible cases: 

1. If ![](https://bjc.edc.org/bjc-r/img/5-algorithms/halts-tester-tester-reporting-true.png "halts \(tester\) \(tester\) reports true") then `tester `will take the first branch of the `if`, and so it will loop forever. That means ![](https://bjc.edc.org/bjc-r/img/5-algorithms/testertester.png "tester\(tester\(\)\)") _won't _halt, and so `halts? `gave the wrong answer.

2. If ![](https://bjc.edc.org/bjc-r/img/5-algorithms/halts-tester-tester-reporting-false.png "halts \(tester\) \(tester\) reports false") then `tester `will take the `else `branch and report "It doesn't matter what value is reported." That means ![](https://bjc.edc.org/bjc-r/img/5-algorithms/testertester.png "tester\(tester\(\)\)") _will _halt, and so `halts? `is wrong again.

It doesn't matter what value tester reports, just that it reports some value, but it does matter what value halts? reports.

No matter what halts? reports, it will always disagree with itself in a program like this. This contradiction \(this logical impossibility\) means that the assumption that it's possible write halts? has to be wrong. This isn't just a claim about what will happen in Snap!. The language you use to explore a computational problem can impact the clarity or readability of your code but not whether a solution to a problem exists. Even with advances in quantum computing, we will never be able to create a general-purpose debugging program. This famous example is known as the halting problem, and the fact that the halting problem is not decidable is the Halting Theorem.

---

#### For You To Do

1. ![](https://bjc.edc.org/bjc-r/img/icons/talk-with-your-partner.png "Talk with Your Partner")Go over this whole proof again together. Make sure both you and your partner understand:

   1. Everything from exercise 1 about proof by contradiction, what `halts?`
      does, and how `halts? `is going to be used in the proof.

   2. The basics of how the `tester `function behaves \(for _any _inputted function\).
   3. How calling ![](https://bjc.edc.org/bjc-r/img/5-algorithms/testertester.png "tester\(tester\(\)\)") leads to a contradiction.

   4. What that contradiction means in the proof.

##### Who first proved the Halting Theorem?

Alan Turing \(1912-1954\) was one of the founders of computer science. He is known for two achievements. First, he made a massive contribution to winning World War II by inventing a mathematical theory and corresponding computer hardware to break the encoded messages generated by the German Enigma machine. Second, together with his colleague Alonzo Church, Turing was a founder of theoretical computer science: proving how computers must work regardless of future technology. Though his work on the Halting Problem, he proved that there are computations that can never be done, no matter how big and fast computers get.

When Turing did this work, there were no programmable computers; people had to rewire physical machines to solve each new problem. With powerful programming languages \(such as Snap!\), we can see and understand the essence of Turing's proof much more easily because we can use functions as inputs to other functions, as you've seen with map, keep, and combine. This proof was even harder for Turing because he had to invent the idea of a computer program that can itself be represented as data inside the computer.



