
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

Perform the following three row operations in the given order:

1. $R_2 \leftarrow R_2-2R_1$
2. $R_3 \leftarrow R_3+R_1$
3. Interchange $R_2$ and $R_3$.

For each of the three operations:

- Write the resulting matrix after performing the operation.
- State an inverse row operation that reverses it.
- Explain how the inverse operation restores the previous matrix.

Finally, explain why elementary row operations are reversible transformations.

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

Therefore:

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

Verification:

```math
(0,0,3)+2(1,2,-1)=(2,4,1)
```

This restores the original second row and therefore the original matrix.

---

## 3. SECOND ROW OPERATION

Starting with matrix $A_1$, perform:

```math
R_3 \leftarrow R_3+R_1
```

The current third row is:

```math
R_3=(-1,1,3)
```

Calculate the new third row:

```math
R_3=(-1,1,3)+(1,2,-1)
```

Therefore:

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

To reverse this operation, subtract the first row from the third row.

```math
R_3 \leftarrow R_3-R_1
```

Verification:

```math
(0,3,2)-(1,2,-1)=(-1,1,3)
```

This restores the previous third row and therefore matrix $A_1$.

---

## 4. THIRD ROW OPERATION

Starting with matrix $A_2$, interchange the second and third rows.

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

To reverse a row interchange, we interchange the same two rows again.

```math
R_2 \leftrightarrow R_3
```

Swapping the same two rows twice restores the previous matrix $A_2$.

---

## 5. SUMMARY OF OPERATIONS AND THEIR INVERSES

| Step | Original operation | Inverse operation |
|---|---|---|
| 1 | $R_2 \leftarrow R_2-2R_1$ | $R_2 \leftarrow R_2+2R_1$ |
| 2 | $R_3 \leftarrow R_3+R_1$ | $R_3 \leftarrow R_3-R_1$ |
| 3 | $R_2 \leftrightarrow R_3$ | $R_2 \leftrightarrow R_3$ |

Each inverse operation restores the matrix to the state it had immediately before the corresponding original operation.

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

The three inverse operations, applied in reverse order, restore the original matrix.

The reverse sequence is:

1. Interchange $R_2$ and $R_3$.
2. Perform $R_3 \leftarrow R_3-R_1$.
3. Perform $R_2 \leftarrow R_2+2R_1$.

---

## 7. CONCLUSION

Elementary row operations are reversible transformations of a matrix.

In this exercise, we performed two row replacement operations and one row interchange.

Each operation has an inverse that restores the previous matrix.

This demonstrates that row operations can transform a matrix in a controlled way while preserving the ability to return to its original form.
