
# EXERCISE 15
# COMBINING DETERMINANT PROPERTIES

---

## 1. GIVEN

Let A and B be invertible 2×2 matrices with the following determinants:

```math
\det(A)=-2
```

```math
\det(B)=3
```

We need to calculate:

```math
\det(B^{-1}A^TB)
```

We must solve this problem without finding the individual entries of the matrices.

We must also:

1. State the determinant properties used, in the correct order.
2. Explain why the factors involving B eventually cancel.

---

## 2. IMPORTANT DETERMINANT PROPERTIES

Before solving the problem, we recall the following properties.

### Property 1 - Determinant of a Product

For square matrices of the same size:

```math
\det(ABC)=\det(A)\det(B)\det(C)
```

### Property 2 - Determinant of an Inverse

For an invertible matrix B:

```math
\det(B^{-1})=\frac{1}{\det(B)}
```

### Property 3 - Determinant of a Transpose

The determinant of a matrix is equal to the determinant of its transpose:

```math
\det(A^T)=\det(A)
```

These three properties are sufficient to solve the exercise.

---

## 3. APPLY THE PRODUCT PROPERTY

We start with the given expression:

```math
\det(B^{-1}A^TB)
```

Using the determinant of a product, we separate the three factors:

```math
=\det(B^{-1})\det(A^T)\det(B)
```

This allows us to calculate each determinant separately.

---

## 4. SUBSTITUTE THE KNOWN VALUES

We know that:

```math
\det(A)=-2
```

```math
\det(B)=3
```

First, calculate the determinant of the inverse of B:

```math
\det(B^{-1})=\frac{1}{\det(B)}
```

Substitute the known value:

```math
\det(B^{-1})=\frac{1}{3}
```

Next, use the transpose property:

```math
\det(A^T)=\det(A)=-2
```

Now substitute all three values into the original expression:

```math
\det(B^{-1}A^TB)
=
\frac{1}{3}\cdot(-2)\cdot3
```

---

## 5. EXPLAIN WHY THE FACTORS INVOLVING B CANCEL

The determinant of B is 3, while the determinant of its inverse is 1/3.

Their product is:

```math
\det(B^{-1})\det(B)
=
\frac{1}{3}\cdot3
```

Therefore:

```math
\det(B^{-1})\det(B)=1
```

The two factors involving B cancel each other.

Only the determinant of A transpose remains:

```math
\det(B^{-1}A^TB)=1\cdot(-2)
```

Therefore:

```math
\det(B^{-1}A^TB)=-2
```

---

## 6. SUMMARY OF THE PROPERTIES USED

| Step | Property | Result |
|---|---|---|
| 1 | Determinant of a product | Separate the three factors |
| 2 | Determinant of an inverse | det(B⁻¹) = 1/3 |
| 3 | Determinant of a transpose | det(Aᵀ) = -2 |
| 4 | Multiplication of determinants | (1/3) × (-2) × 3 = -2 |

---

## 7. FINAL RESULT

The required determinant is:

```math
\det(B^{-1}A^TB)=-2
```

---

## 8. CONCLUSION

We calculated the determinant without finding the individual entries of A or B.

We used the product property, the inverse property, and the transpose property of determinants.

The determinant of B inverse is the reciprocal of the determinant of B.

Therefore, the two factors involving B cancel each other.

The remaining determinant is equal to the determinant of A transpose, which is also equal to the determinant of A.

The final result is:

```math
\det(B^{-1}A^TB)=-2
```

This exercise demonstrates how several determinant properties can be combined to simplify a calculation without knowing the actual matrix entries.
