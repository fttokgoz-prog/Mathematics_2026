# Exercise 4. Triangular Matrix

## Given

A = ( 2   4   1 )
    ( 0  -3   5 )
    ( 0   0   7 )


We need to compute the determinant without expanding it and explain the determinant rule for triangular matrices.

## 1. Identify the type of matrix

The given matrix is an upper triangular matrix.

A matrix is upper triangular when all entries below the main diagonal are zero.

In this matrix, the entries below the main diagonal are:

0, 0, and 0.

Therefore, A is an upper triangular matrix.

## 2. Compute the determinant without expanding

For a triangular matrix, the determinant is equal to the product of the entries on the main diagonal.

The main diagonal entries are:

First diagonal entry: 2

Second diagonal entry: -3

Third diagonal entry: 7


Therefore:

det(A) = 2 × (-3) × 7


**Step 1: Multiply the first two entries.**

2 × (-3) = -6


**Step 2: Multiply the result by the third entry.**

-6 × 7 = -42


Therefore, the determinant is:

det(A) = -42


## 3. State the rule for an arbitrary triangular matrix

For any upper triangular or lower triangular square matrix, the determinant is equal to the product of the entries on the main diagonal.

For example, for a 3 × 3 triangular matrix:

A = ( a₁₁  a₁₂  a₁₃ )
    (  0   a₂₂  a₂₃ )
    (  0    0   a₃₃ )


The determinant is:

det(A) = a₁₁ × a₂₂ × a₃₃


The same rule applies to lower triangular matrices, where all entries above the main diagonal are zero.

## 4. Explain the rule using this example

In the given matrix:

A = ( 2   4   1 )
    ( 0  -3   5 )
    ( 0   0   7 )


The main diagonal contains the numbers 2, -3, and 7.

All entries below the main diagonal are zero, so the matrix is upper triangular.

We can calculate the determinant directly by multiplying the diagonal entries:

det(A) = 2 × (-3) × 7

det(A) = -42


There is no need to expand the determinant because the triangular matrix property gives the result directly.

## Conclusion

The determinant of the given matrix is:

det(A) = -42


For any triangular matrix, the determinant is the product of its main diagonal entries. This property makes calculating determinants easier because we do not need to use cofactor expansion or Sarrus' rule.
