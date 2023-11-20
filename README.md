# Data Analysis
This is the repository for the data analysis module.

The purpose of the repo is to store all work relating to this module

1. Collatz Conjecture

The Collatz conjecture is a famous unsolved problem in mathematics. The problem is to prove that if you start with any positive integer x and repeatedly apply the function f(x) below, you always get stuck in the repeating sequence 1, 4, 2, 1, 4, 2, . .

The code first defines 'f(x)' a function that takes a single integer x as its input. It implements the Collatz function, which checks if x is even, and if so, it returns x divided by 2; otherwise, it returns 3x + 1. This function is used to calculate the next term in the Collatz sequence.

The code then goes on to define 'verify_collatz(limit) that verifies the Collatz Conjecture for positive integers from 1 to the specified limit.

The function starts by iterating through integers from 1 to 'limit'.

Inside the loop, it initialises a variable x with the current value of i. This x will be used to calculate the Collatz sequence for the current integer i.

It then enters a while loop that continues until x reaches 1. In each iteration of the while loop, the Collatz function f(x) is applied to update the value of x.

The code checks if x reaches 1. If x equals 1, it means that the Collatz Conjecture holds for the current integer i, and the loop can break.

If x is not equal to 1 after the loop, it means that the Collatz Conjecture was not confirmed for the current integer i. In this case, it prints a message indicating that the conjecture is not true for that integer and exits the function using return.

After checking all integers in the range, if none of them triggered the "not true" condition, it prints a message confirming that the Collatz Conjecture is true for all numbers up to the specified limit.



2. Pengiun Dataset Variables

Give an overview of the famous penguins data set,explaining the types of variables it contains. Suggest the types of variables that should be used to model them in Python, explaining your rationale.

The tasks first outlines the data with the .info and .describe method showing the stats and data types.

It then briefly describes the most relevant variable to suit each element of of the data



3. Numpy Probability Distribution

For each of the variables in the penguins data set, suggest what probability distribution from the numpy random distributions list is the most appropriate to model the variable.

Many of the variables can be seen to Be normally distributed, upon examining the shapes of the plotted distributions, it was observed that a significant portion of the variables in the dataset display patterns reminiscent of a normal distribution. A normal distribution is characterized by a symmetric, bell-shaped curve.




4. Entropy

Shannon entropy, named after Claude Shannon, is a measure of the amount of uncertainty or information content associated with a random variable. In information theory, it is used to quantify the average amount of surprise or unpredictability inherent in a set of possible outcomes.

The code starts by importing the necessary libraries. matplotlib.pyplot is used for plotting, and numpy is used for numerical operations.

We follow this by defining a function named entropy that takes a probability p as an argument and calculates the Shannon entropy using the provided probabilities for the outcomes (0, 1, and 2 heads).

We generates a range of probability values p_values from 0 to 1 inclusive using 'numpy.linspace'. In this case, it creates 100 equally spaced values between 0 and 1.

Using a list comprehension to we calculate the Shannon entropy for each probability in p_values by calling the entropy function.

The code uses matplotlib.pyplot to create a plot. It plots the calculated entropy values against the probability values. It also adds labels, a title, a legend

By: Anthony Mc Garry