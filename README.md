

# Matrix Operations in C

A console-based C program that performs basic matrix operations:

* Addition
* Subtraction
* Multiplication
* Transpose

## Features

* Supports matrices of user-defined dimensions.
* Performs addition and subtraction only if matrices have matching dimensions.
* Performs multiplication if the number of columns in the first matrix equals the number of rows in the second.
* Calculates and displays the transpose of the first matrix.
* Validates input dimensions and notifies when operations are not possible.

## How to Compile and Run

1. Save the code in a file, e.g., `matrix_operations.c`.
2. Compile using GCC:

```bash
gcc matrix_operations.c -o matrix_operations
```

3. Run the program:

```bash
./matrix_operations
```

4. Follow prompts to enter matrix dimensions and elements.

## Sample Usage

```
Enter dimensions of matrix 1 (rows columns): 2 3
Enter elements of matrix 1:
1 2 3
4 5 6
Enter dimensions of matrix 2 (rows columns): 3 2
Enter elements of matrix 2:
7 8
9 10
11 12

Matrix addition not possible due to dimension mismatch.

Matrix subtraction not possible due to dimension mismatch.

Product of matrices:
58 64
139 154

Transpose of Matrix 1:
1 4
2 5
3 6
```

## Notes

* Input validation is minimal; ensure correct matrix dimensions and valid integers.
* The program uses Variable Length Arrays (VLA) for dynamic matrix sizes (supported in C99 and later).
* In the `printMatrix` function, note: The line `printf("/n");` should be corrected to `printf("\n");` to properly print a new line.

## Suggestions for Improvement

* Add more robust error handling.
* Implement matrix input from files.
* Extend to handle floating-point matrices
