# Exercise 7. Using Properties Instead of Recomputing

## Given

A is a 3 × 3 matrix, and:

det(A) = -4


We need to compute:

1. det(2A)
2. det(Aᵀ)
3. det(A²)
4. det(-A)


Each answer will be justified using the appropriate determinant property.

## 1. Compute det(2A)

For an n × n matrix A, multiplying the entire matrix by a scalar k multiplies its determinant by kⁿ.

The formula is:

det(kA) = kⁿ × det(A)


Since A is a 3 × 3 matrix, we have n = 3.

In this exercise, k = 2 and det(A) = -4.

Therefore:

det(2A) = 2³ × det(A)


**Step 1: Calculate the power of 2.**

2³ = 2 × 2 × 2 = 8


**Step 2: Multiply by the determinant of A.**

det(2A) = 8 × (-4)

det(2A) = -32


**Final answer:**

det(2A) = -32


## 2. Compute det(Aᵀ)

The transpose of a matrix is obtained by changing its rows into columns and its columns into rows.

An important determinant property states that the determinant of a matrix does not change when the matrix is transposed.

The formula is:

det(Aᵀ) = det(A)


We are given:

det(A) = -4


Therefore:

det(Aᵀ) = -4


**Final answer:**

det(Aᵀ) = -4


The determinant remains unchanged because transposing a matrix does not change its determinant.


## 3. Compute det(A²)

The notation A² means multiplying A by itself:

A² = A × A


The determinant of a product is equal to the product of the determinants.

The formula is:

det(AB) = det(A) × det(B)


Applying this property to A²:

det(A²) = det(A × A)

det(A²) = det(A) × det(A)


Since det(A) = -4:

det(A²) = (-4) × (-4)


Multiplying two negative numbers gives a positive result:

det(A²) = 16


**Final answer:**

det(A²) = 16


This result can also be written using the general power property:

det(Aⁿ) = (det(A))ⁿ


For n = 2:

det(A²) = (-4)² = 16


## 4. Compute det(-A)

The matrix -A is obtained by multiplying every entry of A by -1.

For an n × n matrix, multiplying the entire matrix by a scalar k gives:

det(kA) = kⁿ × det(A)


Since A is a 3 × 3 matrix, n = 3 and k = -1.

Therefore:

det(-A) = (-1)³ × det(A)


**Step 1: Calculate the power of -1.**

(-1)³ = (-1) × (-1) × (-1)

(-1)³ = -1


**Step 2: Multiply by det(A).**

det(-A) = (-1) × (-4)

det(-A) = 4


**Final answer:**

det(-A) = 4


The determinant changes sign because the matrix has an odd number of rows and columns, specifically a dimension of 3 × 3.


## Conclusion

Given that det(A) = -4 for a 3 × 3 matrix, the results are:

det(2A) = -32

det(Aᵀ) = -4

det(A²) = 16

det(-A) = 4


These results follow from four determinant properties:

1. Scaling a 3 × 3 matrix by k multiplies its determinant by k³.
2. Transposing a matrix does not change its determinant.
3. The determinant of a product equals the product of the determinants.
4. Multiplying a 3 × 3 matrix by -1 changes the sign of its determinant.

Using these properties allows us to calculate the answers without recomputing the determinants from the entries of A.
