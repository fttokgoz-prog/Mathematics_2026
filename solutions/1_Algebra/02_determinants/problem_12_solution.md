# Exercise 12. A Parameter Revealed by a Row Operation

## Given

A(t) = ( 1  2  3 )
       ( 2  4  t )
       ( 0  1  1 )


We need to find all values of t for which the matrix is not invertible.

Before calculating the determinant, we must perform the row operation:

R₂ ← R₂ − 2R₁


We will use the resulting matrix to simplify the determinant calculation and explain what happens to the rows for the value of t we find.

## 1. Perform the row operation

The original matrix is:

A(t) = ( 1  2  3 )
       ( 2  4  t )
       ( 0  1  1 )


The row operation is:

R₂ ← R₂ − 2R₁


This means that we multiply the first row by 2 and subtract the result from the second row.

The first row is:

R₁ = (1, 2, 3)


Multiply each entry by 2:

2R₁ = (2, 4, 6)


The original second row is:

R₂ = (2, 4, t)


Now subtract 2R₁ from R₂, entry by entry.

**First entry:**

2 − 2 = 0


**Second entry:**

4 − 4 = 0


**Third entry:**

t − 6 = t − 6


Therefore, the new second row is:

R₂ = (0, 0, t − 6)


The resulting matrix is:

A₁(t) = ( 1  2  3 )
        ( 0  0  t − 6 )
        ( 0  1  1 )


## 2. Explain the effect of the row operation on the determinant

The operation R₂ ← R₂ − 2R₁ adds a multiple of one row to another row.

This type of row operation does not change the determinant.

Therefore:

det(A₁(t)) = det(A(t))


We can calculate the determinant using the new matrix because it has simpler entries.

A₁(t) = ( 1  2  3 )
        ( 0  0  t − 6 )
        ( 0  1  1 )


## 3. Calculate the determinant of the new matrix

We expand the determinant along the first column.

The entries in the first column are 1, 0, and 0.

Because the last two entries are zero, only the first entry contributes to the determinant.

Therefore:

det(A₁(t)) = 1 × det ( 0  t − 6 )
                        ( 1    1    )


For a 2 × 2 matrix, the determinant is calculated using the formula:

det = ad − bc


Applying the formula to the 2 × 2 matrix:

det ( 0  t − 6 )
    ( 1    1    )


We obtain:

0 × 1 − (t − 6) × 1

= 0 − (t − 6)

= 6 − t


Therefore:

det(A(t)) = 6 − t


## 4. Find the value of t for which the matrix is not invertible

A square matrix is not invertible if and only if its determinant is zero.

Therefore, we set the determinant equal to zero:

det(A(t)) = 0


Substitute the determinant expression:

6 − t = 0


Subtract 6 from both sides:

−t = −6


Multiply both sides by −1:

t = 6


Therefore, the matrix is not invertible when:

t = 6


## 5. Explain what happens to the rows when t = 6

We found that:

t = 6


Substitute this value into the matrix obtained after the row operation:

A₁(6) = ( 1  2  3 )
        ( 0  0  6 − 6 )
        ( 0  1  1 )


Simplify the second row:

6 − 6 = 0


The matrix becomes:

A₁(6) = ( 1  2  3 )
        ( 0  0  0 )
        ( 0  1  1 )


The second row is now a zero row:

R₂ = (0, 0, 0)


A matrix with a zero row has determinant zero.

Therefore:

det(A(6)) = 0


This confirms that the matrix is not invertible when t = 6.


## 6. Explain the special relationship between the rows

When t = 6, the original matrix becomes:

A(6) = ( 1  2  3 )
       ( 2  4  6 )
       ( 0  1  1 )


Notice that the second row is exactly twice the first row:

R₂ = 2R₁


This means that the first two rows are linearly dependent. The second row does not provide any new independent information because it is a multiple of the first row.

After performing the row operation R₂ ← R₂ − 2R₁, the second row becomes zero.

This dependence between the rows explains why the determinant is zero and why the matrix has no inverse.


## Conclusion

We started with:

A(t) = ( 1  2  3 )
       ( 2  4  t )
       ( 0  1  1 )


After performing the row operation R₂ ← R₂ − 2R₁, we obtained:

A₁(t) = ( 1  2  3 )
        ( 0  0  t − 6 )
        ( 0  1  1 )


The determinant is:

det(A(t)) = 6 − t


Setting the determinant equal to zero gives:

6 − t = 0

t = 6


Therefore, the matrix is not invertible when t = 6.

For this value, the second row of the original matrix is twice the first row. The rows are linearly dependent, and the row operation produces a zero row. This is why the determinant is zero and the matrix is not invertible.
