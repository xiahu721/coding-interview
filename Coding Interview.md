# Coding Interview

**Goal:**

* Readable
* Scalable



#### Arrays

###### Static vs. Dynamic Arrays

*Static Array* : (aka. Fixed or compile-time arrays)

1. **Static Arrays** are created on **stack**.

2. **Size** of static arrays should be **determined at compile-time** (before run-time).

3. **Size** is **fixed**.

4. No need to delete static arrays, they are deleted automatically after going out of scope.

   Eg. : int array[10]; //array of size 10

*Dynamic Array :*

1. **Dynamic Arrays** are allocated on **heap**.

2. **Size** of dynamic arrays can be **determined either at compilation or at run-time (flexible)**.

3. **Size** is not fixed.

4. You can construct **very large** dynamic arrays on heap, unlike static arrays.

5. You **need to manually delete dynamic arrays** after you no longer need them.

   Eg. : int* array = new int[10];

Languages like Javascript, python, ArrayList in Java use **dynamic arrays**.

###### Reverse A String

1. split the string into a array;
2. reverse the array;
3. Join togother the array.

###### Merge Two Sorted Arrays

Two pointers scan the two arrays each.



#### Hash Table

###### Hash Function

MD5, SHA-1, SHA-256

###### First Recurring Character

Back-tracking and using set.

