# Summations:
=============
```
(1) Σ<sub>k = 1</sub><sup>n</sup> c = cn
    eg: Σ<sub>k = 1</sub><sup>8</sup> 7 = 7*8 = 56

(2) Σ<sub>k = 1</sub><sup>n</sup> k = n*(n+1)/2.
    eg: Σ<sub>k = 1</sub><sup>5</sup> k = 5*(5+1)/2 = 15
    eg: Σ<sub>k = 1</sub><sup>4</sup> 6k = 6 * (Σ<sub>k = 1</sub><sup>4</sup> k) =
        6 * ( (4*5) / 2 ) = 3*4*5 = 60.

(3) Σ<sub>k = 1</sub><sup>n</sup> k^2 = n*(n+1)*(2n+1)/6.
    eg: Σ<sub>k = 1</sub><sup>6</sup> k^2 = 6*7*13/6 = 91.

(4) Σ<sub>k = 1</sub><sup>n</sup> k^3 = n^2*(n+1)^2 / 4.
    eg: Σ<sub>k = 1</sub><sup>4</sup> k^3 = 4^2 * 5^2 / 4 = 100.

Examples:
    1-
    Σ<sub>k = 1</sub><sup>5</sup> k[k^2 + 4k] =
    Σ<sub>k = 1</sub><sup>5</sup> [k^3 + 4k^2] =
    ( Σ<sub>k = 1</sub><sup>5</sup> k^3 ) + 4 * ( Σ<sub>k = 1</sub><sup>5</sup> k^2 ) =
    (5^2) *(5+1)^2 / 4                    + 4 * 5 * (5+1) * (2*5 + 1) /6              =
    25 * 9                                + 20 * 11                                   =
    445.

    2-
    Σ<sub>k = 1</sub><sup>9</sup> [k - 1]^2 =
    Σ<sub>k = 1</sub><sup>9</sup> [k^2 - 2k + 1] =
    ( Σ<sub>k = 1</sub><sup>9</sup> [k^2] ) - 2 * ( Σ<sub>k = 1</sub><sup>9</sup> k ) + ( Σ<sub>k = 1</sub><sup>9</sup> 1 ) =
    9*(9+1)*(2*9 + 1) / 6                   - 2 * 9*(9+1)/2                           +  1*9                                =
    90*19/6                                 - 90                                      +  9                                  =
    204.
```

# Geometric series:
===================
```
- Geometric series For all real numbers x BUT x != 1, the summation: (x can be (-3) or 3 or 3.3 but not 1)
      Σ<sub>k = 0</sub> <sup>n</sup> X<sup>k</sup> =  1 + X + .... + X(<sup>n</sup>)
**(5) Σ<sub>k = 0</sub> <sup>n</sup> X<sup>k</sup> = (X(<sup>n+1</sup>) - 1) / (X - 1)**
                                OR
      S<sub>n</sub> = ( a<sub>1</sub>*(1 - r<sup>n</sup>) )/(1 - r)

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
```

