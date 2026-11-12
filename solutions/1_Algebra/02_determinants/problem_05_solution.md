
# EXERCISE 5
# ROW OPERATIONS

---

## 1. GIVEN

We are given the following matrix:

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
```

We need to calculate det(A) by simplifying the matrix using row operations and explain how each operation affects the determinant.

---

## 2. INITIAL MATRIX

The initial matrix is:

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
```

We will use row replacement operations to transform the matrix into upper triangular form.

Adding a multiple of one row to another row does not change the determinant.

---

## 3. FIRST ROW OPERATION

We perform the following operation:

```math
R_2 \leftarrow R_2-2R_1
```

Calculate the new second row:

```math
(2,1,0)-2(1,2,3)
```

```math
=(2,1,0)-(2,4,6)
```

```math
=(-3,-3,-6)
```

The resulting matrix is:

```math
A_1 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2
\end{pmatrix}
```

**Effect on the determinant:**

Adding a multiple of one row to another row does not change the determinant.

Therefore:

```math
\det(A_1)=\det(A)
```

---

## 4. SECOND ROW OPERATION

We perform the following operation:

```math
R_3 \leftarrow R_3+R_1
```

Calculate the new third row:

```math
(-1,4,2)+(1,2,3)
```

```math
=(0,6,5)
```

The resulting matrix is:

```math
A_2 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5
\end{pmatrix}
```

**Effect on the determinant:**

This is also a row replacement operation.

Therefore, the determinant does not change:

```math
\det(A_2)=\det(A_1)
```

---

## 5. THIRD ROW OPERATION

We perform the following operation:

```math
R_3 \leftarrow R_3+2R_2
```

Calculate the new third row:

```math
(0,6,5)+2(0,-3,-6)
```

```math
=(0,6,5)+(0,-6,-12)
```

```math
=(0,0,-7)
```

The resulting upper triangular matrix is:

```math
A_3 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7
\end{pmatrix}
```

**Effect on the determinant:**

Adding a multiple of one row to another does not change the determinant.

Therefore:

```math
\det(A_3)=\det(A_2)
```

---

## 6. CALCULATE THE FINAL DETERMINANT

The matrix is now in upper triangular form.

The determinant of a triangular matrix is equal to the product of its main diagonal entries.

Therefore:

```math
\det(A_3)=1\cdot(-3)\cdot(-7)
```

Calculate:

```math
\det(A_3)=21
```

Since none of our row operations changed the determinant:

```math
\det(A)=\det(A_3)
```

The final answer is:

```math
\boxed{\det(A)=21}
```

---

## 7. SUMMARY OF ROW OPERATIONS

| Step | Row Operation | Effect on Determinant |
|---|---|---|
| 1 | R₂ ← R₂ − 2R₁ | No change |
| 2 | R₃ ← R₃ + R₁ | No change |
| 3 | R₃ ← R₃ + 2R₂ | No change |

All three operations are row replacements, so the determinant remains unchanged throughout the calculation.

---

## 8. CONCLUSION

We simplified the original matrix into upper triangular form using three row replacement operations.

None of these operations changed the determinant.

By multiplying the entries on the main diagonal, we obtained:

```math
\boxed{\det(A)=21}
```

This demonstrates how row operations can simplify determinant calculations while preserving the determinant's value.
