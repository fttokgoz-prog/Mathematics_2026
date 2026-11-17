
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

For the invertible matrix, we must calculate its inverse and verify the result by multiplying the original matrix by its inverse.

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

For a diagonal matrix, the determinant is the product of its diagonal elements.

$$
\det(D)=2(-3)(5)
$$

$$
\boxed{\det(D)=-30}
$$

Since the determinant is not equal to zero, matrix D is invertible.

## 3. FINDING THE INVERSE OF D

For an invertible diagonal matrix, we calculate its inverse by taking the reciprocal of each diagonal element.

Therefore:

$$
D^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
$$

The inverse matrix is:

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

## 4. VERIFYING THE INVERSE BY MULTIPLICATION

To verify our result, we calculate the product of D and D⁻¹.

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

Calculating each element:

$$
DD^{-1} =
\begin{pmatrix}
2(\frac{1}{2})+0+0 &
0+0+0 &
0+0+0 \\

0+0+0 &
(-3)(-\frac{1}{3})+0+0 &
0+0+0 \\

0+0+0 &
0+0+0 &
5(\frac{1}{5})
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

Therefore:

$$
\boxed{DD^{-1}=I}
$$

This confirms that the calculated inverse is correct.

## 5. CHECKING MATRIX E

Now, we examine matrix E.

$$
E =
\begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5
\end{pmatrix}
$$

The determinant is the product of its diagonal elements.

$$
\det(E)=2(0)(5)
$$

$$
\boxed{\det(E)=0}
$$

A matrix is invertible only if its determinant is not equal to zero.

Since the determinant of E is zero, matrix E is not invertible.

We can also see that the second row contains only zeros.

Therefore, the rows are linearly dependent, and the inverse does not exist.

$$
\boxed{E^{-1}\text{ does not exist}}
$$

## 6. CONCLUSION

We examined both diagonal matrices without using Gauss-Jordan elimination.

Matrix D is invertible because all its diagonal elements are nonzero.

Its inverse is:

$$
D^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
$$

We verified the result by multiplying D by D⁻¹ and obtaining the identity matrix.

Matrix E is not invertible because its determinant is zero.

Therefore, the final results are:

$$
\boxed{DD^{-1}=I}
$$

$$
\boxed{E^{-1}\text{ does not exist}}
$$
