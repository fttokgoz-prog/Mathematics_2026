# Exercise 2. Addition and Scalar Multiplication

## Given

The following matrices are given:

$$
A =
\begin{pmatrix}
1 & 2 \\
-1 & 3
\end{pmatrix}
$$

$$
B =
\begin{pmatrix}
4 & -2 \\
0 & 5
\end{pmatrix}
$$

## Questions

Compute the following matrix operations:

1. \(A+B\)
2. \(A-B\)
3. \(3A-2B\)

Explain why matrix addition is possible only for matrices of the same size.

## Solution

### 1. Matrix Addition: A + B

Add the corresponding entries of both matrices:

$$
A+B =
\begin{pmatrix}
1+4 & 2+(-2) \\
-1+0 & 3+5
\end{pmatrix}
$$

$$
\boxed{
A+B =
\begin{pmatrix}
5 & 0 \\
-1 & 8
\end{pmatrix}
}
$$

### 2. Matrix Subtraction: A - B

Subtract the corresponding entries:

$$
A-B =
\begin{pmatrix}
1-4 & 2-(-2) \\
-1-0 & 3-5
\end{pmatrix}
$$

$$
\boxed{
A-B =
\begin{pmatrix}
-3 & 4 \\
-1 & -2
\end{pmatrix}
}
$$

### 3. Scalar Multiplication: 3A - 2B

First, multiply every entry of matrix A by 3:

$$
3A =
\begin{pmatrix}
3 & 6 \\
-3 & 9
\end{pmatrix}
$$

Next, multiply every entry of matrix B by 2:

$$
2B =
\begin{pmatrix}
8 & -4 \\
0 & 10
\end{pmatrix}
$$

Now subtract the matrices:

$$
3A-2B =
\begin{pmatrix}
3-8 & 6-(-4) \\
-3-0 & 9-10
\end{pmatrix}
$$

$$
\boxed{
3A-2B =
\begin{pmatrix}
-5 & 10 \\
-3 & -1
\end{pmatrix}
}
$$

### 4. Explanation

Matrix addition is possible only when both matrices have the same number of rows and columns.

This is because matrix addition is performed by adding corresponding entries.

If the matrices have different sizes, their corresponding entries cannot be matched correctly.

In this exercise, both matrices have size \(2 \times 2\), so addition and subtraction are possible.

## Final Answers

$$
A+B =
\begin{pmatrix}
5 & 0 \\
-1 & 8
\end{pmatrix}
$$

$$
A-B =
\begin{pmatrix}
-3 & 4 \\
-1 & -2
\end{pmatrix}
$$

$$
3A-2B =
\begin{pmatrix}
-5 & 10 \\
-3 & -1
\end{pmatrix}
$$
