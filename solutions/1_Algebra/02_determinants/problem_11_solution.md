
# EXERCISE 11
# SHORTENING THE CALCULATION WITH ROW OPERATIONS

---

## 1. GIVEN

We are given the following 3×3 matrix:

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6
\end{pmatrix}
```

We need to calculate the determinant by first performing row operations that create as many zeros as possible.

We must also state which row operations do not change the determinant.

---

## 2. IMPORTANT ROW OPERATION PROPERTIES

There are three important elementary row operations:

1. Interchanging two rows changes the sign of the determinant.
2. Multiplying a row by a non-zero constant multiplies the determinant by that constant.
3. Adding a multiple of one row to another row does not change the determinant.

In this exercise, we will use the third operation to simplify the matrix without changing its determinant.

---

## 3. FIRST ROW OPERATION

Our original matrix is:

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6
\end{pmatrix}
```

First, subtract the first row from the second row:

```math
R_2 \leftarrow R_2-R_1
```

Calculate the new second row:

```math
(1,3,4)-(1,2,3)=(0,1,1)
```

The new matrix is:

```math
A_1 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 4 & 6
\end{pmatrix}
```

This operation does not change the determinant.

---

## 4. SECOND ROW OPERATION

Next, subtract the first row from the third row:

```math
R_3 \leftarrow R_3-R_1
```

Calculate the new third row:

```math
(1,4,6)-(1,2,3)=(0,2,3)
```

The resulting matrix is:

```math
A_2 =
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3
\end{pmatrix}
```

This operation also does not change the determinant.

---

## 5. THIRD ROW OPERATION

Now subtract twice the second row from the third row:

```math
R_3 \leftarrow R_3-2R_2
```

Calculate the new third row:

```math
(0,2,3)-2(0,1,1)
```

```math
=(0,2,3)-(0,2,2)
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

This operation does not change the determinant either.

---

## 6. CALCULATE THE DETERMINANT

The resulting matrix is an upper triangular matrix.

The determinant of a triangular matrix is equal to the product of its diagonal entries.

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

Therefore, the final result is:

```math
\det(A)=1
```

---

## 7. WHICH OPERATIONS DO NOT CHANGE THE DETERMINANT?

All three operations used in this exercise preserve the determinant.

| Row operation | Effect on determinant |
|---|---|
| R₂ ← R₂ − R₁ | No change |
| R₃ ← R₃ − R₁ | No change |
| R₃ ← R₃ − 2R₂ | No change |

This is because adding a multiple of one row to another row does not change the determinant.

---

## 8. CONCLUSION

We simplified the original matrix using three elementary row operations.

These operations created zeros below the main diagonal and transformed the matrix into upper triangular form.

Since adding a multiple of one row to another does not change the determinant, the determinant remained the same throughout the calculation.

The determinant was obtained by multiplying the diagonal entries of the triangular matrix.

The final result is:

```math
\det(A)=1
```

This exercise demonstrates how carefully chosen row operations can make determinant calculations shorter and easier.
