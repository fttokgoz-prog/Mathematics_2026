
# EXERCISE 10
# DETECTING DEPENDENCE

---

## 1. GIVEN

We are given the following 3×3 matrix:

```math
A =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5
\end{pmatrix}
```

We need to:

1. Explain why the determinant of A is zero without performing a full determinant calculation.
2. Identify a specific linear dependence between the rows.
3. Explain how this dependence is related to the invertibility of the matrix.

---

## 2. IDENTIFY THE ROWS

The three rows of matrix A are:

```math
R_1=(1,2,3)
```

```math
R_2=(2,4,6)
```

```math
R_3=(0,1,5)
```

We can observe that the second row is exactly twice the first row.

In other words:

```math
R_2=2R_1
```

This means that the first and second rows are linearly dependent.

---

## 3. WHY IS THE DETERMINANT ZERO?

A determinant is zero whenever the rows or columns of a square matrix are linearly dependent.

In our matrix:

```math
R_2=2R_1
```

Therefore, two rows are proportional.

This means that the rows cannot be linearly independent.

As a result:

```math
\det(A)=0
```

We can conclude this directly from the structure of the matrix without calculating the full determinant.

---

## 4. CONNECTION WITH INVERTIBILITY

A square matrix is invertible if and only if its determinant is non-zero.

The condition is:

```math
\det(A)\neq0
```

However, we have established that:

```math
\det(A)=0
```

Therefore, matrix A is not invertible.

In other words, the inverse matrix A⁻¹ does not exist.

---

## 5. CONCLUSION

The second row of matrix A is twice the first row.

This creates a linear dependence between the rows.

A square matrix with linearly dependent rows has a determinant equal to zero.

Since the determinant is zero, the matrix is singular and cannot be inverted.

The final result is:

```math
\det(A)=0
```

Matrix A is not invertible because its rows are linearly dependent.
