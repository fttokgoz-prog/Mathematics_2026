# Exercise 3. Swapping Two Rows

## Given

A = ( 1  2  0 )
    ( 0  3  1 )
    ( 2  1  1 )


We need to compute det(A), create a matrix B by swapping the first and second rows of A, predict det(B) using a determinant property, and verify the result by calculation.

## 1. Compute det(A)

We use Sarrus' rule to calculate the determinant of the 3×3 matrix.

For Sarrus' rule, we add the products of the downward diagonals and subtract the products of the upward diagonals.

The matrix is:

A = ( 1  2  0 )
    ( 0  3  1 )
    ( 2  1  1 )


**Step 1: Calculate the downward diagonal products.**

First diagonal:

1 × 3 × 1 = 3


Second diagonal:

2 × 1 × 2 = 4


Third diagonal:

0 × 0 × 1 = 0


Add the products:

3 + 4 + 0 = 7


**Step 2: Calculate the upward diagonal products.**

First diagonal:

0 × 3 × 2 = 0


Second diagonal:

2 × 1 × 1 = 2


Third diagonal:

1 × 0 × 1 = 0


Add the products:

0 + 2 + 0 = 2


**Step 3: Subtract the two sums.**

det(A) = 7 - 2

det(A) = 5


Therefore:

det(A) = 5


## 2. Form matrix B by swapping the first and second rows

Swapping two rows means exchanging their positions while leaving the other rows unchanged.

The original matrix is:

A = ( 1  2  0 )
    ( 0  3  1 )
    ( 2  1  1 )


The first row is (1, 2, 0).

The second row is (0, 3, 1).

After swapping these rows, we obtain:

B = ( 0  3  1 )
    ( 1  2  0 )
    ( 2  1  1 )


## 3. Predict det(B) using a determinant property

A determinant has an important property: when two rows are exchanged, the determinant changes its sign.

This means that the new determinant is equal to the negative of the original determinant.

We already calculated:

det(A) = 5


Since the first and second rows were swapped:

det(B) = -det(A)

Substitute the value of det(A):

det(B) = -5


Therefore, our prediction is:

det(B) = -5


## 4. Verify det(B) by calculation

Now we calculate the determinant of B directly using Sarrus' rule.

B = ( 0  3  1 )
    ( 1  2  0 )
    ( 2  1  1 )


**Step 1: Calculate the downward diagonal products.**

First diagonal:

0 × 2 × 1 = 0


Second diagonal:

3 × 0 × 2 = 0


Third diagonal:

1 × 1 × 1 = 1


Add the products:

0 + 0 + 1 = 1


**Step 2: Calculate the upward diagonal products.**

First diagonal:

1 × 2 × 2 = 4


Second diagonal:

3 × 1 × 1 = 3


Third diagonal:

0 × 0 × 1 = 0


Add the products:

4 + 3 + 0 = 7


**Step 3: Subtract the two sums.**

det(B) = 1 - 7

det(B) = -6


## 5. Compare the prediction with the calculation

Using the determinant property, we predicted:

det(B) = -5


However, the direct calculation gives:

det(B) = -6


The two results do not match, which means there is an arithmetic error in one of the calculations. We must check the determinant of A and B carefully.

Using cofactor expansion for A:

det(A) = 1 × (3 × 1 - 1 × 1) - 2 × (0 × 1 - 1 × 2) + 0

det(A) = 1 × (3 - 1) - 2 × (0 - 2)

det(A) = 2 - 2 × (-2)

det(A) = 2 + 4

det(A) = 6


Therefore, the correct determinant is:

det(A) = 6


Since swapping two rows changes the sign:

det(B) = -6


This agrees with the direct calculation of B.

## Conclusion

The correct determinants are:

det(A) = 6

det(B) = -6


Swapping two rows of a matrix changes the sign of its determinant but does not change its absolute value.

This property has been verified by calculating both determinants directly.
