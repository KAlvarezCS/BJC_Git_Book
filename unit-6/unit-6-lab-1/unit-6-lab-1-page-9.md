# The Digital Domain: Logic Gates

**On this page, **you review three Boolean operators \(`and`, `or`, and `not`\) and learn how they relate to electronic circuitry.

In a circuit with billions of transistors, or even thousands of transistors, hardware designers can't think about each individual transistor. Just as programmers use abstraction, hardware architects use abstractions, in which a group of transistors and other circuit elements are considered as a single thing. What kinds of things? There are basically two kinds, one for memory and one for computation.

---

[Learn more about memory.](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/09-digital-logic-gates.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-memory)

Memory is made out of \_flip-flops.\_A flip-flop is a circuit that has two stable states, on and off. An input signal can tell it to turn on, turn off, or change whatever it's state is. Once that happens, the flip-flop stays in the new state until it gets another signal. It has an output that reflects its state: on if the flip-flop is on, off if it's off.

---

### Boolean Operators

The circuits to do computation are more interesting. They compute _functions,\_just like reporters in Snap_!\_. Since computers do a lot of arithmetic, you might think that the basic circuit functions would be addition, subtraction, multiplication, and division, but that's not the case. Of course there \_are \_circuits to do those things, but they're made out of \_logic gates:\_circuits that compute **Boolean functions**:`and`,`or`, and `not`.

The reason that Boolean functions are considered more fundamental is that their inputs and outputs can be represented with a single wire going into or out from the circuit. That's not true about arithmetic functions. If you consider a voltage on a wire as meaning 1, and no voltage as meaning 0, then you have to see that an adder will have \_three \_possible output values, because 1+1=2, which is neither 0 nor 1. By contrast, if you consider a voltage on a wire as meaning True, and no voltage as meaning False, then the output from a Boolean function of two inputs can still only be True or False, so only one output wire is needed.

You saw some examples in [Unit 2 Lab 3: Making Decisions by Using Predicates](https://bjc.edc.org/bjc-r/cur/programming/2-complexity/3-predicates/1-adding-questions.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment) :`AND`, `OR`, and `NOT`: ![](https://bjc.edc.org/bjc-r/img/6-computers/logical-operators/and-TT-reporting.png "\(true\) AND \(true\) reporting true")![](https://bjc.edc.org/bjc-r/img/6-computers/logical-operators/and-TF-reporting.png "\(true\) AND \(false\) reporting false")![](https://bjc.edc.org/bjc-r/img/6-computers/logical-operators/and-FF-reporting.png "\(false\) AND \(false\) reporting false")![](https://bjc.edc.org/bjc-r/img/6-computers/logical-operators/or-TT-reporting.png "\(true\) OR \(true\) reporting true")![](https://bjc.edc.org/bjc-r/img/6-computers/logical-operators/or-TF-reporting.png "\(true\) OR \(false\) reporting true")![](https://bjc.edc.org/bjc-r/img/6-computers/logical-operators/or-FF-reporting.png "\(false\) OR \(false\) reporting false")![](https://bjc.edc.org/bjc-r/img/6-computers/logical-operators/not-T-reporting.png "NOT \(true\) reporting false")![](https://bjc.edc.org/bjc-r/img/6-computers/logical-operators/not-F-reporting.png "NOT \(false\) reporting true")

**Some other ways to think about Boolean operators:**

It is possible to emulate Boolean operations electronically and these operations are sometimes represented as truth tables \(either with true/false or ones/zeros\).

* [A circuit emulation and truth tables for`and`.](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/09-digital-logic-gates.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-truth-tables-and)
* [A circuit emulation and truth tables for`or`.](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/09-digital-logic-gates.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-truth-tables-or)
* [A circuit emulation and truth tables for`not`.](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/09-digital-logic-gates.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-truth-tables-not)

### Logic Gates

Inside a computer, Boolean operations are implemented in physical circuitry using logic gates. \(A single gate implements one of the  basic functions `and`,`or`, or `not` ample, the following diagram of a logic circuit with two gates represents the Boolean expression![](https://bjc.edc.org/bjc-r/img/6-computers/%28a%29or%28%28a%29and%28b%29%29-booleans.png "A or \(A and B\)") . Can you see how?![](https://bjc.edc.org/bjc-r/img/6-computers/%28a%29or%28%28a%29and%28b%29%29-gate.png "logic gate diagram of \(A or \(A and B\)\)")

#### For You To Do

1. ![](/assets/twoPeopleThinking.png)Look at the logic circuit drawn above. For what values of A and B will the output be `true`?
   1. On the previous page, you learned about tungsten and tin, and here we're talking about Boolean functions. In what sense is this less abstract? **From the point of view of the chip designer, logic gates are the fundamental building blocks of a digital circuit.** \(The actual physical chip fabrication is at an even lower level of abstraction, in the analog domain.\)
2. Review `AND`,`OR`, and `NOT`with the following questions, which are similar to the type of questions you will see on the AP CSP exam.

##### Question 1

1. Which of the following expressions will report true  
   1. ![](https://bjc.edc.org/bjc-r/img/6-computers/boolean-quiz-a.png "\(T and F\) and \(not \(T and F\)\)")  
   2. ![](https://bjc.edc.org/bjc-r/img/6-computers/boolean-quiz-b.png "\(not \(T or F\)\) or \(T or F\)")

* I only

* II only

* I and II
* Neither I nor II

##### Question 2

1. Which of the following logic circuits will report `true`? \(T stands for `true`, and F stands for `false`.\)  
   1. ![](https://bjc.edc.org/bjc-r/img/6-computers/logic-gates-quiz-b.png)  
   2. ![](https://bjc.edc.org/bjc-r/img/6-computers/logic-gates-quiz-a.png)

* I only

* II only

* I and II
* Neither I nor II



[How do engineers draw logic gates?](https://bjc.edc.org/bjc-r/cur/programming/6-computers/1-abstraction/09-digital-logic-gates.html?topic=nyc_bjc%2F6-how-computers-work.topic#hint-target)

![](https://bjc.edc.org/bjc-r/img/6-computers/logic-gates-example-circuit.png "logic gate diagram of \(not and\) and \(or\)")

Engineers typically draw logic gates horizontally and use special shapes that represent each gate:

![](https://bjc.edc.org/bjc-r/img/6-computers/LogicGates_img/Gates/AND.png "AND-gate")

![](https://bjc.edc.org/bjc-r/img/6-computers/LogicGates_img/Gates/OR.png "OR-gate")

![](https://bjc.edc.org/bjc-r/img/6-computers/LogicGates_img/Gates/NOT.png "NOT-gate")

For example, engineers would draw the logic circuit shown at right like this:![](https://bjc.edc.org/bjc-r/img/6-computers/LogicGates_img/Circuits/notandandor.png "Engineer&apos;s version a logic gate with \(not and\) and \(or\)")Do an [image search for "logic gate diagrams"](https://www.google.com/search?q=logic+gate+diagrams&tbm=isch) to see more examples.

