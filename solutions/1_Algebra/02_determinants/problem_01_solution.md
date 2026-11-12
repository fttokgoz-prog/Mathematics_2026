
# EXERCISE 1
# DETERMINANT OF A 2×2 MATRIX

---

## 1. GIVEN

We are given two matrices.

### Matrix A

```math
A =
\begin{pmatrix}
3 & -2 \\
5 & 4
\end{pmatrix}
```

### Matrix B

```math
B =
\begin{pmatrix}
1 & 7 \\
2 & 14
\end{pmatrix}
```

Calculate the determinant of each matrix and determine which matrix is invertible. Justify your answer.

---

## 2. DETERMINANT FORMULA

For a 2×2 matrix:

```math
M =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
```

The determinant is calculated using:

```math
\det(M)=ad-bc
```

A matrix is invertible if and only if its determinant is not zero.

---

## 3. DETERMINANT OF MATRIX A

Using the determinant formula:

```math
\det(A)=(3)(4)-(-2)(5)
```

Calculate:

```math
\det(A)=12+10
```

Therefore:

```math
\boxed{\det(A)=22}
```

Since the determinant is not zero, matrix A is invertible.

---

## 4. DETERMINANT OF MATRIX B

Using the determinant formula:

```math
\det(B)=(1)(14)-(7)(2)
```

Calculate:

```math
\det(B)=14-14
```

Therefore:

```math
\boxed{\det(B)=0}
```

Since the determinant is zero, matrix B is not invertible.

---

## 5. COMPARISON OF THE RESULTS

| Matrix | Determinant | Invertible? |
|---|---:|---|
| A | 22 | Yes |
| B | 0 | No |

Matrix A has a non-zero determinant, while matrix B has a zero determinant.

Therefore, only matrix A is invertible.

---

## 6. CONCLUSION

The determinant determines whether a square matrix has an inverse.

- If the determinant is non-zero, the matrix is invertible.
- If the determinant is zero, the matrix is not invertible.

In this exercise, matrix A is invertible, while matrix B is not.
