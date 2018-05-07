# Classifying Algorithms

**On this page,** you will learn that some correct algorithms take too long to be practical.

#### For You To Do

1. If it isn't already open, load the project U5L3-timer from the previous page, and experiment with `time function`
   on algorithms you've built \(such as `alphie way`,`betsy way`,`find in unsorted list`,`find in sorted list`, and any others you have handy\). What happens to the running time if you double the size of the input?

   1. You can classify algorithms by the amount of time they take to run.

2. [![](https://bjc.edc.org/bjc-r/img/icons/load-save.png "Click here to load this file. Then save it to your Snap! account.")](http://snap.berkeley.edu/snapsource/snap.html#open:https://bjc.edc.org/bjc-r/prog/5-algorithms/U5L3-listfrom.xml)

   1. Use the ![](https://bjc.edc.org/bjc-r/img/5-algorithms/listfrom.png "list from \(\) to \(\)") block to build the following two blocks in Snap_!_. Then, determine which block's algorithm can be executed in a reasonable time, and which cannot.

      1. ![](https://bjc.edc.org/bjc-r/img/5-algorithms/1000numbers.png "1000 numbers starting from \(\)")
      2. ![](https://bjc.edc.org/bjc-r/img/5-algorithms/digitnumbers.png "all \(\) digit numbers")

   2. The list of 2-digit numbers goes from 10 to 99. There's a math operations block that can give you powers of 10.

To classify an algorithm, look at the number of steps it takes to complete the algorithm, compared to the size of the input.

* **Reasonable Time:**
  * Some algorithms always take the same number of steps, even as the input grows. These algorithms take constant time.
  * Some algorithms take a number of steps proportional to the input size. \(If you double the size of the input, the number of steps doubles also.\) These algorithms take linear time.
  * If the number of steps is less than or equal to a polynomial function of the size of the input \(including constant, linear, and quadratic functions, etc.\), then the algorithm takes polynomial time and is reasonable.

Polynomial time can be further broken down, depending on the polynomial. Algorithms whose runtime is about n^2 run in quadratic time. \(If you double the size of the input, that quadruples the number of steps.\) It's rare in practice to find polynomial time algorithms that take more than cubic \(n^3\) time.

* **Unreasonable Time:**
  * If the number of steps is an exponential function of the size of the input \(or another function larger than any polynomial\), we say that the algorithm takes an unreasonable amount of time. For an algorithm that takes 2^n time, just adding 1 to the input size \(n\) doubles the number of steps!

These categories say that an algorithm takes at most so much time. So, for example, a constant-time algorithm is also a linear-time algorithm, and also a polynomial-time algorithm, and also an exponential-time algorithm. But usually if someone says an algorithm "takes linear time," they mean that it takes more than constant time but not more than linear time.

It's important to recognize that an unreasonable-time algorithm **still solves a problem correctly.** Unreasonable-time algorithms can sometimes be replaced by heuristics, simpler algorithms that may not succeed in solving the problem exactly but give a good enough approximation.

#### For You To Do

1. Look at some algorithms you've built. Determine whether each algorithm runs in constant time, linear time, polynomial time, or unreasonable time.

#### If There Is Time...

1. For Alphie's way of adding integers, create a graph with the number of integers on the horizontal and the runtime on the vertical. Generate data for the graph by running `time function `with large inputs to `Alphie's way `\(say, multiples of 100\). Then use the techniques from Lab 2 to plot the graph.
2. What information does this graph tell you about Alphie's algorithm? Is it constant time, linear time, other polynomial time, or is it unreasonable time?

#### For You To Do

1. This question is similar to those you will see on the AP CSP exam.

| Task | Small Town \(population 1,000\) | Mid-Sized Town \(population 10,000\) | Large town \(population 1000,000\) |
| :--- | :--- | :--- | :--- |
| Entering Data | 2 hours | 20 hours | 200 hours |
| Backing up Data | 0.5 hours | 5 hours  | 50 hours |
| Searching through data | 5 hours | 15 hours | 25 hours |
| Sorting Data | 0.01 hour | 1 hour | 100 hours |

Based on the information in the table, which of the following tasks is likely to take the **longest** amount of time when scaled up for a city of population 1,000,000.

* Entering Data
* Sorting Data
* Backing Up Data
* Searching through data



