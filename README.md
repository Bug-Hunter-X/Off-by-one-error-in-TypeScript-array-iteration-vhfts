# TypeScript Off-by-One Error
This repository demonstrates a common off-by-one error in TypeScript when iterating over arrays.

## Bug
The `printArray` function attempts to iterate through an array using a loop that goes one element beyond the array's valid index range. This leads to an error because accessing `arr[arr.length]` attempts to access an element that doesn't exist.

## Solution
The solution corrects the loop condition to `i < arr.length`, ensuring the loop iterates only through valid indices of the array.