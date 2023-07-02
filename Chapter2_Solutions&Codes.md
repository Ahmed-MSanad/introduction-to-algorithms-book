# Solutions
=============
## 2.1-1)
========
```
A = (31, 41, 59, 26, 41, 58)    -->    (31, **41**, 59, 26, 41, 58)    -->    (31, 41, **59**, 26, 41, 58)    -->
(**26**, 31, 41, 59, 41, 58)    -->    (26, 31, 41, **41**, 59, 58)    -->    (26, 31, 41, 41, **58**, 59)
```


## 2.1-2)
========
```
#include <stdio.h>
#include <stdlib.h>

int main()
{
    int a[] = {31, 41, 59, 26, 41, 58};
    for(int i=1;i<6;i++){
        int j = i-1, key = a[i];
        while(j >= 0 && a[j] < key){
            a[j+1] = a[j];
            j--;
        }
        a[j+1] = key;
    }

    for(int i=0;i<6;i++){
        printf("%i\t",a[i]);
    }
    return 0;
}
```

## 2.1-3)
========
```
x = NIL
For loop from j = 1 to A.length
    if A[j] == v then
        x = j
        return j
    end if
end for
return x

Loop invariant : Is v excited or not and On each iteration of the loop body, the invariant upon entering is that there
                 is no index k < j so that A[k] = v.

Initialization : After the loop initialization and before the loop test we don't know whether the value v is
                 excited or not after each iteratoin we check whether it's excited or not.

Maintanince    : Before each iteration we must sure we search the true value.

Termination    : Finally we check whether it's exicted or not and our code is correct if it return the value if it's
                 in the array or NIL if it's not otherwise it's incorrect.
```

## 2.1-4)
========
```
Input : 2 arrays(A, B) of size n each has the binary of a n-bit number.
Output : array of n+1 elements has the sum of the given 2 numbers.

carry =0
for from i = 1 to A.length
    if (A[i] + B[i] + carry) == 3
        c[i] = 1
        carry = 1
    end if
    else if (A[i] + B[i] + carry) == 2
        c[i] = 0
        carry = 1
    end else if
    else if (A[i] + B[i] + carry) == 1
        c[i] = 1
        carry = 0
    end if
    else
        c[i] = 0
        carry = 0
    end else
end for
c[i] = carry
```
