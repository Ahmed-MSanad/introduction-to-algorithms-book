## What is this Appendix_B about ?
```
Many chapters of this book touch on the elements of discrete mathematics.
This appendix reviews more completely the notations, definitions, and elementary
properties of sets, relations, functions, graphs, and trees.
```

# Set
================================================<br>
**assume intersection symbol is n and union symbol is u.** <br><br>
(1) The set is a collection of distinguishable objects, called its members or elements.                            <br><br>
(2) We can describe a set by explicitly listing its members as a list inside braces: S = {1,2,3}                   <br><br>
(3) A set cannot contain the same object more than once, and its elements are not ordered.  <br><br>
(4) Two sets A and B are equal, written A = B, if they contain the same elements: {1,2,3} = {2,3,1} = {3,2,1}  = {1,2,3,1}                                  <br> <br>
(5) A variation of a set, which can contain the same object more than once, is called a multiset: {1,2,3,1}<br><br>
(6) empty set, set of integers, set of real numbers, set of natural numbers: all has special symbols (search them).<br><br>
(7) If all the elements of a set A are contained in a set B, that is, if x is in A implies<br><br>
    x is in B, then we write A is part of or equal to B and say that A is a **subset** of B.<br><br>
(8) set A is a **proper subset** of B, then A is only part of B, but A is not equal to B.<br><br>
(9) We sometimes define sets in terms of other sets. <br><br>
    For example, we can define the set of even integers by {x: x belons to Z(set of integers) and x/2 is an integer}. <br><br>
    The colon in this notation is read “such that.”.<br><br>
(10) Given two sets A and B, we can also define new sets by applying set operations:<br><br>
     - The **intersection** of sets A and B is the set<br><br>
        A intersects B => {x: x belongs to A and x belongs to B}.<br><br>
     - The **union** of sets A and B is the set<br><br><br>
        A unions B =>  {x: x belongs to A or x belongs to B}.<br><br>
     - The **difference** between two sets A and B is the set<br><br>
        A - B => {x: x belongs to A and x don't belongs to B}.<br><br>
(11) <br><br>
Associative laws:<br><br>
    A n (B n C) = (A n B) n C.<br><br>
    A u (B u C) = (A u B) u C.<br><br>
Distributive laws:<br><br>
    A n (B u C) = (A n B) u (A n C).<br><br>
    A u (B n C) = (A u B) n (A u C).<br><br>
Absorption laws:<br><br>
    A n (A u B) = A.<br><br>
    A u (A n B) = A.<br><br>
DeMorgan’s laws:<br><br>
    A - (B n C) = (A - B) u (A - C).<br><br>
    A - (B u C) = (A - B) n (A - C).<br><br>
(12) All the sets are subsets of some larger set U called the universe: <br><br>
For example, if we are considering various sets made up only of integers,<br><br>
the set Z of integers is an appropriate universe.<br><br>
Given a universe U, we define the complement of a set A as A(dash) = U - A = {x: x belongs to U and don't belongs to A} <br><br>
- A u A(dash) = U.<br><br>
- A n A(dash) = Fay(empty set).<br><br>
- A(double dash) = A.<br><br>



