
# EXERCISE 10 – INVERSE OF A DIAGONAL MATRIX

## 1. GIVEN

We are given two diagonal matrices:

$$
D =
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix}
$$

$$
E =
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5
\end{pmatrix}
$$

Our task is to determine which matrix is invertible without using Gauss-Jordan elimination.

For an invertible diagonal matrix, every diagonal element must be nonzero.

## 2. CHECKING MATRIX D

First, we examine matrix D.

$$
D =
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix}
$$

All diagonal elements are nonzero:

$$
2 \neq 0,\quad -3 \neq 0,\quad 5 \neq 0
$$

Therefore, matrix D is invertible.

To find its inverse, we take the reciprocal of each diagonal element.

$$
D^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
$$

Therefore:

$$
\boxed{
D^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
}
$$

## 3. CHECKING MATRIX E

Now, we examine matrix E.

$$
E =
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5
\end{pmatrix}
$$

The middle diagonal element is zero.

$$
0 = 0
$$

We can also calculate its determinant:

$$
\det(E)=2 \cdot 0 \cdot 5
$$

$$
\boxed{\det(E)=0}
$$

A matrix has an inverse only if its determinant is not equal to zero.

Since the determinant of E is zero, matrix E is not invertible.

The second row also contains only zeros, which means the rows are linearly dependent.

Therefore:

$$
\boxed{E^{-1}\text{ does not exist}}
$$

## 4. VERIFICATION OF D⁻¹ BY MULTIPLICATION

To verify the inverse of D, we calculate DD⁻¹.

$$
DD^{-1} =
\begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
$$

Multiplying the corresponding diagonal elements:

$$
DD^{-1} =
\begin{pmatrix}
2(\frac{1}{2}) & 0 & 0 \\
0 & (-3)(-\frac{1}{3}) & 0 \\
0 & 0 & 5(\frac{1}{5})
\end{pmatrix}
$$

Simplifying:

$$
DD^{-1} =
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
$$

We obtain the identity matrix I.

Therefore, the inverse of D is correct.

## 5. CONCLUSION

We examined both diagonal matrices without using Gauss-Jordan elimination.

Matrix D is invertible because all its diagonal elements are nonzero.

Matrix E is not invertible because one of its diagonal elements is zero, making its determinant equal to zero.

We also verified the inverse of D by multiplication.

The final results are:

$$
\boxed{
D^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
}
$$

$$
\boxed{E^{-1}\text{ does not exist}}
$$
