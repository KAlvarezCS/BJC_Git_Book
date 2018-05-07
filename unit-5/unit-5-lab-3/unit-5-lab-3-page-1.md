# Comparing Algorithms

**In this lab,** you will learn that some ways to solve a problem are faster than others.

**On this page,** you will compare two algorithms for adding the numbers from 1 to an input number \(as shown below\).

![](https://bjc.edc.org/bjc-r/img/5-algorithms/sum-from-1-to-5-reporting.png "sum from 1 to \(5\) reporting 15")

#### Thinking Out Loud

Alphie and Betsy are creating algorithms that take a positive integer as input and report the sum of all integers from 1 to the input number, like this:   
![](https://bjc.edc.org/bjc-r/img/5-algorithms/sum-from-1-to-13-reporting.png "sum from 1 to \(13\) reporting 91")

Their two different approaches always give the same outputs for the same inputs. Alphie and Betsy are discussing their different approaches.

**Alphie:** I made two new blocks. First, I created a reporter to list of all the integers between and including two integers, and then I used `combine`to add up the list.

The ![](https://bjc.edc.org/bjc-r/img/blocks/combine.png "combine with\(\) items of \(\)")block takes an operation \(with\_two\_blank input slots\) and a list as input, and it reports a single result \(not a list\): the combination of the elements in the list when using the given operation. For example:  
![](https://bjc.edc.org/bjc-r/img/3-lists/combine-example-1.png "combine with \(\(\)+\(\)\) items of \(list {5,6,2,3}\) reporting 16")

Read this out loud as "combine the elements of the list {5, 6, 2, 3} with addition."

You choose the operation, and `combine`performs that operation by \_combining \_all the items in the input list and then reports the result. Notice that the function used to \_combine \_the list items always has two blank input slots. Both `map`and `keep`only need one blank in their input function, but with `combine`, two are required.

`Combine`is a _higher order function_. This means that it is a function that takes a function as input. You've seen several higher order functions already: `for each`\(in [Unit 2 Lab 2](https://bjc.edc.org/bjc-r/cur/programming/2-complexity/2-data-structures-art/1-the-for-each-block.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment)\), `keep`\(in [Unit 2 Lab 3](https://bjc.edc.org/bjc-r/cur/programming/2-complexity/3-predicates/2-keeping-list-items.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment)\), and `map`\(in [Unit 3 Lab 1](https://bjc.edc.org/bjc-r/cur/programming/3-lists/1-introduction-to-lists/4-mapping-over-list.html?topic=nyc_bjc%2F3-lists.topic&course=bjc4nyc.html&novideo&noassignment)\).

Unlike `map`and `keep,` `combine`is mostly used with one of \_only these six \_functions:

![](https://bjc.edc.org/bjc-r/img/3-lists/plus.png "+")![](https://bjc.edc.org/bjc-r/img/3-lists/times.png "×")![](https://bjc.edc.org/bjc-r/img/3-lists/and-block.png "and")![](https://bjc.edc.org/bjc-r/img/3-lists/or-block.png "or")![](https://bjc.edc.org/bjc-r/img/3-lists/join.png "join")![](https://bjc.edc.org/bjc-r/img/3-lists/join-words.png "join words")  
Among blocks you might write yourself, there are only two likely candidates:![](https://bjc.edc.org/bjc-r/img/3-lists/max.png "max")![](https://bjc.edc.org/bjc-r/img/3-lists/min.png "min")

[Why so few?](https://bjc.edc.org/bjc-r/cur/programming/5-algorithms/3-timing-experiments/1-comparing-algorithms.html?topic=nyc_bjc%2F5-algorithms.topic&course=bjc4nyc.html&novideo&noassignment#hint-3)

_Alphie shows his work: _![](https://bjc.edc.org/bjc-r/img/5-algorithms/list-from-1-to-7-reporting.png "list from \(1\) to \(7\) reporting the list{1,2,3,4,5,6,7")

![](https://bjc.edc.org/bjc-r/img/5-algorithms/sum-of-definition.png "sum of \(inputList\){report\(combine with\(\(\)+\(\)\) items of \(inputList\)\)}")

**Betsy:** Great! I think we can do it another way too.

**Alphie:** Cool. How?

**Betsy:** I was thinking about adding, and I noticed that 1 + 13 = 14 and 2 + 12 = 14 and 3 + 11 = 14...

**Alphie:** So, you added up fourteens?

**Betsy:** Yeah. I wrote down the list from 1 to 13 and then I wrote the same numbers in reverse order—right under my first list, like this:

1    2    3    4    5    6    7    8    9    10    11    12    13

13    12    11    10    9    8    7    6    5    4    3    2    1

**Betsy:** Then I added down and got thirteen fourteens:

1    2    3    4    5    6    7    8    9    10    11    12    13

* 13    12    11    10    9    8    7    6    5    4    3    2    1

14    14    14    14    14    14    14    14    14    14    14    14    14

**Betsy:** And 13 times 14 is 182...

**Alphie:** But the answer is 91.

**Betsy:** Right. I added each number in twice, so the answer is half of 182, which is 91.

Betsy writes \frac{13\* 14}{2}  
 = 91.

**Alphie:** Oh, and if you wanted to add the numbers from 1 to 50, you'd multiply 50 and 51 and divide by 2 to get \(Alphie calculates\) 1275.

Alphie writes \frac{50 \* 51}{2} = 1275.

**Betsy:** \(smiling\) So in general to add the numbers between 1 and some number, n, you multiply the input number by one more than the input number and then you divide the result by 2...

