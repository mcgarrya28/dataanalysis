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


2.
3.
4.

By: Anthony Mc Garry