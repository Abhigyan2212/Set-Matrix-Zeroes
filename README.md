Set Matrix Zeroes

Problem Description

You are given an  integer matrix matrix. If an element in the matrix is , set its entire row and column to . Perform this operation in-place without using extra space for another matrix.

Example 1

Input: matrix = [
    [1, 1, 1],
    [1, 0, 1],
    [1, 1, 1]
]

Output: matrix = [
    [1, 0, 1],
    [0, 0, 0],
    [1, 0, 1]
]
Solution Approach

Algorithm

Mark Rows and Columns:

Traverse the matrix to identify rows and columns that need to be zeroed.

Use the first row and column as markers to store this information.

Update Elements:

Use the markers to update the rest of the matrix, setting elements to  as required.

Handle First Row and Column:

Finally, process the first row and column separately to apply the zeroing.

Complexity

Time Complexity: The matrix is traversed twice: once for marking and once for updating.

Space Complexity: In-place modification is achieved without using additional space.
Key Insights

This solution uses the first row and column of the matrix to store markers for zeroing rows and columns.

It is optimal in terms of both time and space complexity.

Tags

Matrix

In-Place Algorithms

Array Manipulation

