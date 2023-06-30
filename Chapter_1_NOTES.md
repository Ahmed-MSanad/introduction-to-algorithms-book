# The Role of Algorithms in Computing

## What are algorithms?
	- computational procedure that takes some value, or set of values, 	
    as input and produces some value, or set of values, as output,
    where The statement of the problem specifies the desired input/output relationship.

## Why is the study of algorithms worthwhile? 
	- Because many programs use it as an intermediate step, sorting is a fundamental operation in computer science.

## Which algorithm is best for the Sorting Problem? 
  - depends on—among other factors — the number of items to be sorted, the extent to which the items are already somewhat sorted,
    possible restrictions on the item values, the architecture of the computer, and the kind of storage devices to be used.

## When the algorithm is said to be correct?
  - An algorithm is said to be correct if, for every input instance, it halts with the correct output.

## What is the role of algorithms relative to other technologies used in computers?
	- Sorting is by no means the only computational problem for which algorithms have been developed.

## what is an example for using algoritms daily?
  - Electronic commerce enables goods and services to be negotiated and exchanged electronically, and it depends on the privacy of personal information
    such as credit card numbers, passwords, and bank statements.
    The core technologies used in electronic commerce include public-key cryptography and digital signatures (covered in Chapter 31),
    which are based on numerical algorithms and number theory.

## Subsequence:
===============
- A subsequence of X is just X with some (or possibly all or none) of its elements removed.
  subsequence of {A; B; C; D; E; F; G} would be {B; C; E; G}.

- If X has n symbols X ={A,E,...n} , then X has 2^n possible subsequences.

- Empty subsequence is the common subsequence between all sequences.

- n of elements has n! orders(!n permutation):
  for ex: abc has 3! permutations --> abc, acb, bac, bca, cab ,cba.

- The factorial function grows faster than an exponential function:
  factorial function takes more time than exponential function at large number inputs.

## Data structure:
   ===============
- A data structure is a way to store and organize data in order to facilitate access and modifications.

- No single data structure works well for all purposes, and so it is important to know the strengths and limitations of several of them.

- Our usual measure of efficiency is speed, i.e., how long an algorithm takes to produce its result.

- In order to perform more computations per second, therefore, chips are being designed to contain not just one but several processing “cores.”.

-  Chapter 27 presents a model for “multithreaded” algorithms, which take advantage of multiple cores.
   This model has advantages from a theoretical standpoint, and it forms the basis of several successful computer programs, including a championship chess program.

## Algorithms as a technology
   ==========================

-	**if the computers were very fast and the memory was free that wouldn't eleminate the study of algorithms**.

- computers may be fast, but they are not infinitely fast, And memory may be inexpensive, but it is not free,
  So Computing time is therefore a bounded resource, and so is space in memory, so You should use these resources wisely.

-	**The same problem may have different algorithms with different efficiency in memory space and performance**:
```
For eg:
    Insertion sort, takes time roughly equal to c<sub>1</sub>n<sup>2</sup> to sort n items, where c<sub>1</sub> is a constant that does not depend on n.
That is, it takes time roughly proportional to n<sup>2</sup>.
The second, Merge sort, takes time roughly equal to c<sub>2</sub> n lg(n),
where lg(n) stands for log2(n) and c<sub>2</sub> is another constant that also does not depend on n.

Although insertion sort usually runs faster than merge sort for small input sizes,
once the input size n becomes large enough, merge sort’s advantage of lg(n) vs n will more than compensate for the difference in constant factors. 

    let us pit a faster computer (computer A) running insertion sort against a slower computer (computer B) running merge sort.
They each must sort an array of 10 million numbers. Suppose that computer A executes 10 billion instructions per second
and computer B executes only 10 million instructions per second, so that computer A is 1000 times faster than computer B.
To make the difference even more dramatic, suppose that the world’s craftiest programmer codes insertion sort in machine language for computer A,
and the resulting code requires 2n<sup>2</sup> instructions to sort n numbers. Suppose further that just an average programmer implements merge sort,
using a high level language with an inefficient compiler, with the resulting code taking 50n*lg(n) instructions. To sort 10 million numbers:
	Computer A takes: 
(2*(10^7)^2 instructions) / (10^10 instructions/second) = 20,000 seconds (more than 5.5 hours).
	Computer B takes:
(50*(10^7)*lg(10^7) instructions) / (10^7 instructions/second)= 1163 seconds (more than 20 minutes).

By using an algorithm whose running time grows more slowly, even with a poor compiler,
computer B runs more than 17 times faster than computer A !.
The advantage of merge sort is even more pronounced when we sort 100 million numbers:
where insertion sort takes more than 23 days, merge sort takes under four hours.
**In general, as the problem size increases, so does the relative advantage of merge sort.**

So, system performance depends on choosing efficient algorithms as much as on choosing fast hardware

**Algorithms are at the core of most technologies used in contemporary computers.**
The hardware design used algorithms.
The design of any GUI relies on algorithms.
Routing in networks relies heavily on algorithms.

===================================================================================================================================================
