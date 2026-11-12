
# EXERCISE 13
# DETERMINANT BY ELIMINATION

---

## 1. GIVEN

We are given the following 3×3 matrix:

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2
\end{pmatrix}
```

We need to compute the determinant using Gaussian elimination.

During the calculation, we must record every row operation and explain its effect on the determinant.

---

## 2. IMPORTANT ROW OPERATION PROPERTIES

Before starting, we recall three important properties:

1. Swapping two rows changes the sign of the determinant.
2. Multiplying a row by a non-zero constant multiplies the determinant by that constant.
3. Adding a multiple of one row to another row does not change the determinant.

In this exercise, we will use row replacement operations, so the determinant will remain unchanged throughout the elimination.

---

## 3. FIRST ROW OPERATION

Start with the original matrix:

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 5 & 7 \\
1 & 0 & 2
\end{pmatrix}
```

We want to create a zero below the first diagonal entry.

Perform the operation:

```math
R_2 \leftarrow R_2-2R_1
```

Calculate the new second row:

```math
(2,5,7)-2(1,2,3)
```

```math
=(2,5,7)-(2,4,6)
```

```math
=(0,1,1)
```

The resulting matrix is:

```math
A_1 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 0 & 2
\end{pmatrix}
```

**Effect on the determinant:**

Adding a multiple of one row to another does not change the determinant.

Therefore:

```math
\det(A_1)=\det(A)
```

---

## 4. SECOND ROW OPERATION

Next, we create a zero in the first column of the third row.

Perform the operation:

```math
R_3 \leftarrow R_3-R_1
```

Calculate the new third row:

```math
(1,0,2)-(1,2,3)
```

```math
=(0,-2,-1)
```

The resulting matrix is:

```math
A_2 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & -2 & -1
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

Now we create a zero below the second diagonal entry.

Perform the operation:

```math
R_3 \leftarrow R_3+2R_2
```

Calculate the new third row:

```math
(0,-2,-1)+2(0,1,1)
```

```math
=(0,-2,-1)+(0,2,2)
```

```math
=(0,0,1)
```

The resulting matrix is:

```math
A_3 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 0 & 1
\end{pmatrix}
```

**Effect on the determinant:**

Adding twice the second row to the third row does not change the determinant.

Therefore:

```math
\det(A_3)=\det(A_2)
```

---

## 6. CALCULATE THE FINAL DETERMINANT

The resulting matrix is now upper triangular.

For an upper triangular matrix, the determinant is equal to the product of its diagonal entries.

Therefore:

```math
\det(A_3)=1\cdot1\cdot1
```

```math
\det(A_3)=1
```

Since none of our row operations changed the determinant:

```math
\det(A)=\det(A_3)
```

The final result is:

```math
\det(A)=1
```

---

## 7. SUMMARY OF ROW OPERATIONS

| Step | Row operation | Effect on determinant |
|---|---|---|
| 1 | R₂ ← R₂ − 2R₁ | No change |
| 2 | R₃ ← R₃ − R₁ | No change |
| 3 | R₃ ← R₃ + 2R₂ | No change |

All three operations are row replacement operations.

Therefore, the determinant remains unchanged throughout the entire elimination process.

---

## 8. CONCLUSION

We calculated the determinant by transforming the original matrix into upper triangular form.

We used three elementary row operations, and none of them changed the determinant.

The determinant of the final triangular matrix is the product of its diagonal entries.

Therefore, the determinant of the original matrix is:

```math
\det(A)=1
```

This exercise demonstrates how Gaussian elimination can simplify determinant calculations while preserving the determinant through appropriate row operations.
