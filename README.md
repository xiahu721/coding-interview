## Arrays



#### Merge Arrays

**question**:

Given 2 sorted arrays, A and B, where A is long enough to hold the contents of A and B, write a function to copy the contents of B into A without using any buffer or additional memory.

> A = [1, 3, 5, 0, 0, 0];
>
> B = [2, 4, 6];
>
> mergeArrays(A, B);
>
> A = [1, 2, 3, 4, 5, 6];



**Selution:**

Two pointers scan the two arrays each.

```js
// Input:
let A = [1, 3, 5];
let B = [2, 4, 6];

function mergeArrays(A, B) {
  let toalLength = A.length + B.length;

  let i = A.length - 1;
  let j = B.length - 1;
  let k = toalLength - 1;

  while (i >= 0 && j >= 0) {
    if (A[i] > B[j]) {
      A[k--] = A[i--];
    } else {
      A[k--] = B[j--];
    }
  }
  while (j >= 0) {
    A[k--] = B[j--];
  }
}

mergeArrays(A, B);
console.log(A); 

// Output:
//A: [ 1, 2, 3, 4, 5, 6 ]
```

