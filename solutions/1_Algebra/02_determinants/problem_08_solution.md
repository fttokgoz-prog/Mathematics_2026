
# EXERCISE 8
# DETERMINANT OF A PRODUCT

---

## 1. GIVEN

Let A and B be square matrices of the same size, with the following determinants:

```math
\det(A)=3
```

```math
\det(B)=-5
```

We need to calculate:

1. $\det(AB)$
2. $\det(BA)$
3. $\det(A^{-1}B)$, if it exists.

We must also explain why the first two determinants are equal, even though matrix multiplication is generally not commutative.

---

## 2. IMPORTANT DETERMINANT PROPERTIES

We will use three important properties.

### Property 1 - Determinant of a Product

For two square matrices of the same size:

```math
\det(AB)=\det(A)\det(B)
```

### Property 2 - Determinant of an Inverse

If a matrix A is invertible, then:

```math
\det(A^{-1})=\frac{1}{\det(A)}
```

### Property 3 - Determinant of a Matrix Product

The determinant of a product is equal to the product of the individual determinants.

These properties allow us to calculate the required results without knowing the actual entries of A and B.

---

## 3. CALCULATE THE DETERMINANT OF AB

Using the determinant of a product:

```math
\det(AB)=\det(A)\det(B)
```

Substitute the given values:

```math
\det(AB)=3\cdot(-5)
```

Therefore:

```math
\det(AB)=-15
```

---

## 4. CALCULATE THE DETERMINANT OF BA

Using the same determinant property:

```math
\det(BA)=\det(B)\det(A)
```

Substitute the given values:

```math
\det(BA)=(-5)\cdot3
```

Therefore:

```math
\det(BA)=-15
```

---

## 5. WHY ARE THE FIRST TWO RESULTS EQUAL?

We have calculated:

```math
\det(AB)=-15
```

```math
\det(BA)=-15
```

Therefore:

```math
\det(AB)=\det(BA)
```

This happens because multiplication of real numbers is commutative:

```math
\det(A)\det(B)=\det(B)\det(A)
```

However, matrix multiplication itself is generally not commutative.

In other words:

```math
AB\neq BA
```

does not necessarily mean that:

```math
\det(AB)\neq\det(BA)
```

The matrices AB and BA can be different matrices while having the same determinant.

---

## 6. CALCULATE THE DETERMINANT OF A INVERSE TIMES B

We need to calculate:

```math
\det(A^{-1}B)
```

### STEP 1 - Check Whether A Is Invertible

A square matrix is invertible if its determinant is not zero.

We are given:

```math
\det(A)=3
```

Since 3 is not zero, A is invertible.

Therefore, $A^{-1}$ exists.

### STEP 2 - Calculate the Determinant of A Inverse

Using the inverse determinant property:

```math
\det(A^{-1})=\frac{1}{\det(A)}
```

Substitute the given value:

```math
\det(A^{-1})=\frac{1}{3}
```

### STEP 3 - Calculate the Determinant of A Inverse Times B

Using the product property:

```math
\det(A^{-1}B)=\det(A^{-1})\det(B)
```

Substitute the known values:

```math
\det(A^{-1}B)=\frac{1}{3}\cdot(-5)
```

Therefore:

```math
\det(A^{-1}B)=-\frac{5}{3}
```

---

## 7. SUMMARY OF THE RESULTS

| Expression | Determinant |
|---|---:|
| $\det(AB)$ | -15 |
| $\det(BA)$ | -15 |
| $\det(A^{-1}B)$ | -5/3 |

All three determinants are defined because A and B are square matrices of the same size, and A is invertible.

---

## 8. CONCLUSION

Using the properties of determinants, we obtained the following results:

```math
\det(AB)=-15
```

```math
\det(BA)=-15
```

```math
\det(A^{-1}B)=-\frac{5}{3}
```

The first two determinants are equal because multiplication of real numbers is commutative.

Although matrix multiplication is generally not commutative, the determinant of AB is always equal to the determinant of BA for square matrices of the same size.

Finally, since $\det(A)=3$ is non-zero, the inverse of A exists, allowing us to calculate the determinant of $A^{-1}B$.
