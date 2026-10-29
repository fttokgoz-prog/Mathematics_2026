# Exercise 8. Determinant of a Product

## Given

A and B are square matrices such that:

det(A) = 3

det(B) = -5


We need to compute det(AB), det(BA), and det(A⁴B⁻¹), if it exists. We must also explain why the first two results are equal even though AB is not necessarily equal to BA.

## 1. Compute det(AB)

An important property of determinants states that the determinant of a product of two square matrices is equal to the product of their determinants.

The formula is:

det(AB) = det(A) × det(B)


We are given:

det(A) = 3

det(B) = -5


Substitute these values into the formula:

det(AB) = 3 × (-5)


Multiply the two numbers:

det(AB) = -15


Therefore:

det(AB) = -15


## 2. Compute det(BA)

We use the same determinant property:

det(BA) = det(B) × det(A)


Substitute the given values:

det(BA) = (-5) × 3


Multiply the two numbers:

det(BA) = -15


Therefore:

det(BA) = -15


## 3. Explain why det(AB) = det(BA), even though AB is not necessarily equal to BA

From our calculations, we obtained:

det(AB) = -15

det(BA) = -15


Therefore:

det(AB) = det(BA)


This happens because ordinary multiplication of numbers is commutative.

In other words:

det(A) × det(B) = det(B) × det(A)


However, matrix multiplication itself is not generally commutative. This means that AB and BA can be different matrices even when their determinants are equal.

Therefore, equal determinants do not necessarily mean that two matrices are equal.

## 4. Compute det(A⁴B⁻¹)

We need to calculate the determinant of the product A⁴B⁻¹.

First, we use the determinant property for products:

det(A⁴B⁻¹) = det(A⁴) × det(B⁻¹)


We will calculate each determinant separately.

### Step 1: Calculate det(A⁴)

For a square matrix A, the determinant of a power satisfies:

det(Aⁿ) = (det(A))ⁿ


For n = 4:

det(A⁴) = (det(A))⁴


Since det(A) = 3:

det(A⁴) = 3⁴

det(A⁴) = 3 × 3 × 3 × 3

det(A⁴) = 81


Therefore:

det(A⁴) = 81


### Step 2: Calculate det(B⁻¹)

Since det(B) = -5 and -5 is not zero, matrix B is invertible.

For any invertible square matrix B, the determinant of its inverse is:

det(B⁻¹) = 1 / det(B)


Substitute det(B) = -5:

det(B⁻¹) = 1 / (-5)


Therefore:

det(B⁻¹) = -1/5


### Step 3: Calculate det(A⁴B⁻¹)

Now, multiply the two determinants:

det(A⁴B⁻¹) = det(A⁴) × det(B⁻¹)


Substitute the results:

det(A⁴B⁻¹) = 81 × (-1/5)


Multiply:

det(A⁴B⁻¹) = -81/5


Therefore:

det(A⁴B⁻¹) = -81/5


## 5. Check whether the inverse exists

The inverse B⁻¹ exists if and only if det(B) is not zero.

We are given:

det(B) = -5


Since:

-5 ≠ 0


Matrix B is invertible, so B⁻¹ exists.

Therefore, the determinant det(A⁴B⁻¹) is defined.


## Conclusion

The final results are:

det(AB) = -15

det(BA) = -15

det(A⁴B⁻¹) = -81/5


The first two determinants are equal because det(AB) = det(A)det(B) and det(BA) = det(B)det(A). Ordinary multiplication of numbers is commutative, even though matrix multiplication is not generally commutative.

The inverse B⁻¹ exists because det(B) = -5 is nonzero. This allows us to calculate det(A⁴B⁻¹) using the determinant properties for powers, inverses, and products.
