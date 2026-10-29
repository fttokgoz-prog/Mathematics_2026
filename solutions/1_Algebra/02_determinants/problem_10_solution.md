# Exercise 10. Detecting Dependence

## Given

A = ( 1  2  3 )
    ( 2  4  6 )
    ( 0  1  5 )


We need to explain why det(A) = 0 without performing a full determinant calculation, identify a specific dependence between the rows, and connect this dependence with the noninvertibility of the matrix.

## 1. Examine the rows of the matrix

The matrix is:

A = ( 1  2  3 )
    ( 2  4  6 )
    ( 0  1  5 )


The three rows are:

First row: R₁ = (1, 2, 3)

Second row: R₂ = (2, 4, 6)

Third row: R₃ = (0, 1, 5)


We can observe that the second row is exactly twice the first row.

R₂ = 2R₁


To verify this relationship, multiply every entry of the first row by 2:

2 × (1, 2, 3) = (2, 4, 6)


This is exactly the second row of the matrix.

Therefore:

R₂ = 2R₁


## 2. Explain why the determinant is zero

An important property of determinants states that if two rows of a square matrix are proportional, its determinant is zero.

In this matrix, the second row is twice the first row.

R₂ = 2R₁


This means that the rows are linearly dependent. One row can be obtained by multiplying another row by a constant.

Therefore, the rows do not provide three independent directions.

As a result, the determinant must be zero:

det(A) = 0


We can reach this conclusion directly from the structure of the matrix without calculating the determinant using Sarrus' rule or cofactor expansion.

## 3. Identify the linear dependence between the rows

The relationship between the first two rows is:

R₂ = 2R₁


We can rewrite this equation as:

R₂ - 2R₁ = 0


This is a nontrivial linear relation between the rows because the coefficients are not all zero.

Specifically:

- The coefficient of R₁ is -2.
- The coefficient of R₂ is 1.
- The coefficient of R₃ is 0.

Therefore:

-2R₁ + R₂ + 0R₃ = 0


This confirms that the rows of A are linearly dependent.

## 4. Connect the zero determinant with noninvertibility

A square matrix is invertible if and only if its determinant is nonzero.

If the determinant is zero, the matrix does not have an inverse.

For the given matrix, we established that:

det(A) = 0


Therefore, A is not invertible.

The linear dependence between the rows explains why the matrix is singular: its rows are not linearly independent, so the matrix cannot have full rank.

Consequently, there is no inverse matrix A⁻¹ satisfying:

AA⁻¹ = I


## Conclusion

The given matrix is:

A = ( 1  2  3 )
    ( 2  4  6 )
    ( 0  1  5 )


The second row is twice the first row:

R₂ = 2R₁


Therefore, the rows are linearly dependent, which implies:

det(A) = 0


Since the determinant is zero, the matrix is not invertible.

This example shows that we can identify a zero determinant by recognizing linear dependence between rows, without carrying out a full determinant calculation.
