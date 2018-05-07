# Timing Reporters

**On this page,** you will create an _algorithm timer_ to help you compare the efficiency of algorithms.

Snap! allows us to report how long a program takes to finish.

#### For You To Do

1. In the "Sensing" palette, look for the for the `current (`date`)`reporter. Drag it into the scripting area. From its input menu, select time in milliseconds.
2. Click the block several times. Note the results. 

This block can be used to time how long a reporter takes to output. Here’s an algorithm:

* **Step 1. **Create a variable start time and set it to the current time.
* **Step 2. **Call the reporter that you're trying to time. Ignore the result.
* **Step 3. **When the reporter finishes, get the current time and subtract start time from it.

#### For You To Do

1. Download [this library](https://bjc.edc.org/bjc-r/prog/5-algorithms/U5L3functiontimer.xml) and drag the file into your Snap! application so that it gets imported. A block called time function is provided that takes any reporter \(with its inputs filled in\), computes the result, but reports how long it took to do the computation. The answer will be in milliseconds. Take a minute to review the code in time function.
2. Open the project **U5L3-ReporterTimer** that you saved on page 1 of this lab. Drag in the **U5L3functiontimer** library that you just downloaded.
   ![](https://bjc.edc.org/bjc-r/img/5-algorithms/timereport.png "time function \(list from \(1\) through \(1000\)\) reporting 27")You can replace the `list from `block with any reporter. You can edit `time function `to see how it works. In this example, it took 27 milliseconds to compute the list of integers from 1 to 1000. \(The actual number will depend on how fast your computer is.\)

#### For You To Do

1. Use `time function `to compare Alphie and Betsy's ways of adding the integers from 1 to _n_. Try it with several different large numbers to see just how different the algorithms are in terms of the time it takes to compute their outputs. ![](https://bjc.edc.org/bjc-r/img/5-algorithms/time-function-betsy-way-2000-reporting.png "time function \(betsy way \(2000\)\) reporting 1")![](https://bjc.edc.org/bjc-r/img/5-algorithms/time-function-alphie-way-2000-reporting.png "time function \(alphie way \(2000\)\) reporting 187")

Alphie and Betsy’s algorithms solve the same problem but are quite different in efficiency. Imagine the difference when adding the integers from 1 to 1,000,000…

The efficiency of an algorithm can make a huge difference. Sometimes, an efficient algorithm is necessary to solve larger instances of a problem.

1. In Lab 1 you built two reporters that output the position of an element in a list. The reporter position of \_\_ in unsorted list works for any list as a linear search, checking element-by-element until it finds a match \(or gets to the end and reports "Not In List"\). The reporter position of \_\_ in sorted list works on sorted lists as a binary search algorithm. So, both will work on sorted lists. Compare them for some long sorted lists and make a table of your findings.	You may have to use very large lists, say 1000 or 2000 items, to get meaningful results. Is the other algorithm ever faster? Which algorithm is faster?
2. Throughout this course, you've programmed many algorithms. Try timing them! Test your favorite algorithms, such as:
   1. Creating a list of numbers
   2. Testing a list to see if the elements are distinct
   3. Adding 1 to a number
      Number guessing games

Time your algorithms for varying size inputs and describe the different behaviors you see. Again, use large inputs for meaningful results.

Save this as "U5L3-timer"

  


