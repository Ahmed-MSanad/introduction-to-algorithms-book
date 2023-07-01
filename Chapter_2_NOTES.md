# Chapter_2 NOTES
=================

```
2.1 Insertion sort 
2.2 Analyzing algorithms 
2.3 Designing algorithms 
```
## 2.1 Insertion sort
=====================
```
Input: A sequence of n numbers.
Output: A permutation (reordering) of the input sequence ascending or descnding

insertion sort is an efficient algorithm for **sorting a small number of elements**.

Insertion sort works the way many people sort a hand of playing cards.
We start with an empty left hand and the cards face down on the table.
We then remove one card at a time from the table and insert it into the correct position in the left hand.
To find the correct position for a card, we compare it with each of the cards already in the hand,
from right to left. At all times, the cards held in the left hand are sorted.

We state these properties of A[1 : j - 1] formally as a **loop invariant**:
At the start of each iteration of the for loop of the subarray
A[1 : j-1] consists of the elements originally in A[1 : j-1] but in sorted order.

We use loop invariants to help us understand why an algorithm is correct.

***Loop invariant:***
      is a condition that is true before and after each iteration of a loop in a computer program.
      In other words, it is a property that holds true for every iteration of a loop.
      Loop invariants are useful for proving the correctness of algorithms and are commonly used in formal methods.
      To establish a loop invariant, you need to identify a property that is true for the initial state of the loop
      and that is preserved by each iteration of the loop. Once you have established a loop invariant,
      you can use it to prove that the loop terminates correctly and produces the desired result.

      For example, consider the following code snippet that computes the factorial of a non-negative integer n:

factorial = 1
i = 1
while i <= n:
    factorial *= i
    i += 1

      A loop invariant for this code could be "factorial is equal to the product of the first i-1 positive integers."
      This is true before the loop starts (when i=1 and factorial=1) and is preserved by each iteration of the loop
      (since we multiply factorial by i in each iteration). Therefore, we can use this loop invariant to prove that
      the loop correctly computes the factorial of n.

We must show three things about a loop invariant:
**Initialization**: It is true prior to the first iteration of the loop.
**Maintenance**   : If it is true before an iteration of the loop, it remains true before the next iteration.
**Termination**   : When the loop terminates, the invariant gives us a useful property that helps show that
                    the algorithm is correct.

***Mathematical induction:***

Mathematical induction is a method of proving mathematical statements for all natural numbers
(i.e., integers greater than or equal to zero). It is based on the principle that if a statement is true
for a specific natural number, and if it can be shown that if the statement is true for some natural number k,
then it is also true for k+1, then the statement is true for all natural numbers greater than or equal to the starting number.

The process of mathematical induction involves two steps:
Base case: Prove that the statement is true for some specific natural number, usually 0 or 1.
Inductive step: Assume that the statement is true for some arbitrary natural number k,
and then prove that the statement is also true for k+1.

By doing so, we establish that the statement is true for all natural numbers greater than or equal to the base case.
For example, let's prove by mathematical induction that the sum of the first n natural numbers is n(n+1)/2:
Base case: For n=1, the sum of the first natural number is 1, and n(n+1)/2 = 1(1+1)/2 = 1, so the statement is true for n=1.
Inductive step: Assume that the statement is true for some arbitrary natural number k,
the sum of the first k natural numbers is k(k+1)/2. We want to prove that the statement is also true for k+1.
The sum of the first k+1 natural numbers is (k+1) + the sum of the first k natural numbers,
which is (k+1) + k(k+1)/2 = (k+1)(k+2)/2 = (k+1)((k+1)+1)/2. Therefore, the statement is true for k+1.
By the principle of mathematical induction, we can conclude that the statement is true for all natural numbers.




```
