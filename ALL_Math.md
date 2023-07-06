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













