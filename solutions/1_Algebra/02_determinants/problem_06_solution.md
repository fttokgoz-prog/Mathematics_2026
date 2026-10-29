# Exercise 6. Parameter and Invertibility

## Given

A(t) = ( t  1 )
       ( 2  t )


We need to find all values of t for which the matrix is not invertible and explain how this relates to the determinant being zero.

## 1. Calculate the determinant of A(t)

For a 2×2 matrix, the determinant is calculated using the formula:

det(A) = ad - bc

For the given matrix:

A(t) = ( t  1 )
       ( 2  t )


The entries are:

a = t

b = 1

c = 2

d = t


Substituting these values into the determinant formula:

det(A(t)) = t × t - 1 × 2


**Step 1: Multiply the entries on the main diagonal.**

t × t = t²


**Step 2: Multiply the entries on the other diagonal.**

1 × 2 = 2


**Step 3: Subtract the second product from the first product.**

det(A(t)) = t² - 2


Therefore, the determinant is:

det(A(t)) = t² - 2


## 2. Find the values of t for which the matrix is not invertible

A square matrix is not invertible if and only if its determinant is equal to zero.

Therefore, we set the determinant equal to zero:

det(A(t)) = 0


Substitute the determinant expression:

t² - 2 = 0


**Step 1: Add 2 to both sides.**

t² - 2 + 2 = 0 + 2

t² = 2


**Step 2: Take the square root of both sides.**

t = ±√2


This gives two possible values:

t = √2

t = -√2


Therefore, the matrix is not invertible when:

t = √2 or t = -√2


## 3. Verify the result

We can substitute both values into the determinant formula to check that the determinant is zero.

**Case 1: t = √2**

det(A(√2)) = (√2)² - 2

det(A(√2)) = 2 - 2

det(A(√2)) = 0


Therefore, the matrix is not invertible when t = √2.


**Case 2: t = -√2**

det(A(-√2)) = (-√2)² - 2

det(A(-√2)) = 2 - 2

det(A(-√2)) = 0


Therefore, the matrix is also not invertible when t = -√2.


## 4. Explain the relationship between the determinant and invertibility

The determinant tells us whether a square matrix is invertible.

If the determinant is nonzero, the matrix is invertible and has an inverse.

If the determinant is zero, the matrix is not invertible and has no inverse.

For this matrix:

det(A(t)) = t² - 2


When t² - 2 is not zero, the matrix is invertible.

When t² - 2 equals zero, the matrix is not invertible.

Solving t² - 2 = 0 gives t = √2 and t = -√2.

These are exactly the values for which the determinant is zero.


## Conclusion

The determinant of the matrix is:

det(A(t)) = t² - 2


Setting the determinant equal to zero gives:

t² - 2 = 0

t² = 2

t = ±√2


Therefore, the matrix A(t) is not invertible for:

t = √2 and t = -√2


A square matrix is not invertible exactly when its determinant is zero.
