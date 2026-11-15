
# EXERCISE 9 – MATRIX EQUATION

## 1. GIVEN

We are given the matrix equation:

$$
AX=B
$$

Where:

$$
A =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
$$

And:

$$
B =
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

Our task is to find matrix X and verify the result by calculating AX.

## 2. DECIDING WHICH SIDE TO USE

Since A is on the left side of X in the equation AX = B, we must multiply both sides by A⁻¹ on the left.

We obtain:

$$
A^{-1}(AX)=A^{-1}B
$$

Using the associative property of matrix multiplication:

$$
(A^{-1}A)X=A^{-1}B
$$

Since:

$$
A^{-1}A=I
$$

We get:

$$
IX=A^{-1}B
$$

Therefore:

$$
\boxed{X=A^{-1}B}
$$

## 3. CALCULATING THE INVERSE OF A

First, we calculate the determinant of A.

$$
\det(A)=1(1)-2(0)
$$

$$
\det(A)=1
$$

Since the determinant is not zero, the inverse exists.

Using the 2×2 inverse formula:

$$
A^{-1}=
\frac{1}{1}
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A^{-1}=
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
}
$$

## 4. CALCULATING X

We use the formula:

$$
X=A^{-1}B
$$

Substituting the matrices:

$$
X=
\begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

Calculating each element:

$$
X=
\begin{pmatrix}
1(3)+(-2)(2) & 1(1)+(-2)(4) \\
0(3)+1(2) & 0(1)+1(4)
\end{pmatrix}
$$

Simplifying:

$$
X=
\begin{pmatrix}
3-4 & 1-8 \\
2 & 4
\end{pmatrix}
$$

Therefore, the solution is:

$$
\boxed{
X=
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
}
$$

## 5. VERIFICATION BY CALCULATING AX

To verify our result, we substitute X into the original equation AX = B.

$$
AX=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
$$

Calculating each element:

$$
AX=
\begin{pmatrix}
1(-1)+2(2) & 1(-7)+2(4) \\
0(-1)+1(2) & 0(-7)+1(4)
\end{pmatrix}
$$

Simplifying:

$$
AX=
\begin{pmatrix}
-1+4 & -7+8 \\
2 & 4
\end{pmatrix}
$$

Therefore:

$$
AX=
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

This is exactly equal to matrix B.

$$
\boxed{AX=B}
$$

The result is correct.

## 6. CONCLUSION

We solved the matrix equation AX = B by multiplying both sides by A⁻¹ on the left.

The inverse was calculated successfully, and we found:

$$
\boxed{
X=
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
}
$$

Finally, we verified the result by calculating AX.

Since AX is equal to B, our solution is correct.

The important rule is that when solving AX = B, we multiply by A⁻¹ on the left:

$$
\boxed{X=A^{-1}B}
$$
