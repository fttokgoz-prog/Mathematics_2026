# Exercise 15. Combining Determinant Properties

## Given

Let A and B be invertible 2 × 2 matrices with:

det(A) = -2

det(B) = 3


We need to compute:

det(B⁻¹AᵀB)


We must state the determinant properties used, in order, and explain why the factors involving B eventually cancel.

## 1. Apply the determinant property for a product

The determinant of a product of square matrices is equal to the product of their determinants.

The formula is:

det(XYZ) = det(X) × det(Y) × det(Z)


Applying this property to the given expression:

det(B⁻¹AᵀB) = det(B⁻¹) × det(Aᵀ) × det(B)


We now calculate each determinant separately.


## 2. Calculate det(B⁻¹)

For any invertible square matrix B, the determinant of its inverse is the reciprocal of the determinant of B.

The formula is:

det(B⁻¹) = 1 / det(B)


We are given:

det(B) = 3


Substitute this value:

det(B⁻¹) = 1 / 3


Therefore:

det(B⁻¹) = 1/3


## 3. Calculate det(Aᵀ)

An important determinant property states that the determinant of a matrix is equal to the determinant of its transpose.

The formula is:

det(Aᵀ) = det(A)


We are given:

det(A) = -2


Therefore:

det(Aᵀ) = -2


## 4. Substitute the determinant values

From the previous steps, we know that:

det(B⁻¹) = 1/3

det(Aᵀ) = -2

det(B) = 3


Substitute these values into the product formula:

det(B⁻¹AᵀB) = (1/3) × (-2) × 3


First, multiply the first two factors:

(1/3) × (-2) = -2/3


Then multiply by 3:

(-2/3) × 3 = -2


Therefore, the final answer is:

det(B⁻¹AᵀB) = -2


## 5. Explain why the factors involving B cancel

The original expression contains both B⁻¹ and B:

B⁻¹AᵀB


When calculating the determinant, these matrices contribute the factors:

det(B⁻¹) × det(B)


Using the inverse property:

det(B⁻¹) × det(B) = (1 / det(B)) × det(B)


Since det(B) = 3:

(1/3) × 3 = 1


Therefore, the factors involving B cancel each other in the determinant calculation.

The result becomes:

det(B⁻¹AᵀB) = 1 × det(Aᵀ)


Since det(Aᵀ) = det(A):

det(B⁻¹AᵀB) = det(A)


Finally:

det(B⁻¹AᵀB) = -2


It is important to note that we are cancelling the determinant factors, not rearranging the matrices themselves. Matrix multiplication is not generally commutative, but the determinants are ordinary numbers, so their factors can be rearranged.


## 6. List the determinant properties used

We used three main properties.

**Property 1: Determinant of a product**

det(XYZ) = det(X) × det(Y) × det(Z)


This allows us to separate the determinant of the product into three factors.


**Property 2: Determinant of an inverse**

det(B⁻¹) = 1 / det(B)


This gives the reciprocal of det(B), which cancels with det(B).


**Property 3: Determinant of a transpose**

det(Aᵀ) = det(A)


This means transposing A does not change its determinant.


## Conclusion

We were given:

det(A) = -2

det(B) = 3


Using the determinant properties:

det(B⁻¹AᵀB) = det(B⁻¹) × det(Aᵀ) × det(B)


Substituting the values:

det(B⁻¹AᵀB) = (1/3) × (-2) × 3

det(B⁻¹AᵀB) = -2


Therefore, the final answer is:

det(B⁻¹AᵀB) = -2


The factors involving B cancel because det(B⁻¹) = 1/det(B). The remaining determinant is det(Aᵀ), which equals det(A).
