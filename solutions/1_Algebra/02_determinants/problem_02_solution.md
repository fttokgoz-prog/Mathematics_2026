# Exercise 2. Determinant of a 3×3 Matrix

## Given

A = ( 1   2  -1 )
    ( 0   3   4 )
    ( 2   1   5 )


We need to compute det(A) using Sarrus' rule and check the result using a property of determinants.

## 1. Compute det(A) using Sarrus' rule

For a 3×3 matrix, Sarrus' rule states that we add the products of the three diagonals going from top-left to bottom-right, and subtract the products of the three diagonals going from top-right to bottom-left.

The matrix is:

A = ( 1   2  -1 )
    ( 0   3   4 )
    ( 2   1   5 )


**Step 1: Calculate the products of the downward diagonals.**

First diagonal:

1 × 3 × 5 = 15


Second diagonal:

2 × 4 × 2 = 16


Third diagonal:

(-1) × 0 × 1 = 0


Add these three products:

15 + 16 + 0 = 31


**Step 2: Calculate the products of the upward diagonals.**

First diagonal:

(-1) × 3 × 2 = -6


Second diagonal:

2 × 0 × 5 = 0


Third diagonal:

1 × 4 × 1 = 4


Add these three products:

-6 + 0 + 4 = -2


**Step 3: Subtract the sum of the upward diagonals from the sum of the downward diagonals.**

det(A) = 31 - (-2)

Subtracting a negative number is the same as adding a positive number.

det(A) = 31 + 2

det(A) = 33


**Final answer:**

det(A) = 33


## 2. Check the result using a determinant property

We can check the result by expanding the determinant along the first row. This uses the cofactor expansion formula.

For a 3×3 matrix, the determinant can be calculated by multiplying each entry in the first row by its corresponding signed 2×2 minor.

The formula is:

det(A) = a(ei - fh) - b(di - fg) + c(dh - eg)

For our matrix:

A = ( 1   2  -1 )
    ( 0   3   4 )
    ( 2   1   5 )


Expanding along the first row:

det(A) = 1 × (3 × 5 - 4 × 1)
         - 2 × (0 × 5 - 4 × 2)
         + (-1) × (0 × 1 - 3 × 2)


**Step 1: Calculate the first term.**

1 × (15 - 4)

= 1 × 11

= 11


**Step 2: Calculate the second term.**

-2 × (0 - 8)

= -2 × (-8)

= 16


**Step 3: Calculate the third term.**

(-1) × (0 - 6)

= (-1) × (-6)

= 6


**Step 4: Add the three terms.**

det(A) = 11 + 16 + 6

det(A) = 33


## 3. Compare the results

Using Sarrus' rule, we obtained:

det(A) = 33


Using cofactor expansion along the first row, we obtained:

det(A) = 33


Both methods give the same result, so the calculation is confirmed.


## Conclusion

The determinant of the matrix is:

det(A) = 33

Sarrus' rule gives the determinant by adding the downward diagonal products and subtracting the upward diagonal products. The cofactor expansion provides an independent check and confirms that the determinant is 33.
