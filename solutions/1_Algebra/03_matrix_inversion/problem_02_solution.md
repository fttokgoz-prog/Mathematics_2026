
# EXERCISE 2 – FORMULA FOR A 2×2 MATRIX

## 1. GIVEN

We are given the following matrix:

$$
A =
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
$$

Our task is to find the inverse of A using the formula for a 2×2 matrix and verify the result by multiplying it with A.

## 2. CALCULATING THE DETERMINANT

First, we calculate the determinant of matrix A.

For a 2×2 matrix:

$$
A =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

The determinant is:

$$
\det(A)=ad-bc
$$

Substituting the values:

$$
\det(A)=3(4)-2(5)
$$

$$
\det(A)=12-10
$$

$$
\boxed{\det(A)=2}
$$

Since the determinant is not equal to zero, the inverse of A exists.

## 3. FINDING THE INVERSE

The inverse formula for a 2×2 matrix is:

$$
A^{-1}=\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

Using the values from matrix A:

$$
A^{-1}=\frac{1}{2}
\begin{pmatrix}
4 & -2 \\
-5 & 3
\end{pmatrix}
$$

Now, we multiply each element by 1/2:

$$
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

Therefore, the inverse matrix is:

$$
\boxed{
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
}
$$

## 4. VERIFICATION

To check our result, we calculate the product of A and its inverse.

$$
AA^{-1}=
\begin{pmatrix}
3 & 2 \\
5 & 4
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
$$

Calculating each element:

$$
AA^{-1}=
\begin{pmatrix}
3(2)+2(-\frac{5}{2}) & 3(-1)+2(\frac{3}{2}) \\
5(2)+4(-\frac{5}{2}) & 5(-1)+4(\frac{3}{2})
\end{pmatrix}
$$

Simplifying:

$$
AA^{-1}=
\begin{pmatrix}
6-5 & -3+3 \\
10-10 & -5+6
\end{pmatrix}
$$

$$
AA^{-1}=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

This is the identity matrix I.

## 5. CONCLUSION

The determinant of A is 2, which means that the inverse exists.

Using the 2×2 inverse formula, we found the inverse matrix.

Finally, multiplying A by its inverse gives the identity matrix.

Therefore, our result is correct:

$$
\boxed{
A^{-1}=
\begin{pmatrix}
2 & -1 \\
-\frac{5}{2} & \frac{3}{2}
\end{pmatrix}
}
$$
