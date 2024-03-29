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
for from i = A.length to 1
    if (A[i] + B[i] + carry) == 3
        c[i+1] = 1
        carry = 1
    else if (A[i] + B[i] + carry) == 2
        c[i+1] = 0
        carry = 1
    else if (A[i] + B[i] + carry) == 1
        c[i+1] = 1
        carry = 0
    else
        c[i+1] = 0
        carry = 0
    end if
end for
c[1] = carry

OR

carry = 0
for i=n to 1 do
    C[i + 1] = (A[i] + B[i] + carry) (mod 2)
    if A[i] + B[i] + carry ≥ 2 then
        carry = 1
    else
        carry = 0
    end if
end for
C[1] = carry
```
2.3-1:
======
From top to Bottom: <br>
3, 41, 52, 26, 38, 57, 9, 49<br>

3, 41, 52, 26 <=> 38, 57, 9, 49 <br>

3, 41 <=> 52, 26 <=> 38, 57 <=> 9, 49 <br>

3 <=> 41 <=> 52 <=> 26 <=> 38 <=> 57 <=> 9 <=> 49 <br>


From Bottom to top:
3, 9, 26, 38, 41, 49, 52, 57<br>

3, 26, 41, 52 <=> 9, 38, 49, 57 <br>

3, 41 <=> 26, 52 <=> 38, 57 <=> 9, 49 <br>

3 <=> 41 <=> 52 <=> 26 <=> 38 <=> 57 <=> 9 <=> 49 <br>

2.3-2:
======


```
void MergeCombine(int a[],int l,int m,int r){
    int i,j,k;
    int n1 = m - l + 1; // first subarray is arr[L..m] , sz_left_subarr
    int n2 = r - m; // second subarray is arr[m+1..r] , sz_right_subarr
    int *L =new int[n1], *R =new int[n2]; // dynamic array to let us set it's size as variable

    for(i = 0 ; i < n1 ; i++){
        L[i] = a[l + i];
    }
    for(j = 0 ; j < n2 ; j++){
        R[j] =a[m + 1 + j];
    }

    i = j = 0;
    k = l;

    while(i < n1 && j < n2){
        if(L[i] <= R[j]){               // If wanna sorting descending make it >
            a[k++] =L[i++];
        }
        else{
            a[k++] =R[j++];
        }
    }
    while(i < n1){
        a[k++] = L[i++];
    }
    while(j < n2){
        a[k++] = R[j++];
    }
}
```

2.3-5:
======
```
int BinarySearch_iterativly(int value,
                            int myArray[],
                            int sz)
{
    int l =0,r =sz-1,md;
    while(l <= r){
        md = l + (r-l)/2;
        if(myArray[md] == value){return md;}
        else if(myArray[md] > value){r =md-1;}
        else{l =md+1;}
    }
    return -1;
}
```



