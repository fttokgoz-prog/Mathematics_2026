
# EXERCISE 6 – SOLVING A SYSTEM USING THE INVERSE

## 1. GIVEN

We are given the linear system:

$$
Ax=b
$$

Where:

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
$$

And:

$$
b=
\begin{pmatrix}
5 \\
7
\end{pmatrix}
$$

Our task is to solve the system using:

$$
x=A^{-1}b
$$

After finding the solution, we must substitute the resulting vector back into the original equation Ax = b to verify the result.

## 2. CALCULATING THE INVERSE OF A

First, we calculate the determinant of A.

$$
\det(A)=2(3)-1(1)
$$

$$
\det(A)=6-1=5
$$

Since the determinant is not equal to zero, the inverse exists.

Using the 2×2 inverse formula:

$$
A^{-1}=
\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
$$

Therefore:

$$
A^{-1}=
\begin{pmatrix}
\frac{3}{5} & -\frac{1}{5} \\
-\frac{1}{5} & \frac{2}{5}
\end{pmatrix}
$$

## 3. SOLVING THE SYSTEM USING x = A⁻¹b

We use the formula:

$$
x=A^{-1}b
$$

Substituting the matrices:

$$
x=
\begin{pmatrix}
\frac{3}{5} & -\frac{1}{5} \\
-\frac{1}{5} & \frac{2}{5}
\end{pmatrix}
\begin{pmatrix}
5 \\
7
\end{pmatrix}
$$

Calculating each element:

$$
x=
\begin{pmatrix}
\frac{3}{5}(5)-\frac{1}{5}(7) \\
-\frac{1}{5}(5)+\frac{2}{5}(7)
\end{pmatrix}
$$

Simplifying:

$$
x=
\begin{pmatrix}
\frac{15-7}{5} \\
\frac{-5+14}{5}
\end{pmatrix}
$$

Therefore, the solution is:

$$
\boxed{
x=
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix}
}
$$

## 4. VERIFICATION BY SUBSTITUTION

To verify the obtained solution, we substitute the vector x back into the original equation:

$$
Ax=b
$$

We have found:

$$
x=
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix}
$$

Now, we substitute this vector into the equation:

$$
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix}
=
\begin{pmatrix}
5 \\
7
\end{pmatrix}
$$

Calculating the matrix multiplication:

$$
\begin{pmatrix}
2(\frac{8}{5})+1(\frac{9}{5}) \\
1(\frac{8}{5})+3(\frac{9}{5})
\end{pmatrix}
=
\begin{pmatrix}
5 \\
7
\end{pmatrix}
$$

Simplifying:

$$
\begin{pmatrix}
\frac{16+9}{5} \\
\frac{8+27}{5}
\end{pmatrix}
=
\begin{pmatrix}
5 \\
7
\end{pmatrix}
$$

Therefore:

$$
\begin{pmatrix}
\frac{25}{5} \\
\frac{35}{5}
\end{pmatrix}
=
\begin{pmatrix}
5 \\
7
\end{pmatrix}
$$

Both sides are equal.

Thus, the obtained solution satisfies the original equation Ax = b.

$$
\boxed{Ax=b}
$$

## 5. CONCLUSION

We calculated the inverse of matrix A and used it to solve the linear system.

The obtained solution is:

$$
\boxed{
x=
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix}
}
$$

Finally, we substituted this vector into the original equation Ax = b.

The matrix multiplication produced the original vector b, confirming that the solution is correct.
