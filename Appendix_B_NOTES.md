## What is this Appendix_B about ?
```
Many chapters of this book touch on the elements of discrete mathematics.
This appendix reviews more completely the notations, definitions, and elementary
properties of sets, relations, functions, graphs, and trees.
```

# Set
================================================
**assume intersection symbol is n and union symbol is u.**
(1) The set is a collection of distinguishable objects, called its members or elements.                            <br>
(2) We can describe a set by explicitly listing its members as a list inside braces: S = {1,2,3}                   <br>
(3) A set cannot contain the same object more than once, and its elements are not ordered.  
(4) Two sets A and B are equal, written A = B, if they contain the same elements: {1,2,3} = {2,3,1} = {3,2,1}  = {1,2,3,1}                                  <br> 
(5) A variation of a set, which can contain the same object more than once, is called a multiset: {1,2,3,1}
(6) empty set, set of integers, set of real numbers, set of natural numbers: all has special symbols (search them).
(7) If all the elements of a set A are contained in a set B, that is, if x is in A implies
    x is in B, then we write A is part of or equal to B and say that A is a **subset** of B.
(8) set A is a **proper subset** of B, then A is only part of B, but A is not equal to B.
(9) We sometimes define sets in terms of other sets. 
    For example, we can define the set of even integers by {x: x belons to Z(set of integers) and x/2 is an integer}. The
    colon in this notation is read “such that.”.
(10) Given two sets A and B, we can also define new sets by applying set operations:
     - The **intersection** of sets A and B is the set
        A intersects B => {x: x belongs to A and x belongs to B}.
     - The **union** of sets A and B is the set
        A unions B =>  {x: x belongs to A or x belongs to B}.
     - The **difference** between two sets A and B is the set
        A - B => {x: x belongs to A and x don't belongs to B}.
(11) 
Associative laws:
    A n (B n C) = (A n B) n C.
    A u (B u C) = (A u B) u C.
Distributive laws:
    A n (B u C) = (A n B) u (A n C).
    A u (B n C) = (A u B) n (A u C).
Absorption laws:
    A n (A u B) = A.
    A u (A n B) = A.
DeMorgan’s laws:
    A - (B n C) = (A - B) u (A - C).
    A - (B u C) = (A - B) n (A - C).
(12) All the sets are subsets of some larger set U called the universe: 
For example, if we are considering various sets made up only of integers,
the set Z of integers is an appropriate universe.
Given a universe U, we define the complement of a set A as A(dash) = U - A = {x: x belongs to U and don't belongs to A} 
- A u A(dash) = U.
- A n A(dash) = Fay(empty set).
- A(double dash) = A.




