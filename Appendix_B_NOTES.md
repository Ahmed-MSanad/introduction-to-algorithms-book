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
(6) empty set, set of integers, set of real numbers, set of natural numbers: all has special symbols (search them).<br>
    (Natural numbers are the non negative integers)<br><br>
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
    (A n B)(dash) = A(dash) u B(dash).<br><br>
    (A u B)(dash) = A(dash) n B(dash).<br><br>
    
(12) All the sets are subsets of some larger set U called the universe: <br><br>
For example, if we are considering various sets made up only of integers,<br><br>
the set Z of integers is an appropriate universe.<br><br>
Given a universe U, we define the complement of a set A as A(dash) = U - A = {x: x belongs to U and don't belongs to A} <br><br>
- A u A(dash) = U.<br><br>
- A n A(dash) = Fay(empty set).<br><br>
- A(double dash) = A.<br><br>

(13) Two sets A and B are **disjoint** if they have no elements in common ==> (A n B = FAY).<br><br>

(14) The number of elements in a set is the **cardinality (or size)** of the set, denoted |S|.<br>
     Two sets have the same cardinality if their elements can be put into a one-to-one correspondence.<br>
     The cardinality of the empty set is 0.<br>
     If the cardinality of a set is a natural number, we say the set is finite; otherwise, it is infinite.<br>
     For any two finite sets A and B, we have the identity |A U B| = |A| + |B| - |A n B| .<br><br>
    
(15) A finite set of n elements is sometimes called an **n-set**. A 1-set is called a
     **singleton**. A subset of k elements of a set is sometimes called a **k-subset**.<br><br>

(16) We denote the set of all subsets of a set S, including the empty set and S itself,<br>
     by 2<sup>|S|</sup> ; we call 2<sup>S</sup> **the power set of S** ====> For eg:<br>
     S = {a,b} ====> the size of the set of all subsets is 2<sup>set size</sup><br>
     which is 4 here ====> {{},{a},{b},{a,b}}<br>
     The **power set** of a finite set S has cardinality 2<sup>|S|</sup>.<br><br>

(17) An ordered pair of two elements a and b is denoted (a,b) and is defined formally
     as the set {a, {b, a}}.<br> 
     Thus, the ordered pair (a,b) is not the same as the ordered pair (b,a) ===> {b, {a, b}}.


(18) Cartesian product of 2 sets:
     For example {a,b} X {a,b,c} = {(a,a),(a,b),(a,c),(b,a),(b,b),(b,c)}. 
     When A and B are finite sets, the cardinality of their Cartesian product is
     |A X B| = |A| * |B|.
