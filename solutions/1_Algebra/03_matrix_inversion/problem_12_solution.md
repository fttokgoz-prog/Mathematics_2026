
# EXERCISE 12 – FINDING INVERSES WITHOUT STARTING FROM SCRATCH

## 1. GIVEN

We are given the inverse of matrix A:

$$
A^{-1} =
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
$$

Our task is to calculate (3A)⁻¹, (Aᵀ)⁻¹, and (A²)⁻¹ without finding the original matrix A.

We will use the appropriate inverse properties.

## 2. CALCULATING (3A)⁻¹

The inverse property for a scalar multiplied by a matrix is:

$$
(kA)^{-1}=\frac{1}{k}A^{-1}
$$

Since k = 3, we obtain:

$$
(3A)^{-1}=\frac{1}{3}A^{-1}
$$

Substituting the given inverse:

$$
(3A)^{-1}=
\frac{1}{3}
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
$$

Multiplying each element by 1/3:

$$
\boxed{
(3A)^{-1}=
\begin{pmatrix}
\frac{2}{3} & -\frac{1}{3} \\
-1 & \frac{2}{3}
\end{pmatrix}
}
$$

## 3. CALCULATING (Aᵀ)⁻¹

The inverse of a transpose follows this property:

$$
(A^T)^{-1}=(A^{-1})^T
$$

This means we take the transpose of the given inverse matrix by switching its rows and columns.

$$
(A^T)^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}^{T}
$$

After switching the rows and columns:

$$
\boxed{
(A^T)^{-1}=
\begin{pmatrix}
2 & -3 \\
-1 & 2
\end{pmatrix}
}
$$

## 4. CALCULATING (A²)⁻¹

The inverse property for a product of matrices is:

$$
(AB)^{-1}=B^{-1}A^{-1}
$$

Since A² = AA, we can write:

$$
(A^2)^{-1}=(AA)^{-1}
$$

Applying the inverse property:

$$
(A^2)^{-1}=A^{-1}A^{-1}
$$

Substituting the given inverse matrix:

$$
(A^2)^{-1}=
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
\begin{pmatrix}
2 & -1 \\
-3 & 2
\end{pmatrix}
$$

Calculating each element:

$$
(A^2)^{-1}=
\begin{pmatrix}
2(2)+(-1)(-3) & 2(-1)+(-1)(2) \\
(-3)(2)+2(-3) & (-3)(-1)+2(2)
\end{pmatrix}
$$

Simplifying:

$$
(A^2)^{-1}=
\begin{pmatrix}
4+3 & -2-2 \\
-6-6 & 3+4
\end{pmatrix}
$$

Therefore:

$$
\boxed{
(A^2)^{-1}=
\begin{pmatrix}
7 & -4 \\
-12 & 7
\end{pmatrix}
}
$$

## 5. SUMMARY OF THE RESULTS

Using the inverse properties, we obtained three results without calculating the original matrix A.

**First result:**

$$
(3A)^{-1}=
\begin{pmatrix}
\frac{2}{3} & -\frac{1}{3} \\
-1 & \frac{2}{3}
\end{pmatrix}
$$

**Second result:**

$$
(A^T)^{-1}=
\begin{pmatrix}
2 & -3 \\
-1 & 2
\end{pmatrix}
$$

**Third result:**

$$
(A^2)^{-1}=
\begin{pmatrix}
7 & -4 \\
-12 & 7
\end{pmatrix}
$$

## 6. CONCLUSION

We used three different inverse properties to calculate the required matrices.

We did not need to find the original matrix A or calculate its inverse again.

The important properties are:

$$
(kA)^{-1}=\frac{1}{k}A^{-1}
$$

$$
(A^T)^{-1}=(A^{-1})^T
$$

$$
(A^2)^{-1}=A^{-1}A^{-1}
$$

These properties allow us to calculate new inverses directly from a known inverse matrix.
