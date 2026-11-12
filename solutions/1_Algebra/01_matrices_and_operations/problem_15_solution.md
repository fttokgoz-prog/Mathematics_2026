
# EXERCISE 15
# ASSOCIATIVITY OF MULTIPLICATION AND DIFFERENT CALCULATION PATHS

---

## 1. GIVEN

We are given three matrices:

Matrix A:

```math
A =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
```

Matrix B:

```math
B =
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
```

Matrix C:

```math
C =
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
```

We need to calculate:

- (AB)C
- A(BC)

Then compare the results and the number of intermediate operations.

---

## 2. FIRST CALCULATION PATH: (AB)C

### STEP 1 - Calculate AB

Multiply matrix A by matrix B.

```math
AB =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
```

Calculate each entry:

```math
AB =
\begin{pmatrix}
1+4+0 & 0+2+0 \\
0+2-1 & 0+1+3
\end{pmatrix}
```

The result is:

```math
AB =
\begin{pmatrix}
5 & 2 \\
1 & 4
\end{pmatrix}
```

### STEP 2 - Calculate (AB)C

Now multiply the result by matrix C.

```math
(AB)C =
\begin{pmatrix}
5 & 2 \\
1 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
```

Calculate:

```math
(AB)C =
\begin{pmatrix}
10 & 5-2 \\
2 & 1-4
\end{pmatrix}
```

The final result of the first path is:

```math
\boxed{
(AB)C =
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
}
```

---

## 3. SECOND CALCULATION PATH: A(BC)

### STEP 1 - Calculate BC

First, multiply matrix B by matrix C.

```math
BC =
\begin{pmatrix}
1 & 0 \\
2 & 1 \\
-1 & 3
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
0 & -1
\end{pmatrix}
```

Calculate each entry:

```math
BC =
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4
\end{pmatrix}
```

### STEP 2 - Calculate A(BC)

Now multiply matrix A by the result of BC.

```math
A(BC) =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
4 & 1 \\
-2 & -4
\end{pmatrix}
```

Calculate:

```math
A(BC) =
\begin{pmatrix}
2+8+0 & 1+2+0 \\
0+4-2 & 0+1-4
\end{pmatrix}
```

The final result of the second path is:

```math
\boxed{
A(BC) =
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
}
```

---

## 4. COMPARISON OF THE RESULTS

The first calculation path gives:

```math
(AB)C =
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
```

The second calculation path gives:

```math
A(BC) =
\begin{pmatrix}
10 & 3 \\
2 & -3
\end{pmatrix}
```

Both paths produce exactly the same matrix.

Therefore:

```math
\boxed{(AB)C=A(BC)}
```

This demonstrates the associativity of matrix multiplication.

---

## 5. COMPARISON OF INTERMEDIATE OPERATIONS

Both calculation paths require two matrix multiplications.

However, the dimensions of the intermediate matrices are different.

### First Path: (AB)C

1. Multiply a 2 × 3 matrix by a 3 × 2 matrix.
2. Obtain a 2 × 2 intermediate matrix.
3. Multiply the 2 × 2 result by another 2 × 2 matrix.

Scalar operation counts:

- First multiplication: 12 multiplications and 8 additions.
- Second multiplication: 8 multiplications and 4 additions.

Total:

- 20 scalar multiplications.
- 12 scalar additions.

### Second Path: A(BC)

1. Multiply a 3 × 2 matrix by a 2 × 2 matrix.
2. Obtain a 3 × 2 intermediate matrix.
3. Multiply the 2 × 3 matrix by the 3 × 2 result.

Scalar operation counts:

- First multiplication: 12 multiplications and 6 additions.
- Second multiplication: 12 multiplications and 8 additions.

Total:

- 24 scalar multiplications.
- 14 scalar additions.

### Summary Table

| Calculation Path | Multiplications | Additions |
|---|---:|---:|
| (AB)C | 20 | 12 |
| A(BC) | 24 | 14 |

The first calculation path requires fewer scalar operations for these matrices.

---

## 6. CONCLUSION

Matrix multiplication is associative, which means that changing the grouping of three matrices does not change the final result.

Therefore:

```math
\boxed{(AB)C=A(BC)}
```

However, different calculation paths can require different numbers of operations.

In this example, calculating AB first is more efficient than calculating BC first.

This shows that associativity guarantees the same mathematical result, but choosing the calculation order can affect computational efficiency.
