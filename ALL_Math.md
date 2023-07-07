# Sequences:
=============

- Find the pattern:
  ==================
  eg 1:  {2, 3/sqrt(2), 4/sqrt(3), 5/2, ......}    <br>
  sol:   {2/sqrt(1), 3/sqrt(2), 4/sqrt(3), 5/sqrt(4), .....} ,<br>
          a<sub>1</sub> = 2/sqrt(1)<br>
          a<sub>2</sub> = 3/sqrt(2)<br>
          a<sub>3</sub> = 4/sqrt(3)<br>
          a<sub>4</sub> = 5/sqrt(4)<br>
          so , a<sub>n</sub> = (n+1)/sqrt(n)<br>
  
# Summations:
=============

(1) ***Σ<sub>k = 1</sub><sup>n</sup> c = cn***<br>
    eg: Σ<sub>k = 1</sub><sup>8</sup> 7 = 7*8 = 56<br>

(2) ***Σ<sub>k = 1</sub><sup>n</sup> k = n*(n+1)/2.***<br>
    eg: Σ<sub>k = 1</sub><sup>5</sup> k = 5*(5+1)/2 = 15<br>
    eg: Σ<sub>k = 1</sub><sup>4</sup> 6k = 6 * (Σ<sub>k = 1</sub><sup>4</sup> k) =<br>
        6 * ( (4*5) / 2 ) = 3*4*5 = 60.<br>

(3) ***Σ<sub>k = 1</sub><sup>n</sup> k<sup>2</sup> = n*(n+1)*(2n+1)/6.***<br>
    eg: Σ<sub>k = 1</sub><sup>6</sup> k^2 = 6*7*13/6 = 91.<br>

(4) ***Σ<sub>k = 1</sub><sup>n</sup> k<sup>3</sup> = n<sup>2</sup>*(n+1)<sup>2</sup> / 4.***<br>
    eg: Σ<sub>k = 1</sub><sup>4</sup> k<sup>3</sup> = 4<sup>2</sup> * 5<sup>2</sup> / 4 = 100.<br>

Examples:<br>
1-
    Σ<sub>k = 1</sub><sup>5</sup> k[k<sup>2</sup> + 4k] =<br>
    Σ<sub>k = 1</sub><sup>5</sup> [k<sup>3</sup> + 4k<sup>2</sup>] =<br>
    ( Σ<sub>k = 1</sub><sup>5</sup> k<sup>3</sup> ) + 4 * ( Σ<sub>k = 1</sub><sup>5</sup> k<sup>2</sup> ) =<br>
    (5^2) *(5+1)<sup>2</sup> / 4                    + 4 * 5 * (5+1) * (2*5 + 1) /6                        =<br>
    25 * 9                                          + 20 * 11                                             =<br>
    445.<br>

2-
    Σ<sub>k = 1</sub><sup>9</sup> [k - 1]<sup>2</sup> =<br>
    Σ<sub>k = 1</sub><sup>9</sup> [k<sup>2</sup> - 2k + 1] =<br>
    ( Σ<sub>k = 1</sub><sup>9</sup> [k<sup>2</sup>] ) - 2 * ( Σ<sub>k = 1</sub><sup>9</sup> k ) + ( Σ<sub>k = 1</sub><sup>9</sup> 1 ) =<br>
    9*(9+1)*(2*9 + 1) / 6                             - 2 * 9*(9+1)/2                           +  1*9                                =<br>
    90*19/6                                           - 90                                      +  9                                  =<br>
    204.<br>


# Geometric series:<br>
===================

- Geometric series For all real numbers x BUT x != 1, the summation: (x can be (-3) or 3 or 3.3 but not 1)<br>
      Σ<sub>k = 0</sub> <sup>n</sup> X<sup>k</sup> =  1 + X + .... + X(<sup>n</sup>)<br>
**(5) Σ<sub>k = 0</sub> <sup>n</sup> X<sup>k</sup> = (X(<sup>n+1</sup>) - 1) / (X - 1)**<br>
                                OR<br>
      S<sub>n</sub> = ( a<sub>1</sub>*(1 - r<sup>n</sup>) )/(1 - r)<br>

- When the summation is infinite and |x| < 1, we have the infinite decreasing geometric series:
**(6) Σ<sub>k = 0</sub> <sup>∞</sup> X<sub>k</sub> = 1/(1-X)**
                                OR
S = ( a<sub>1</sub> )/(1 - r) , |r| < 1 ===>> (-1 < r < 1)

Examples:
---------
1-
     Σ<sub>k = 1</sub> <sup>6</sup> 2<sub>k</sub> = ((2^(6+1) - 1) / (2-1)) - 1 = 126.

2-
    Σ<sub>k = 1</sub> <sup>4</sup> 3/2<sub>(k-1)</sub> =
    Σ<sub>k = 1</sub> <sup>4</sup> (3/2)<sub>k</sub> / (3/2) =  (Σ<sub>k = 0</sub> <sup>4</sup> - Σ<sub>k = 0</sub> <sup>0</sup>)
    (2/3) * ( ( (3/2)^(4+1) - 1) / ((3/2) - 1)  - (3/2)^0 )  = 8.125.

3-
    Σ<sub>k = 1</sub> <sup>∞</sup> 8 * (2/3)<sub>(k-1)</sub> =
    8*(3/2) * Σ<sub>k = 1</sub> <sup>∞</sup> (2/3)<sub>k</sub> =
    12 * (Σ<sub>k = 0</sub> <sup>∞</sup> (2/3)<sub>k</sub> - Σ<sub>k = 0</sub> <sup>0</sup> (2/3)<sub>k</sub>) =
    12 * ( 1 / (1 - ( 2/3 ) ) - (2/3)^0) = 24.
    
OR

as |2/3| < 1  ==>> -1 < 2/3 < 1
S = 8/(1-2/3) = 24.

# Harmonic series
==================


# Telescoping series
=====================


