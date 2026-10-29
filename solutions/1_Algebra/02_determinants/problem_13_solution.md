# Exercise 13. Determinant by Elimination

## Given

A = ( 1  2  3 )
    ( 2  5  7 )
    ( 1  0  2 )


We need to compute the determinant using elimination and record the effect of every row operation on the determinant.

## 1. Write the determinant

The given matrix is:

A = ( 1  2  3 )
    ( 2  5  7 )
    ( 1  0  2 )


Our goal is to transform the matrix into an upper triangular matrix by creating zeros below the main diagonal.

Once the matrix is upper triangular, its determinant is the product of the diagonal entries.

We must also keep track of how each row operation affects the determinant.

## 2. Perform the first row operation

We start with:

A = ( 1  2  3 )
    ( 2  5  7 )
    ( 1  0  2 )


The first entry of the second row is 2, and the first entry of the first row is 1.

To create a zero in the first column of the second row, perform:

R₂ ← R₂ − 2R₁


First, multiply the first row by 2:

2R₁ = ( 2  4  6 )


Now subtract it from the second row:

R₂ = (2, 5, 7) − (2, 4, 6)


Calculate each entry:

2 − 2 = 0

5 − 4 = 1

7 − 6 = 1


The new second row is:

R₂ = (0, 1, 1)


The resulting matrix is:

A₁ = ( 1  2  3 )
     ( 0  1  1 )
     ( 1  0  2 )


**Effect on the determinant:**

Adding a multiple of one row to another row does not change the determinant.

Therefore:

det(A₁) = det(A)


## 3. Perform the second row operation

The current matrix is:

A₁ = ( 1  2  3 )
     ( 0  1  1 )
     ( 1  0  2 )


The first entry of the third row is 1. We can create a zero by subtracting the first row from the third row.

Perform:

R₃ ← R₃ − R₁


Calculate the new third row:

First entry:

1 − 1 = 0


Second entry:

0 − 2 = -2


Third entry:

2 − 3 = -1


The new third row is:

R₃ = (0, -2, -1)


The resulting matrix is:

A₂ = ( 1   2   3 )
     ( 0   1   1 )
     ( 0  -2  -1 )


**Effect on the determinant:**

This operation also adds a multiple of one row to another row, so the determinant does not change.

Therefore:

det(A₂) = det(A₁)


Combining the first two operations:

det(A₂) = det(A)


## 4. Perform the third row operation

We now have:

A₂ = ( 1   2   3 )
     ( 0   1   1 )
     ( 0  -2  -1 )


The second entry of the third row is -2. We want to make it zero by using the second row.

Perform:

R₃ ← R₃ + 2R₂


First, multiply the second row by 2:

2R₂ = (0, 2, 2)


Now add this result to the third row:

R₃ = (0, -2, -1) + (0, 2, 2)


Calculate each entry:

0 + 0 = 0

-2 + 2 = 0

-1 + 2 = 1


The new third row is:

R₃ = (0, 0, 1)


The resulting matrix is:

U = ( 1  2  3 )
    ( 0  1  1 )
    ( 0  0  1 )


**Effect on the determinant:**

The operation R₃ ← R₃ + 2R₂ does not change the determinant because adding a multiple of one row to another row preserves the determinant.

Therefore:

det(U) = det(A₂)


Since none of our row operations changed the determinant:

det(U) = det(A)


## 5. Calculate the determinant of the upper triangular matrix

We obtained:

U = ( 1  2  3 )
    ( 0  1  1 )
    ( 0  0  1 )


This is an upper triangular matrix because all entries below the main diagonal are zero.

For any triangular matrix, the determinant equals the product of the main diagonal entries.

The diagonal entries are:

1, 1, and 1.


Therefore:

det(U) = 1 × 1 × 1


Calculate the product:

det(U) = 1


Since all row operations preserved the determinant:

det(A) = det(U)


Therefore, the final answer is:

det(A) = 1


## 6. Record the effect of each row operation

The row operations used were:

**First operation:**

R₂ ← R₂ − 2R₁

The determinant does not change.


**Second operation:**

R₃ ← R₃ − R₁

The determinant does not change.


**Third operation:**

R₃ ← R₃ + 2R₂

The determinant does not change.


All three operations involve adding a multiple of one row to another row. Therefore, the determinant remains unchanged throughout the elimination process.

No rows were interchanged, and no row was multiplied by a constant by itself.

## Conclusion

The original matrix was:

A = ( 1  2  3 )
    ( 2  5  7 )
    ( 1  0  2 )


After elimination, we obtained:

U = ( 1  2  3 )
    ( 0  1  1 )
    ( 0  0  1 )


The determinant of the upper triangular matrix is:

det(U) = 1 × 1 × 1 = 1


Since every row operation preserved the determinant, we conclude that:

det(A) = 1


This exercise demonstrates how elimination simplifies determinant calculations while allowing us to track the effect of every row operation.
