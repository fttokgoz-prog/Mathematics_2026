
# EXERCISE 8 – INVERSE OF A TRANSFORMATION

## 1. GIVEN

We are given the following matrix:

$$
S =
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
$$

This matrix describes a scaling transformation of the plane.

Our task is to find S⁻¹, explain its geometric meaning, and check the action of S and S⁻¹ on a simple vector.

## 2. FINDING THE INVERSE MATRIX

Since S is a diagonal matrix, we can find its inverse by taking the reciprocal of each diagonal element.

The original matrix is:

$$
S =
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
$$

Taking the reciprocal of each diagonal element:

$$
S^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
$$

Therefore, the inverse matrix is:

$$
\boxed{
S^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
}
$$

## 3. GEOMETRIC INTERPRETATION

The original transformation S changes the coordinates of a vector in two different ways.

- The x-coordinate is multiplied by 2, so the plane is stretched horizontally.
- The y-coordinate is multiplied by 1/2, so the plane is compressed vertically.

The inverse transformation S⁻¹ reverses these changes.

- The x-coordinate is multiplied by 1/2, so the horizontal direction is compressed.
- The y-coordinate is multiplied by 2, so the vertical direction is stretched.

Therefore, S⁻¹ undoes the original transformation S and restores the original vector.

## 4. CHECKING THE TRANSFORMATION ON A VECTOR

To verify the result, we choose a simple vector:

$$
v =
\begin{pmatrix}
2 \\
4
\end{pmatrix}
$$

First, we apply the transformation S.

$$
Sv =
\begin{pmatrix}
2 & 0 \\
0 & \frac{1}{2}
\end{pmatrix}
\begin{pmatrix}
2 \\
4
\end{pmatrix}
$$

Calculating:

$$
Sv =
\begin{pmatrix}
2(2)+0(4) \\
0(2)+\frac{1}{2}(4)
\end{pmatrix}
$$

$$
Sv =
\begin{pmatrix}
4 \\
2
\end{pmatrix}
$$

Now, we apply the inverse transformation S⁻¹ to the resulting vector.

$$
S^{-1}(Sv) =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
\begin{pmatrix}
4 \\
2
\end{pmatrix}
$$

Calculating:

$$
S^{-1}(Sv) =
\begin{pmatrix}
\frac{1}{2}(4)+0(2) \\
0(4)+2(2)
\end{pmatrix}
$$

$$
S^{-1}(Sv) =
\begin{pmatrix}
2 \\
4
\end{pmatrix}
$$

We have obtained the original vector again.

Therefore:

$$
\boxed{S^{-1}(Sv)=v}
$$

## 5. CONCLUSION

The inverse transformation reverses the scaling performed by the original matrix.

The original transformation stretches the horizontal direction and compresses the vertical direction.

The inverse transformation does the opposite.

By applying both transformations to the vector (2,4), we obtained the original vector again.

This confirms that S⁻¹ correctly reverses the transformation S.

The final result is:

$$
\boxed{
S^{-1} =
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 2
\end{pmatrix}
}
$$
