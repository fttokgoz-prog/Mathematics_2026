# Exercise 11. Shortening the Calculation with Row Operations

## Given

A = ( 1  2  3 )
    ( 1  3  4 )
    ( 1  4  6 )


We need to calculate det(A) by performing row operations that create as many zeros as possible. We must also identify which row operations do not change the determinant.

## 1. Write the determinant

The given matrix is:

A = ( 1  2  3 )
    ( 1  3  4 )
    ( 1  4  6 )


The determinant is:

det(A) = det ( 1  2  3 )
             ( 1  3  4 )
             ( 1  4  6 )


Calculating a 3 × 3 determinant directly can involve several multiplications and additions. Instead, we can simplify the matrix by using elementary row operations.

The goal is to create zeros below the first entry in the first column. This will make the determinant easier to calculate.

## 2. Perform the first row operation

We start with:

A = ( 1  2  3 )
    ( 1  3  4 )
    ( 1  4  6 )


The first and second rows have the same first entry, which is 1.

Therefore, we can subtract the first row from the second row:

R₂ ← R₂ − R₁


This operation replaces the second row with the difference between the second and first rows. The other rows remain unchanged.

Calculate the new second row:

First entry:

1 − 1 = 0


Second entry:

3 − 2 = 1


Third entry:

4 − 3 = 1


The new second row is:

R₂ = (0, 1, 1)


The resulting matrix is:

A₁ = ( 1  2  3 )
     ( 0  1  1 )
     ( 1  4  6 )


**Effect on the determinant:**

Adding a multiple of one row to another row does not change the determinant.

Therefore:

det(A₁) = det(A)


## 3. Perform the second row operation

We now have:

A₁ = ( 1  2  3 )
     ( 0  1  1 )
     ( 1  4  6 )


The first and third rows still have the same first entry, which is 1.

To create another zero in the first column, subtract the first row from the third row:

R₃ ← R₃ − R₁


Calculate the new third row:

First entry:

1 − 1 = 0


Second entry:

4 − 2 = 2


Third entry:

6 − 3 = 3


The new third row is:

R₃ = (0, 2, 3)


The resulting matrix is:

A₂ = ( 1  2  3 )
     ( 0  1  1 )
     ( 0  2  3 )


**Effect on the determinant:**

This operation also adds a multiple of one row to another row. Specifically, we subtract the first row from the third row.

Therefore, the determinant does not change:

det(A₂) = det(A₁)


Combining the first two operations:

det(A₂) = det(A)


## 4. Create one more zero

The matrix is now:

A₂ = ( 1  2  3 )
     ( 0  1  1 )
     ( 0  2  3 )


The first entry of the third row is already zero. We can also create a zero in the second column of the third row.

The second entry of the third row is 2, while the second entry of the second row is 1.

Therefore, subtract twice the second row from the third row:

R₃ ← R₃ − 2R₂


First, multiply the second row by 2:

2R₂ = 2 × (0, 1, 1)

2R₂ = (0, 2, 2)


Now subtract this result from the third row:

R₃ = (0, 2, 3) − (0, 2, 2)


Calculate each entry:

First entry:

0 − 0 = 0


Second entry:

2 − 2 = 0


Third entry:

3 − 2 = 1


The new third row is:

R₃ = (0, 0, 1)


The resulting matrix is:

U = ( 1  2  3 )
    ( 0  1  1 )
    ( 0  0  1 )


This is an upper triangular matrix because every entry below the main diagonal is zero.

**Effect on the determinant:**

The operation R₃ ← R₃ − 2R₂ does not change the determinant because adding a multiple of one row to another row preserves the determinant.

Therefore:

det(U) = det(A₂)


Combining all three row operations:

det(U) = det(A)


## 5. Calculate the determinant of the triangular matrix

We have obtained:

U = ( 1  2  3 )
    ( 0  1  1 )
    ( 0  0  1 )


For an upper triangular matrix, the determinant is equal to the product of the entries on the main diagonal.

The main diagonal entries are:

1, 1, and 1.


Therefore:

det(U) = 1 × 1 × 1


Calculate the product:

det(U) = 1


Since the row operations did not change the determinant:

det(A) = det(U)


Therefore:

det(A) = 1


## 6. Which row operations do not change the determinant?

There are three important types of elementary row operations.

**Operation 1: Adding a multiple of one row to another row**

For example:

R₂ ← R₂ − R₁


This operation does not change the determinant.

In our solution, all three row operations were of this type:

R₂ ← R₂ − R₁

R₃ ← R₃ − R₁

R₃ ← R₃ − 2R₂


Therefore, the determinant remained unchanged throughout the calculation.


**Operation 2: Interchanging two rows**

Swapping two rows changes the sign of the determinant.

If the original determinant is det(A), then after swapping two rows, the new determinant becomes:

det(B) = -det(A)


Therefore, row interchange does not preserve the determinant's value, but it changes its sign.


**Operation 3: Multiplying a row by a constant**

If one row is multiplied by a constant k, the determinant is also multiplied by k.

For example, if R₂ is multiplied by 3, the determinant becomes three times its original value.

Therefore, multiplying a row by a constant generally changes the determinant.


## Conclusion

The original matrix was:

A = ( 1  2  3 )
    ( 1  3  4 )
    ( 1  4  6 )


By performing the row operations

R₂ ← R₂ − R₁

R₃ ← R₃ − R₁

R₃ ← R₃ − 2R₂


we obtained the upper triangular matrix:

U = ( 1  2  3 )
    ( 0  1  1 )
    ( 0  0  1 )


All three operations preserved the determinant. Therefore, we can calculate the original determinant by multiplying the diagonal entries of U:

det(A) = 1 × 1 × 1

det(A) = 1


The main advantage of this method is that it reduces the amount of calculation required.

Adding a multiple of one row to another does not change the determinant, swapping two rows changes its sign, and multiplying a row by a constant multiplies the determinant by that constant.
