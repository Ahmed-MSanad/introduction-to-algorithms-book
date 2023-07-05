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

When the loop is a for loop, the moment at which we check the loop invariant just prior to the first
iteration is immediately after the initial assignment to the loop-counter variable and just before the
first test in the loop header.

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
## 2.2 Analyzing algorithms
===========================
```
      Analyzing algorithms: predicting the resources that an algorithm whould need.
                            most often needed resources are the computational time and memory.

      What is The RAM model ??
      ========================
      The RAM model, which stands for Random Access Machine model,
      is a theoretical model of a computer used in computer science and computational complexity theory.
      The RAM model is a simple but powerful model that is used to investigate the computational complexity
      of algorithms and problems.

      In the RAM model, a computer is represented as a sequence of memory cells, each of which can store
      an integer value. The model has a finite number of registers, which are used to store temporary values
      during computation.
      The RAM model also has a central processing unit (CPU) that can perform simple operations on memory
      values, such as reading and writing values, arithmetic operations
      (addition, subtraction, multiplication, and division), and conditional branching.

      The RAM model is useful because it provides a simple and flexible abstraction of a computer
      that can be used to reason about the time and space complexity of algorithms.
      By counting the number of operations performed by an algorithm in the RAM model,
      we can estimate its running time, and by counting the number of memory cells it uses,
      we can estimate its space requirements.

      is exponentiation a constanttime instruction? In the general case, no.
      “shift left” instruction, which in constant time shifts the bits of an integer by k positions to the left
```
```
Analysis of insertion sort
==========================
    - The time taken by an algorithm grows with the size of the input,
      so it is traditional to describe the running time of a program as
      a function of the size of its input.

      Also, depending on how nearly sorted they already are.

    - The running time of an algorithm on a particular input is the
      number of primitive operations or “steps” executed.

    - The running time of the algorithm is the sum of running times for each statement executed
      a statement that takes ci steps to execute and executes n times will
      contribute c<sub>i</sub>*n to the total running time.

NOTE: A statement that references m words of memory and is executed n times
      does not necessarily reference mn distinct words of memory

      To compute T(n), the running time of INSERTION-SORT on an input of n values,
      we sum the products of the cost and times.

      Even for inputs of a given size, an algorithm’s running time may depend on
      which input of that size is given. For example, in INSERTION-SORT, the best
      case occurs if the array is already sorted.

      If the array is in reverse order—then,it is the worst case.

NOTE:
      Σ<sub>2</sub> <sup>n</sup> j = (n*(n+1)/2) -1
AND
      Σ<sub>2</sub> <sup>n</sup> (j-1) = (n*(n-1)/2)

      ========================
      Summations(Appendix A):
      ========================
      **Summation formulas and properties**:
      --------------------------------------
      a1 + a2 + a3 + a4 + ..... + an = Σ<sub>k = 1</sub> <sup>n</sup> a<sub>k</sub>

      a1 + a2 + a3 + a4 + ........   = Σ<sub>k = 1</sub> <sup>∞</sup> a<sub>k</sub> =
      lim<sub> n -> ∞ </sub> Σ<sub>k = 1</sub> <sup>n</sup> a<sub>k</sub>
      If the limit does not exist, the series diverges; otherwise, it converges.

The terms of a convergent series cannot always be added in any order. We can, however,
rearrange the terms of an absolutely convergent series, that is, a series
Σ<sub>k = 1</sub> <sup>∞</sup> a<sub>k</sub>for which the series
Σ<sub>k = 1</sub> <sup>∞</sup> |a<sub>k</sub>| also converges.

A series can either converge or diverge, depending on whether the sum of the terms
in the sequence approaches a finite value or not.

A series is said to converge if the sum of its terms approaches a finite limit as the number
of terms in the series increases. In other words, if the value of the sum of the terms becomes
arbitrarily close to a fixed value as more and more terms are added, the series is said to converge.

The geometric series is an example of a convergent series. It has the general form: (a + ar + ar^2 + ar^3 + ...)
where "a" is the first term, "r" is the common ratio between consecutive terms, and the series continues
indefinitely. The geometric series converges if and only if the absolute value of the common ratio "r"
is less than 1. In this case, the **sum of the series is given by: (S = a / (1 - r)).**
For example, the series 1 + 1/2 + 1/4 + 1/8 + ... is a geometric series with "a" = 1 and "r" = 1/2.
Since the absolute value of the common ratio is less than 1, the series converges, and its sum is:
(S = a / (1 - r) = 1 / (1 - 1/2) = 2) So the sum of the series is 2.

A series is said to diverge if the sum of its terms does not approach a finite limit as the number of
terms in the series increases. In other words, if the sum of the terms grows without bound as more and
more terms are added, the series is said to diverge.

The harmonic series is an example of a divergent series. It has the general form: (1 + 1/2 + 1/3 + 1/4 + ...)
where the series continues indefinitely. The harmonic series is a famous example of a divergent series,
and it diverges to infinity. This means that as the number of terms in the series increases, the sum of
the terms grows without bound, and there is no finite limit that the sum approaches.

Whether a series converges or diverges depends on the behavior of its terms and the particular method
used to add them up. There are many different tests and criteria that can be used to determine the
convergence or divergence of a series, such as the ratio test, the comparison test, and the integral
test, among others.

      Linearity property:
      -------------------
      Σ<sub>k = 1</sub> (C*a<sub>k</sub> + b<sub>k</sub>) <sup>n</sup> =
      (C * Σ<sub>k = 1</sub> a<sub>k</sub> <sup>n</sup>) + (Σ<sub>k = 1</sub> b<sub>k</sub> <sup>n</sup>)

      The linearity property also applies to infinite convergent series.

      Arithmetic series:
      ------------------
      Σ<sub>k = 1</sub> k <sup>n</sup> = 1 + 2 + ... + n (is an arithmetic series and has the value:)
**(1) Σ<sub>k = 1</sub> <sup>n</sup> k = n*(n+1)/2  **
**(2) Σ<sub>k = 1</sub> <sup>n</sup> k<sup>2</sup> = n*(n+1)*(2n+1)/6  **
**(3) Σ<sub>k = 1</sub> <sup>n</sup> k<sup>3</sup> = n<sup>2</sup>*(n+1)<sup>2</sup>/4  **

      Geometric series:
      -----------------
      - Geometric series For real x != 1, the summation: (x can be (-3) or 3 or 3.3 but not 1)
      Σ<sub>k = 0</sub> <sup>n</sup> x<sup>k</sup> =  1 + x + .... + x(<sup>n</sup>)
**(4) Σ<sub>k = 0</sub> <sup>n</sup> X<sup>k</sup> = (X(<sup>n+1</sup>) - 1) / (X - 1)**


      - When the summation is infinite and |x| < 1, we have the infinite decreasing geometric series:
**(5) Σ<sub>k = 0</sub> <sup>∞</sup> X<sub>k</sub> = 1/(1-X)**


      Harmonic series:
      -----------------
      For positive integers n, the nth harmonic number is:
      H<sub>n</sub> = 1 + (1/2) + (1/3) + .... + (1/n) = Σ<sub>k = 1</sub> <sup>n</sup> 1/k

By integrating or differentiating the formulas above, additional formulas arise. For
example, by differentiating both sides of the infinite geometric series (A.6) and
multiplying by x, we get:
**(6) Σ<sub>k = 0</sub> <sup>∞</sup> kX<sub>k</sub> = X/(1-X)<sup>2</sup>** , for |x| < 1.

      Telescoping series:
      -------------------
      For any sequence a0,a1,....,an,
**(7) Σ<sub>k = 1</sub> <sup>n</sup> (a<sub>k</sub> - a<sub>k-1</sub>) = an - a0**

**(8) Σ<sub>k = 0</sub> <sup>n-1</sup> (a<sub>k</sub> - a<sub>k+1</sub>) = a0 - an**



```
