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
   2. Create a single person sprite and use the `create a clone of myself `block to generate a population with the size inputted by the user.
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



