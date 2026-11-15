
# EXERCISE 6 – SOLVING A SYSTEM USING THE INVERSE

## 1. GIVEN

We are given the following linear system:

$$
Ax=b
$$

Where:

$$
A =
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
$$

And:

$$
b =
\begin{pmatrix}
5 \\
7
\end{pmatrix}
$$

Our task is to solve the system using:

$$
x=A^{-1}b
$$

## 2. CALCULATING THE INVERSE OF A

First, we calculate the determinant of matrix A.

$$
\det(A)=2(3)-1(1)
$$

$$
\det(A)=6-1=5
$$

Since the determinant is not equal to zero, the inverse exists.

Using the 2×2 inverse formula:

$$
A^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

Substituting the values:

$$
A^{-1}=\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A^{-1}=
\begin{pmatrix}
\frac{3}{5} & -\frac{1}{5} \\
-\frac{1}{5} & \frac{2}{5}
\end{pmatrix}
}
$$

## 3. SOLVING THE SYSTEM USING x = A⁻¹b

Now, we calculate x by multiplying the inverse matrix by vector b.

$$
x=A^{-1}b
$$

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

Therefore:

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

To check our result, we substitute the values of x back into the original equation:

$$
Ax=b
$$

We use:

$$
x_1=\frac{8}{5}, \qquad x_2=\frac{9}{5}
$$

The original system is:

$$
\begin{cases}
2x_1+x_2=5 \\
x_1+3x_2=7
\end{cases}
$$

First equation:

$$
2\left(\frac{8}{5}\right)+\frac{9}{5}
$$

$$
=\frac{16}{5}+\frac{9}{5}
$$

$$
=\frac{25}{5}=5
$$

Second equation:

$$
\frac{8}{5}+3\left(\frac{9}{5}\right)
$$

$$
=\frac{8}{5}+\frac{27}{5}
$$

$$
=\frac{35}{5}=7
$$

Both equations are satisfied.

Therefore, the solution is correct.

## 5. CONCLUSION

We calculated the inverse of matrix A and used it to solve the linear system.

By applying the formula x = A⁻¹b, we obtained:

$$
\boxed{
x=
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix}
}
$$

Finally, we substituted the values back into the original system and verified that both equations are satisfied.

Therefore, the final solution is:

$$
\boxed{x_1=\frac{8}{5}, \quad x_2=\frac{9}{5}}
$$
