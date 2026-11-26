
# EXERCISE 13 – UNDOING A COMPOSITE TRANSFORMATION

## Given

The matrices are:

$$
S =
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix},
\qquad
H =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Describe nonuniform scaling and shear.

For T = HS, find T^(-1) in two ways:

1. First compute T, then calculate its inverse.
2. Use the formula (HS)^(-1) = S^(-1)H^(-1).

Compare the results. Additionally, compute H^(-1)S^(-1) and verify that the incorrect order gives a different matrix.

Explain why undoing a composition reverses the operation order.

## Solution

### Step 1 – Calculate T = HS

$$
T =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
$$

$$
T =
\begin{pmatrix}
2 & 1 \\
0 & 1
\end{pmatrix}
$$

### Step 2 – First Method: Calculate the Inverse of T

For a 2x2 matrix:

$$
A^{-1} =
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

The determinant of T is:

$$
\det(T) = (2)(1)-(1)(0)=2
$$

Therefore:

$$
T^{-1} =
\frac{1}{2}
\begin{pmatrix}
1 & -1 \\
0 & 2
\end{pmatrix}
$$

$$
T^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
$$

### Step 3 – Second Method: Use the Inverse Product Rule

The inverse matrices are:

$$
S^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
$$

$$
H^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

Using the inverse product rule:

$$
(HS)^{-1} = S^{-1}H^{-1}
$$

Substitute the matrices:

$$
T^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

$$
T^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
$$

Both methods give the same result.

### Step 4 – Check the Incorrect Order

Now calculate H^(-1)S^(-1):

$$
H^{-1}S^{-1} =
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
$$

$$
H^{-1}S^{-1} =
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1
\end{pmatrix}
$$

This is different from the correct inverse:

$$
T^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
$$

Therefore, the order of multiplication cannot be changed.

### Step 5 – Explanation

When we multiply T = HS, the scaling transformation S is applied first, followed by the shear transformation H.

To undo these operations, we must reverse their order.

First, we undo the shear using H^(-1), and then we undo the scaling using S^(-1).

This is why the inverse of a product reverses the multiplication order:

$$
(HS)^{-1} = S^{-1}H^{-1}
$$

### Final Answer

$$
\boxed{
T^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
}
$$
