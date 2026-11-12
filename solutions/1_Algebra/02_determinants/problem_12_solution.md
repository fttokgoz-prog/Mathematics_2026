
# EXERCISE 12
# A PARAMETER REVEALED BY A ROW OPERATION

---

## 1. GIVEN

We are given a matrix depending on the parameter t:

```math
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1
\end{pmatrix}
```

We need to find all values of t for which the matrix is not invertible.

Before calculating the determinant, we must perform the following row operation:

```math
R_2 \leftarrow R_2-2R_1
```

We must use the resulting matrix to identify the required value of t.

Finally, we must explain what special relationship appears between the rows for this value.

---

## 2. APPLY THE ROW OPERATION

The original matrix is:

```math
A(t)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1
\end{pmatrix}
```

We perform the operation:

```math
R_2 \leftarrow R_2-2R_1
```

The first row remains unchanged:

```math
R_1=(1,2,3)
```

Calculate the new second row:

```math
R_2=(2,4,t)-2(1,2,3)
```

Distribute the multiplication:

```math
R_2=(2,4,t)-(2,4,6)
```

Therefore:

```math
R_2=(0,0,t-6)
```

The third row remains unchanged:

```math
R_3=(0,1,1)
```

The resulting matrix is:

```math
A_1(t)=
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1
\end{pmatrix}
```

---

## 3. FIND THE VALUE OF t

A square matrix is not invertible if and only if its determinant is zero.

The row operation we performed does not change the determinant because we only subtracted a multiple of one row from another.

Therefore:

```math
\det(A(t))=\det(A_1(t))
```

We calculate the determinant of the resulting matrix by expanding along the first column:

```math
\det(A_1(t))=
1\begin{vmatrix}
0 & t-6 \\
1 & 1
\end{vmatrix}
```

Calculate the 2×2 determinant:

```math
\det(A_1(t))=1(0\cdot1-(t-6)\cdot1)
```

Simplifying:

```math
\det(A_1(t))=6-t
```

For the matrix to be non-invertible, its determinant must equal zero:

```math
6-t=0
```

Solving for t:

```math
t=6
```

Therefore, the matrix is not invertible when t equals 6.

---

## 4. WHAT HAPPENS WHEN t = 6?

Substitute t = 6 into the resulting matrix:

```math
A_1(6)=
\begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & 0 \\
0 & 1 & 1
\end{pmatrix}
```

The second row becomes a zero row.

This means that the rows are linearly dependent.

We can also examine the original matrix when t = 6:

```math
A(6)=
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 1
\end{pmatrix}
```

Notice that the second row is exactly twice the first row:

```math
R_2=2R_1
```

Therefore, the original matrix has linearly dependent rows.

A square matrix with linearly dependent rows has a determinant equal to zero and cannot be inverted.

---

## 5. SUMMARY OF THE RESULTS

| Condition | Result |
|---|---|
| Row operation | R₂ ← R₂ − 2R₁ |
| New second row | (0, 0, t − 6) |
| Determinant | 6 − t |
| Non-invertible value | t = 6 |
| Special property | Second row becomes twice the first row in the original matrix |

---

## 6. CONCLUSION

We used an elementary row operation to simplify the matrix and identify the value of the parameter.

The determinant of the matrix is:

```math
\det(A(t))=6-t
```

The matrix is not invertible when its determinant is zero.

Therefore, the only required value is:

```math
t=6
```

For this value, the second row of the original matrix is twice the first row.

After the row operation, the second row becomes a zero row.

This demonstrates that linear dependence between rows causes the determinant to be zero, making the matrix non-invertible.
