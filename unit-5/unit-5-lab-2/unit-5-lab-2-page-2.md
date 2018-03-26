# Flipping a Coin Project

**On this page, **you will learn how to model the tossing of a coin.

When you toss a coin, you assume that the chances of getting a head or a tail are equal. But if you toss a coin 10 times, you know that you might not get exactly 5 heads and 5 tails. What percent of the time do you get that result? Is it different if you tossed the coin 100 times? 1000 times? It is tiresome and impractical to toss a coin hundreds or thousands of times, but it is possible to explore these questions with a _simulation_. In this project you will simulate the flipping of a coin and test your hypotheses.

#### For You To Do

1. Play with the Snap_! _file [linked here](https://bjc.edc.org/bjc-r/cur/programming/5-algorithms/2-simulation/2c-flipping-a-coin-interactive.html) to see a possible implementation of what you are trying to achieve with your the simulation. Before starting to program in Snap_!_, plan out the sequence of events that will occur in your simulation:

   1. When and how will the user input the desired number of flips?
   2. How will the program simulate the coin toss mathematically?
   3. How will the program simulate the coin toss visually? What will the user see?
   4. What are the variables to create in order to keep track of the important parameters in the simulation? When should these be initialized? When should they be updated?

   Before building your algorithm in Snap!, work through your pseudocode with a few example inputs until you have debugged it as much as possible.

2. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:https://bjc.edc.org/bjc-r/prog/5-algorithms/U5L6-coinflip-student.xml) Use this file to build a Snap! program to run the simulation. It includes a sprite named "Coin" with two costumes \(Heads and Tails\) and a sound file \("Pop"\) to get you started in your work. Do this on your own but if you get stuck, you can visit [this page](https://bjc.edc.org/bjc-r/cur/programming/5-algorithms/2-simulation/2b-flipping-a-coin-hints.html) for hints.

3. If you toss a coin 10 times and repeat this 10-toss trial many times, how likely do you think each possible percentage of heads will be across all trials? Here are two examples of possible distributions of the percentage of heads across many 10-toss trials. Which shape of a histogram do you expect in your class simulations? ![](https://bjc.edc.org/bjc-r/img/5-algorithms/img_flipping-a-coin/UniformDistribution.png "Histogram of \(almost\) uniform distribution")

   ![](https://bjc.edc.org/bjc-r/img/5-algorithms/img_flipping-a-coin/NormalDistribution.png "Histogram of \(almost\) normal distribution")

4. Use your program to simulate tossing a coin 10 times and record the percentage of heads that is observed. Combine your results as a class to graphically display the distribution of this percentage with a histogram. Are the results in accordance with what you predicted?

5. If you were to repeat the above experiment but this time tossing the coin 100 times \(doing 100-toss trials\), how would you expect your histogram of percentage of heads to change? Test your hypothesis using your simulation and combining the results as a class.

#### Take It Further

1. Save a copy of your work and create code that simulates an _unfair_ coin. For example, instead of the odds of heads vs. tails being 50:50, the respective likelihoods could be 75:25. Your program should ask the user to input what this bias should be.
2. On paper, study the mathematics behind tossing a coin a number of times. For example, in 3 tosses of a coin, what is the theoretical likelihood of getting:

   1. exactly 3 heads

   2. exactly 2 heads

   3. exactly 1 head

   4. no heads

      1. Hint: you can do this most easily by first listing all the possible outcomes: HHH, HHT, etc.

1. Create a Snap! program to simulate the rolling of a single die. Then extend your program to simulate the rolling of two dice. Create a variable to report the sum of the two dice. Predict which sum will occur most often if you rolled the dice 1000 times. Use your simulation to test your hypothesis.



