
# EXERCISE 9 – MATRIX EQUATION

## Given

$$
A =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix},
\qquad
B =
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

## Problem

Solve the matrix equation AX = B for X.

Before calculating, decide on which side of the equation A^(-1) must be used to isolate X. Explain why the order of multiplication matters.

After finding X, check the result by computing AX.

## Solution

### Step 1 – Decide Which Side to Use

We are given:

$$
AX = B
$$

Since A is on the left side of X, we must multiply both sides by A^(-1) from the left.

$$
A^{-1}AX = A^{-1}B
$$

Since A^(-1)A = I, we obtain:

$$
IX = A^{-1}B
$$

Therefore:

$$
X = A^{-1}B
$$

### Step 2 – Calculate the Inverse of A

$$
A^{-1} =
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
$$

### Step 3 – Calculate X

We substitute the matrices:

$$
X =
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

Multiply the matrices:

$$
X =
\begin{pmatrix}
1(3)+(-2)(2) & 1(1)+(-2)(4) \\
0(3)+1(2) & 0(1)+1(4)
\end{pmatrix}
$$

$$
X =
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
$$

### Step 4 – Check the Result

To verify our answer, we calculate AX.

$$
AX =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
$$

$$
AX =
\begin{pmatrix}
1(-1)+2(2) & 1(-7)+2(4) \\
0(-1)+1(2) & 0(-7)+1(4)
\end{pmatrix}
$$

$$
AX =
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

This is equal to the original matrix B.

### Final Answer

$$
\boxed{
X =
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
}
$$

### Explanation

The order of multiplication is important because matrix multiplication is not commutative.

In the equation AX = B, A^(-1) must be multiplied from the left because A is on the left side of X.

Multiplying from the right would not correctly isolate X.

The final check confirms that AX = B, so the solution is correct.
