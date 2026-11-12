
# EXERCISE 7
# USING PROPERTIES INSTEAD OF RECOMPUTING

---

## 1. GIVEN

We are given a 3×3 matrix A with the following determinant:

```math
\det(A)=-4
```

We need to calculate:

- det(2A)
- det(Aᵀ)
- det(A²)
- det(-A)

We will use determinant properties instead of calculating each determinant from scratch.

---

## 2. DETERMINANT OF 2A

One important property states that for an n×n matrix:

```math
\det(kA)=k^n\det(A)
```

Since A is a 3×3 matrix, n = 3.

Therefore:

```math
\det(2A)=2^3\det(A)
```

Substitute the given determinant:

```math
\det(2A)=8\cdot(-4)
```

Therefore:

```math
\boxed{\det(2A)=-32}
```

---

## 3. DETERMINANT OF THE TRANSPOSE

The determinant of a matrix is equal to the determinant of its transpose.

The property is:

```math
\det(A^T)=\det(A)
```

Since:

```math
\det(A)=-4
```

We obtain:

```math
\boxed{\det(A^T)=-4}
```

---

## 4. DETERMINANT OF A²

The determinant of a product of two square matrices is equal to the product of their determinants.

The property is:

```math
\det(AB)=\det(A)\det(B)
```

Therefore:

```math
\det(A^2)=\det(A\cdot A)
```

Using the property:

```math
\det(A^2)=\det(A)\cdot\det(A)
```

Substitute the given value:

```math
\det(A^2)=(-4)\cdot(-4)
```

Therefore:

```math
\boxed{\det(A^2)=16}
```

---

## 5. DETERMINANT OF -A

For an n×n matrix, multiplying the matrix by -1 gives:

```math
\det(-A)=(-1)^n\det(A)
```

Since A is a 3×3 matrix:

```math
\det(-A)=(-1)^3\det(A)
```

Substitute the given determinant:

```math
\det(-A)=-1\cdot(-4)
```

Therefore:

```math
\boxed{\det(-A)=4}
```

---

## 6. SUMMARY OF THE RESULTS

| Expression | Determinant |
|---|---:|
| det(2A) | -32 |
| det(Aᵀ) | -4 |
| det(A²) | 16 |
| det(-A) | 4 |

---

## 7. CONCLUSION

We used four important properties of determinants to calculate the required results without recomputing the original determinant.

The final answers are:

```math
\boxed{
\begin{aligned}
\det(2A)&=-32\\
\det(A^T)&=-4\\
\det(A^2)&=16\\
\det(-A)&=4
\end{aligned}
}
```

These properties make determinant calculations faster and easier, especially when working with larger matrices.
