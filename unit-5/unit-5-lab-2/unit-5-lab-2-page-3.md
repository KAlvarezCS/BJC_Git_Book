# Disease Spread Project

**On this page,**you will model the spread of a disease in a population.

![](https://bjc.edc.org/bjc-r/img/5-algorithms/img_disease-spread/disease-spread.gif)

Suppose you are a medical researcher at the Centers for Disease Control \(CDC\) and would like to understand the factors that contribute to the spreading of a new disease across a population. In particular, you would like to know the effect of population size on the rate at which the disease spreads.

#### For You To Do

1. What would be a sensible hypothesis on how population size relates to the rate of the spread of the disease?

You may not have enough data from actual outbreaks to test your hypothesis and make any meaningful conclusions, and it would be unethical to induce the disease in some population in order to gather new data. In this situation, a simulation would be the best option to generate data in order to test your hypotheses without the constraints of time, cost, and ethics.

In this project, you will simulate the spread of a disease within a small population and explore the effects of variables such as population size and speed of human interaction on the spread of disease.

#### For You To Do

1. Play with the Snap! file [linked here](https://bjc.edc.org/bjc-r/cur/programming/5-algorithms/2-simulation/3c-disease-spread-interactive.html) to get a feel for the simulation program you will be writing.
2. Your code should:

   1. Ask the user for 3 inputs: the population size, the percentage of the population initially infected, and the speed at which the people should be moving.
   2. Create a single person sprite and use the `create a clone of myself`block to generate a population with the size inputted by the user.
   3. Make the user-specified percentage of the population sick and the rest of the population healthy. 
   4. Have a timer measure the duration of the outbreak \(until everyone is infected\).
   5. Have the people move around with the constant speed inputted by the user.
   6. Make sure that when a healthy person collides with a sick person, they also becomes sick.
   7. Stop the animations and the timer when the entire population becomes sick.

3. Discuss how your simulation may be similar to and different from a real life disease outbreak. Identify the simplifying assumptions you made in this simulation.

4. Study the relationships between the various variables in the simulation:

   1. the population size\(N\)

   2. the percentage of the population initially sick \(P\)

   3. the speed at which the people move \(v, for velocity\)

   4. time elapsed until the entire procedure becomes sick\(T\)

   5. Start with a hypothesis predicting the pattern that will emerge in the simulations.

      1. For example, to understand the effect of population size \(N\) on the time it takes the disease to fully spread \(T\), fix P=10 and v=2, and use your simulation to make a chart of T \(on the vertical axes\) as a function of N \(on the horizontal axis\) in increments of 10 for N.

To ensure reliability, you may need to run each particular simulation \(for N=10, 20, 30, ... , 100\) several times and take an average. Create a visual graph of your findings. Do you see any patterns? Do they agree with your hypothesis? How can you study the effects of other variables with your simulations?

#### Take It Further

1. Here are some possible variations on this simulation that could make it more realistic. Save a copy of your work before exploring one or more of these variations:
   1. Give a probability to being infected when a healthy person encounters a sick person. 
   2. Let the infected people slow down in speed. 
   3. Let the infected people heal either with time or by a probability.
   4. Let those infected and then healed become immune to the sickness.
   5. Introduce doctor sprites that heal the sick upon encounter.
   6. At the start of simulation, introduce vaccination to a given percentage of the population.
2. Design and implement a predator-prey simulation in Snap!. For example, you could model an environment with wolf and deer populations where the wolf prey on the deer. What are some parameters you need to incorporate into your model so you can simulate realistic fluctuations in the populations of predator and prey?
3. Imagine you work at a bank that wants to minimize customer wait times in line. The bank is considering two alternatives:
   1. a single line where the customers stand in arrival order and wait for the next available teller, or
   2. separate lines for each teller.

Design and implement two simulations in Snap! to help the bank determine the average wait time for customers in each scenario in order to choose the best option.

![](https://bjc.edc.org/bjc-r/img/5-algorithms/img_disease-spread/single-queue.png "Single queue")![](https://bjc.edc.org/bjc-r/img/5-algorithms/img_disease-spread/multiple-queues.png "Multiple queues")

