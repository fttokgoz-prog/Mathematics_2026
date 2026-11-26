
# EXERCISE 4 – GAUSS-JORDAN METHOD

## Question

Find A^(-1) using the Gauss-Jordan method for:

$$
A =
\begin{pmatrix}
1 & 2 \\
3 & 5
\end{pmatrix}
$$

Show the augmented matrix [A | I] after each successive operation and explain why obtaining I on the left gives the inverse on the right.

## Solution

### Step 1 – Initial Augmented Matrix

We start by writing the matrix A next to the identity matrix I.

$$
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
3 & 5 & 0 & 1
\end{array}
\right]
$$

### Step 2 – Eliminate the First Number in Row 2

Apply the row operation:

$$
R_2 \rightarrow R_2 - 3R_1
$$

The new augmented matrix is:

$$
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
0 & -1 & -3 & 1
\end{array}
\right]
$$

### Step 3 – Make the Pivot Equal to 1

Apply the row operation:

$$
R_2 \rightarrow -R_2
$$

The new augmented matrix is:

$$
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
0 & 1 & 3 & -1
\end{array}
\right]
$$

### Step 4 – Eliminate the Second Number in Row 1

Apply the row operation:

$$
R_1 \rightarrow R_1 - 2R_2
$$

The new augmented matrix is:

$$
\left[
\begin{array}{cc|cc}
1 & 0 & -5 & 2 \\
0 & 1 & 3 & -1
\end{array}
\right]
$$

### Step 5 – Final Result

The left side is now the identity matrix. Therefore, the right side is the inverse of the original matrix.

$$
A^{-1} =
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
$$

### Explanation

Each elementary row operation is equivalent to multiplying the original matrix by an elementary matrix.

If we apply all these operations to A, we obtain:

$$
EA = I
$$

Therefore:

$$
E = A^{-1}
$$

The same operations are applied to the identity matrix on the right side of the augmented matrix. As a result, when the left side becomes the identity matrix, the right side becomes the inverse of A.

This explains why:

$$
[A \mid I] \rightarrow [I \mid A^{-1}]
$$

