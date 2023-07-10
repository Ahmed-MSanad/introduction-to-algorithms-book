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
        Σ<sub>k = 1</sub><sup>∞</sup>X<sup>k</sup> = ( 1/(1-X) ) - 1 = x/(1-X)
        Multiply each side by X<sup>k</sup>,
        Σ<sub>k = 1</sub><sup>∞</sup>X<sup>2k</sup> = X/(1-X)


```
How to solve any summation prove or show:
=========================================
(1) by following the patteren the series is growing.
(2) by using known formules to conclude another formules.
(3) by using mathematical induction.
(4) differentiate or integrate some known formules.
```
