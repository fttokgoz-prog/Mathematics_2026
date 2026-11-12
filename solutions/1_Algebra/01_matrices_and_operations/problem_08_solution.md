
# EXERCISE 8
# ROW OPERATIONS AND THEIR REVERSIBILITY

---

## 1. GIVEN

We are given the following matrix:

```math
A =
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix}
```

We need to perform the following three row operations in order:

1. Subtract twice the first row from the second row.
2. Add the first row to the third row.
3. Interchange the second and third rows.

After each operation:

- Write the resulting matrix.
- State the inverse operation that reverses the transformation.
- Explain why the inverse operation restores the previous matrix.

---

## 2. FIRST ROW OPERATION

The first operation is:

```math
R_2 \leftarrow R_2-2R_1
```

The original rows are:

```math
R_1=(1,2,-1)
```

```math
R_2=(2,4,1)
```

Calculate the new second row:

```math
R_2=(2,4,1)-2(1,2,-1)
```

```math
R_2=(2,4,1)-(2,4,-2)
```

```math
R_2=(0,0,3)
```

The resulting matrix is:

```math
A_1=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3
\end{pmatrix}
```

### Inverse Operation

To reverse this operation, we add twice the first row to the second row.

```math
R_2 \leftarrow R_2+2R_1
```

This restores the original second row:

```math
(0,0,3)+2(1,2,-1)=(2,4,1)
```

Therefore, the inverse operation successfully restores the original matrix.

---

## 3. SECOND ROW OPERATION

Starting with matrix A₁, we perform:

```math
R_3 \leftarrow R_3+R_1
```

The current rows are:

```math
R_3=(-1,1,3)
```

```math
R_1=(1,2,-1)
```

Calculate the new third row:

```math
R_3=(-1,1,3)+(1,2,-1)
```

```math
R_3=(0,3,2)
```

The resulting matrix is:

```math
A_2=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2
\end{pmatrix}
```

### Inverse Operation

To reverse this operation, we subtract the first row from the third row.

```math
R_3 \leftarrow R_3-R_1
```

This restores the previous third row:

```math
(0,3,2)-(1,2,-1)=(-1,1,3)
```

Therefore, the inverse operation restores matrix A₁.

---

## 4. THIRD ROW OPERATION

Starting with matrix A₂, we interchange the second and third rows.

The operation is:

```math
R_2 \leftrightarrow R_3
```

Before the interchange:

```math
R_2=(0,0,3)
```

```math
R_3=(0,3,2)
```

After the interchange, the resulting matrix is:

```math
A_3=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}
```

### Inverse Operation

To reverse a row interchange, we simply interchange the same two rows again.

```math
R_2 \leftrightarrow R_3
```

This restores matrix A₂.

Therefore, swapping the same two rows twice returns the matrix to its previous state.

---

## 5. SUMMARY OF THE OPERATIONS AND THEIR INVERSES

| Step | Original Operation | Inverse Operation |
|---|---|---|
| 1 | R₂ ← R₂ − 2R₁ | R₂ ← R₂ + 2R₁ |
| 2 | R₃ ← R₃ + R₁ | R₃ ← R₃ − R₁ |
| 3 | R₂ ↔ R₃ | R₂ ↔ R₃ |

Each row operation has an inverse operation that restores the previous matrix.

---

## 6. FINAL RESULT

After performing all three row operations, we obtain:

```math
A_3=
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}
```

The three operations are reversible:

- The first operation is reversed by adding twice the first row to the second row.
- The second operation is reversed by subtracting the first row from the third row.
- The third operation is reversed by swapping the second and third rows again.

---

## 7. CONCLUSION

Elementary row operations are reversible transformations of a matrix.

Each operation has a corresponding inverse operation that restores the previous matrix.

This exercise demonstrates that row operations can be used to transform matrices in a controlled way without losing the ability to return to the original matrix.
