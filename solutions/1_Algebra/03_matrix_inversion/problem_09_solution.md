
# EXERCISE 9 – MATRIX EQUATION

## 1. GIVEN

We are given the matrix equation:

$$
AX=B
$$

Where:

$$
A=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
$$

And:

$$
B=
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}
$$

Our task is to find matrix X and verify the result by calculating AX.

## 2. DECIDING WHICH SIDE TO USE BEFORE CALCULATING

Before calculating the inverse, we must determine on which side A⁻¹ should be applied.

The original equation is:

$$
AX=B
$$

Matrix A is on the left side of X.

Therefore, we must multiply both sides of the equation by A⁻¹ ON THE LEFT.

We obtain:

$$
A^{-1}(AX)=A^{-1}B
$$

Using the associative property:

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

We must not multiply by A⁻¹ on the right because matrix multiplication is not generally commutative.

## 3. CALCULATING THE INVERSE OF A

Now, we calculate the inverse of matrix A.

First, we calculate its determinant:

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

We use the formula determined earlier:

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

Therefore:

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

To verify our result, we substitute the calculated matrix X into the original equation AX = B.

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

We solved the matrix equation AX = B.

Before calculating the inverse, we determined that A⁻¹ must be applied on the left side because A is on the left side of X.

We obtained:

$$
X=A^{-1}B
$$

The final solution is:

$$
\boxed{
X=
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
}
$$

Finally, we verified the solution by calculating AX and confirmed that it is equal to B.
