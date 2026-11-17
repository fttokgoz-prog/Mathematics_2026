
# EXERCISE 13 – UNDOING A COMPOSITE TRANSFORMATION

## 1. GIVEN

We are given two matrices:

$$
S=
\begin{pmatrix}
2 & 0\\
0 & 1
\end{pmatrix}
$$

$$
H=
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
$$

The composite transformation is:

$$
T=HS
$$

Our task is to find T⁻¹ in two ways:

1. First, calculate T and then find its inverse.
2. Use the inverse property (HS)⁻¹ = S⁻¹H⁻¹.

Additionally, we must calculate the reversed-order candidate H⁻¹S⁻¹ and compare it with the true inverse.

## 2. FIRST METHOD – CALCULATING T AND ITS INVERSE

First, we calculate T = HS.

$$
T=
\begin{pmatrix}
1 & 1\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0\\
0 & 1
\end{pmatrix}
$$

Multiplying the matrices:

$$
T=
\begin{pmatrix}
2 & 1\\
0 & 1
\end{pmatrix}
$$

Now, we calculate the determinant:

$$
\det(T)=2(1)-1(0)=2
$$

Since the determinant is not zero, the inverse exists.

Using the 2×2 inverse formula:

$$
T^{-1}=
\frac{1}{2}
\begin{pmatrix}
1 & -1\\
0 & 2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
T^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2}\\
0 & 1
\end{pmatrix}
}
$$

## 3. SECOND METHOD – USING THE INVERSE OF A PRODUCT

We use the property:

$$
(AB)^{-1}=B^{-1}A^{-1}
$$

Since T = HS:

$$
(HS)^{-1}=S^{-1}H^{-1}
$$

First, we calculate S⁻¹:

$$
S^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0\\
0 & 1
\end{pmatrix}
$$

Next, we calculate H⁻¹:

$$
H^{-1}=
\begin{pmatrix}
1 & -1\\
0 & 1
\end{pmatrix}
$$

Now, we multiply them in the correct order:

$$
T^{-1}=S^{-1}H^{-1}
$$

$$
T^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1\\
0 & 1
\end{pmatrix}
$$

Calculating each element:

$$
T^{-1}=
\begin{pmatrix}
\frac{1}{2}(1)+0(0) &
\frac{1}{2}(-1)+0(1)\\
0(1)+1(0) &
0(-1)+1(1)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
S^{-1}H^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2}\\
0 & 1
\end{pmatrix}
}
$$

Both methods give the same inverse.

## 4. CALCULATING THE REVERSED-ORDER CANDIDATE H⁻¹S⁻¹

Now, we calculate the reversed-order candidate explicitly:

$$
H^{-1}S^{-1}
$$

Using the previously calculated inverse matrices:

$$
H^{-1}S^{-1}=
\begin{pmatrix}
1 & -1\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0\\
0 & 1
\end{pmatrix}
$$

Calculating each element:

$$
H^{-1}S^{-1}=
\begin{pmatrix}
1(\frac{1}{2})+(-1)(0) &
1(0)+(-1)(1)\\
0(\frac{1}{2})+1(0) &
0(0)+1(1)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
H^{-1}S^{-1}=
\begin{pmatrix}
\frac{1}{2} & -1\\
0 & 1
\end{pmatrix}
}
$$

## 5. COMPARING THE REVERSED ORDER WITH THE TRUE INVERSE

The true inverse obtained from the first two methods is:

$$
T^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2}\\
0 & 1
\end{pmatrix}
$$

The reversed-order candidate is:

$$
H^{-1}S^{-1}=
\begin{pmatrix}
\frac{1}{2} & -1\\
0 & 1
\end{pmatrix}
$$

Comparing the two matrices:

$$
\boxed{
S^{-1}H^{-1}\neq H^{-1}S^{-1}
}
$$

The matrices are different because matrix multiplication is not generally commutative.

To verify that the reversed-order candidate is not the true inverse, we multiply T by H⁻¹S⁻¹:

$$
T(H^{-1}S^{-1})=
\begin{pmatrix}
2 & 1\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & -1\\
0 & 1
\end{pmatrix}
$$

Calculating:

$$
=
\begin{pmatrix}
2(\frac{1}{2})+1(0) &
2(-1)+1(1)\\
0(\frac{1}{2})+1(0) &
0(-1)+1(1)
\end{pmatrix}
$$

Therefore:

$$
=
\begin{pmatrix}
1 & -1\\
0 & 1
\end{pmatrix}
$$

This is not the identity matrix.

Thus, H⁻¹S⁻¹ is not the inverse of T.

## 6. WHY MUST THE ORDER BE REVERSED?

The original transformation is:

$$
T=HS
$$

When applying HS to a vector, S acts first and H acts second.

To undo the original transformation, we must reverse the order:

1. First, undo H using H⁻¹.
2. Then, undo S using S⁻¹.

Therefore, the correct inverse is:

$$
\boxed{(HS)^{-1}=S^{-1}H^{-1}}
$$

The reversed order H⁻¹S⁻¹ does not give the correct inverse.

## 7. CONCLUSION

We found T⁻¹ using two different methods.

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
\frac{1}{2} & -\frac{1}{2}\\
0 & 1
\end{pmatrix}
}
$$

We also calculated the reversed-order candidate:

$$
H^{-1}S^{-1}=
\begin{pmatrix}
\frac{1}{2} & -1\\
0 & 1
\end{pmatrix}
$$

This matrix is different from the true inverse and does not produce the identity matrix when multiplied by T.

Therefore, when undoing a composition of transformations, we must reverse the order of the operations.
