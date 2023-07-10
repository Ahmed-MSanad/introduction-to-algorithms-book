## A.1-1
========<br>
Σ<sub>k = 1</sub><sup>n</sup> (2k - 1) = ( 2*Σ<sub>k = 1</sub><sup>n</sup> k ) - (Σ<sub>k = 1</sub><sup>n</sup> 1) <br>
        = 2*(n*(n+1)/2) - n = n*n + n - n = n*n = n<sup>2</sup> .

## A.1-2
========<br>
Σ<sub>k = 1</sub><sup>n</sup> (1/(2k - 1)) =  (substitute) <br>
{1 + 1/3 + 1/5 + 1/7 + .....}            = <br>
{1 + 1/2 + 1/3 + 1/4 + .....} - {1/2 + 1/4 + 1/6 + ....} = <br>
{1 + 1/2 + 1/3 + 1/4 + .....} - 1/2 * {1 + 1/2 + 1/3 + ....} =  -------->> (3)<br>
From the harmonic series: Σ<sub>k = 1</sub><sup>n</sup> (1/k) = ln(n) + O(1). So, <br>
From (3): <br>
ln(n) + O(1)                  - 1/2 * (ln(n) + O(1))         = <br>
ln(n) - ln(n)/2 + O(1) - O(1)/2                              = <br>
ln(n)/2 + O(1)                                               =  (Why O(1) ? consider it as constant so 1/2 won't be issue)<br>
ln(n<sup>1/2</sup>) + O(1)                                   = <br>
**ln(sqrt(n)) + O(1)**

## A.1-3
========<br>

From the Geometric series : Σ<sub>k = 0</sub><sup>∞</sup> (X<sup>k</sup>) = 1/(1-X) ,as |X| < 1 <br>
Σ<sub>k = 0</sub><sup>∞</sup> (X<sup>k</sup>) = 1/(1-X)       ==>> differentiate both sides considering X <br>
k * Σ<sub>k = 0</sub><sup>∞</sup> (X<sup>k-1</sup>)                 = 1/((1-X)<sup>2</sup>)    ==>> multiply both sides by X            <br>
k * Σ<sub>k = 0</sub><sup>∞</sup> (X<sup>k</sup>)                   = X/((1-X)<sup>2</sup>)    ==>> differentiate both sides considering X <br>
k<sup>2</sup> * Σ<sub>k = 0</sub><sup>∞</sup> (X<sup>k-1</sup>)     = ((1-X)<sup>2</sup> - X * ( 2*(1-X)*-1 )) / ( (1-X)<sup>4</sup> ) 
k<sup>2</sup> * Σ<sub>k = 0</sub><sup>∞</sup> (X<sup>k-1</sup>)     = ((1-X) * (1+X)) / ( (1-X)<sup>4</sup> )
k<sup>2</sup> * Σ<sub>k = 0</sub><sup>∞</sup> (X<sup>k-1</sup>)     = (1+X) / ( (1-X)<sup>3</sup> )        ==>> multiply both sides by X <br>
**k<sup>2</sup> * Σ<sub>k = 0</sub><sup>∞</sup> (X<sup>k</sup>)     = X(1+X) / ( (1-X)<sup>3</sup> )**

## A.1-4
========<br>
From the Geometric series : Σ<sub>k = 0</sub><sup>∞</sup> (X<sup>k</sup>) = 1/(1-X) ,as |X| < 1 <br>

Σ<sub>k = 0</sub><sup>∞</sup> (k-1)/(2<sup>k</sup>) = 
Σ<sub>k = 0</sub><sup>∞</sup> (k-1)*((1/2)<sup>k</sup>) = 
( Σ<sub>k = 0</sub><sup>∞</sup> (k * ((1/2)<sup>k</sup>)) ) + ( Σ<sub>k = 0</sub><sup>∞</sup> (-1 * ((1/2)<sup>k</sup>)) )
( Σ<sub>k = 0</sub><sup>∞</sup> (k * ((1/2)<sup>k</sup>)) ) + (-1*(1/( 1 - 1/2 ))) = 

( Σ<sub>k = 0</sub><sup>∞</sup> (k * ((1/2)<sup>k</sup>)) ) + -2                   ===>> eq(1)

Σ<sub>k = 0</sub><sup>∞</sup> (X<sup>k</sup>) = 1/(1-X)       ==>> differentiate both sides considering X <br>
k * Σ<sub>k = 0</sub><sup>∞</sup> (X<sup>k-1</sup>)                 = 1/((1-X)<sup>2</sup>)        ==>> multiply both sides by X            <br>

k * Σ<sub>k = 0</sub><sup>∞</sup> (X<sup>k</sup>)                   = X/((1-X)<sup>2</sup>)        sustitute in eq(1) we get:

**(1/2) / ((1 - 1/2) <sup>2</sup>) - 2 = 2 - 2 = 0**

## A.1-5
========<br>
        Σ<sub>k = 1</sub><sup>∞</sup>Y<sup>k</sup> = ( 1/(1-Y) ) - 1 = Y/(1-Y)
        > put Y = X<sup>2</sup>
        Σ<sub>k = 1</sub><sup>∞</sup>X<sup>2k</sup> = X<sup>2</sup>/(1-X<sup>2</sup>)
        > Multiply each side by X
        Σ<sub>k = 1</sub><sup>∞</sup>X<sup>(2k+1)</sup> = (X<sup>3</sup>)/((1-X<sup>2</sup>))
        > differentiate both sides
        (2k+1) * Σ<sub>k = 1</sub><sup>∞</sup>X<sup>2k</sup> = 
        ((3X</sup>2<sup> * (1-X</sup>2<sup>)) - (X</sup>3<sup> * -2X) / (1-X<sup>2</sup>))<sup>2</sup>) = 
        ((3X</sup>2<sup> - 3X</sup>4<sup>) + 2X<sup>4</sup>) / (1-X<sup>2</sup>))<sup>2</sup>)  = 
        ((3X</sup>2<sup> - X</sup>4<sup>) / (1-X<sup>2</sup>))<sup>2</sup>)
        
## A.1-6
=========<br>
Let g<sub>1</sub> ,g<sub>2</sub> ..g<sub>n</sub> be any function such that g<sub>k</sub>(i) = O(f<sub>k</sub>(i)).                <br>

By the definition of big O there are constants c<sub>1</sub> ,c<sub>2</sub>, ....c<sub>n</sub> such that                          <br>

g<sub>k</sub>(i) <= c<sub>k</sub> * (f<sub>k</sub>(i)).                                                                           <br>

Let c = max<sub>(1<k<=n)</sub> c<sub>k</sub>. Then:                                                                               <br>

Σ g<sub>k</sub>(i) <= Σ c<sub>k</sub> * (f<sub>k</sub>(i)) <= Σ c * (f<sub>k</sub>(i))  =                                         <br>
O(Σf<sub>k</sub>(i)) --> NOTE: all Σ from k=1 to n                                                                                <br>


## A.1-7
========<br>
∏<sub>k=1</sub><sup>n</sup>(2 * 4<sup>k</sup>) =>
we have: lg(∏<sub>k=1</sub><sup>n</sup>a<sub>k</sub>) = Σ<sub>k=1</sub><sup>n</sup>lg(a<sub>k</sub>)                          <br>
So: lg(∏<sub>k=1</sub><sup>n</sup>(2*4<sup>k</sup>)) = Σ<sub>k=1</sub><sup>n</sup>lg(2*4<sup>k</sup>) =                       <br>
Σ<sub>k=1</sub><sup>n</sup> lg(2) + Σ<sub>k=1</sub><sup>n</sup> lg(4<sup>k</sup>) =                                           <br>
lg(2) * Σ<sub>k=1</sub><sup>n</sup>  + lg(4)* Σ<sub>k=1</sub><sup>n</sup> k =                                                 <br>
(lg(2) * n) + (lg(4) * n*(n+1)/2) =                                                                                           <br>     
n + 2*(n*(n+1)/2)) =( n + n*(n+1) )= n(1 + n + 1) = n * (n + 2)                                                               <br>

SO: lg(∏<sub>k=1</sub><sup>n</sup>(2*4<sup>k</sup>)) = n*(n+2)                                                                <br>
Then: ∏<sub>k=1</sub><sup>n</sup>(2*4<sup>k</sup>) =                                                                          <br>
2<sup>(n*(n+2))</sup> = 2<sup>(n<sup>2</sup>+2n))</sup> = 2<sup>(n<sup>2</sup>))</sup> * 4<sup>n</sup>                        <br>

## A.1-8
========<br>
∏<sub>k = 2</sub> <sup>n</sup> (1-1/k<sup>2</sup>) = (n+1) / 2n                                                               <br>
```
How to solve any summation prove or show:
=========================================
(1) by following the patteren the series is growing.
(2) by using known formules to conclude another formules.
(3) by using mathematical induction.
(4) differentiate or integrate some known formules.
```
