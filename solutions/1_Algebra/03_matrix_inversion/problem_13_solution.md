
# EXERCISE 13 – UNDOING A COMPOSITE TRANSFORMATION

## 1. GIVEN

We are given two matrices:

$$
S =
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
$$

$$
H =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

The composite transformation is:

$$
T=HS
$$

Our task is to find T⁻¹ in two different ways, compare the results, and explain why the order of inverse transformations matters.

## 2. FIRST METHOD – CALCULATING T AND THEN ITS INVERSE

First, we calculate the product T = HS.

$$
T =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
$$

Calculating each element:

$$
T =
\begin{pmatrix}
1(2)+1(0) & 1(0)+1(1) \\
0(2)+1(0) & 0(0)+1(1)
\end{pmatrix}
$$

Therefore:

$$
T =
\begin{pmatrix}
2 & 1 \\
0 & 1
\end{pmatrix}
$$

Now, we calculate the determinant:

$$
\det(T)=2(1)-1(0)
$$

$$
\det(T)=2
$$

Since the determinant is not zero, the inverse exists.

Using the 2×2 inverse formula:

$$
T^{-1}=
\frac{1}{2}
\begin{pmatrix}
1 & -1 \\
0 & 2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
T^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
}
$$

## 3. SECOND METHOD – USING THE INVERSE OF A PRODUCT

We know the inverse property:

$$
(AB)^{-1}=B^{-1}A^{-1}
$$

Since T = HS, we obtain:

$$
(HS)^{-1}=S^{-1}H^{-1}
$$

First, we calculate S⁻¹.

$$
S =
\begin{pmatrix}
2 & 0 \\
0 & 1
\end{pmatrix}
$$

Taking the reciprocal of the diagonal elements:

$$
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
$$

Next, we calculate H⁻¹.

$$
H =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Using the 2×2 inverse formula:

$$
H^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

Now, we multiply S⁻¹ by H⁻¹ in the correct order.

$$
T^{-1}=S^{-1}H^{-1}
$$

$$
T^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

Calculating each element:

$$
T^{-1}=
\begin{pmatrix}
\frac{1}{2}(1)+0(0) &
\frac{1}{2}(-1)+0(1) \\
0(1)+1(0) &
0(-1)+1(1)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
T^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
}
$$

Both methods give the same result.

## 4. CHECKING THE INCORRECT ORDER

Now, we calculate the product in the incorrect order:

$$
H^{-1}S^{-1}
$$

$$
H^{-1}S^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & 1
\end{pmatrix}
$$

Calculating:

$$
H^{-1}S^{-1}=
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1
\end{pmatrix}
$$

This result is different from the correct inverse:

$$
S^{-1}H^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
$$

Therefore:

$$
\boxed{S^{-1}H^{-1}\neq H^{-1}S^{-1}}
$$

To verify that the incorrect order does not give the inverse, we multiply T by the incorrect result.

$$
T(H^{-1}S^{-1})=
\begin{pmatrix}
2 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & -1 \\
0 & 1
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1 & -2+1 \\
0 & 1
\end{pmatrix}
$$

$$
=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

This is not the identity matrix.

Therefore, the incorrect order does not produce the inverse of T.

## 5. WHY MUST THE ORDER BE REVERSED?

The original transformation is:

$$
T=HS
$$

When a vector is multiplied by HS, the transformation S is applied first, followed by H.

To undo this composite transformation, we must reverse the order of the operations.

First, we undo H using H⁻¹.

Then, we undo S using S⁻¹.

This is why:

$$
\boxed{(HS)^{-1}=S^{-1}H^{-1}}
$$

The inverse of a product always reverses the order of the original matrices.

## 6. CONCLUSION

We calculated T⁻¹ using two different methods.

The first method involved calculating T = HS and then finding its inverse.

The second method used the inverse-of-a-product property:

$$
(HS)^{-1}=S^{-1}H^{-1}
$$

Both methods produced the same result:

$$
\boxed{
T^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & 1
\end{pmatrix}
}
$$

We also demonstrated that using the incorrect order H⁻¹S⁻¹ produces a different matrix and does not give the identity when multiplied by T.

Therefore, when undoing a composition of transformations, we must always reverse the order of the operations.
