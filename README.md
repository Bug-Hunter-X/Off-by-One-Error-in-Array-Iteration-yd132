# Off-by-One Error in Java Array
This repository demonstrates a common off-by-one error in Java when iterating over an array.  The code attempts to access an index that is out of bounds, resulting in an `ArrayIndexOutOfBoundsException`.  The solution demonstrates the correct way to iterate to avoid this error.

## Bug
The `Bug.java` file contains the erroneous code. The for loop condition `i <= arr.length` is incorrect; it should be `i < arr.length`. The array has indexes 0-4, but the loop tries to access index 5, which is out of bounds.

## Solution
The `BugSolution.java` file provides the corrected code. The loop condition is changed to `i < arr.length` to prevent the out-of-bounds access. This ensures the loop only iterates through valid indices.