
# EXERCISE 7 – INVERSE OF A PRODUCT

## 1. GIVEN

We are given two matrices:

$$
A =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

$$
B =
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
$$

Our task is to calculate (AB)⁻¹ and B⁻¹A⁻¹, check that the results are the same, and explain why the order is reversed.

## 2. CALCULATING AB

First, we multiply matrix A by matrix B.

$$
AB =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
$$

Calculating each element:

$$
AB =
\begin{pmatrix}
1(2)+1(0) & 1(0)+1(3) \\
0(2)+1(0) & 0(0)+1(3)
\end{pmatrix}
$$

Therefore:

$$
AB =
\begin{pmatrix}
2 & 3 \\
0 & 3
\end{pmatrix}
$$

## 3. CALCULATING (AB)⁻¹

First, we calculate the determinant of AB.

$$
\det(AB)=2(3)-3(0)
$$

$$
\det(AB)=6
$$

Using the inverse formula for a 2×2 matrix:

$$
(AB)^{-1}=
\frac{1}{6}
\begin{pmatrix}
3 & -3 \\
0 & 2
\end{pmatrix}
$$

Therefore:

$$
\boxed{
(AB)^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
}
$$

## 4. CALCULATING B⁻¹ AND A⁻¹

First, we calculate the inverse of matrix B.

$$
B^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3}
\end{pmatrix}
$$

Now, we calculate the inverse of matrix A.

$$
A^{-1}=
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

## 5. CALCULATING B⁻¹A⁻¹

Now, we multiply B⁻¹ by A⁻¹ in the given order.

$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3}
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
$$

Calculating each element:

$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2}(1)+0(0) &
\frac{1}{2}(-1)+0(1) \\
0(1)+\frac{1}{3}(0) &
0(-1)+\frac{1}{3}(1)
\end{pmatrix}
$$

Therefore:

$$
\boxed{
B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
}
$$

## 6. COMPARING THE RESULTS

We obtained:

$$
(AB)^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

And:

$$
B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
$$

Both results are exactly the same.

Therefore:

$$
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
$$

## 7. WHY IS THE ORDER REVERSED?

The order is reversed because matrix multiplication is not generally commutative.

To undo the multiplication AB, we must first undo B and then undo A.

This is why the inverse of a product is calculated in reverse order.

The general property is:

$$
\boxed{(AB)^{-1}=B^{-1}A^{-1}}
$$

## 8. CONCLUSION

We calculated the inverse of the product AB and separately calculated B⁻¹A⁻¹.

Both calculations gave the same result.

This confirms that the inverse of a product is equal to the product of the inverses in reversed order.

The final answer is:

$$
\boxed{
(AB)^{-1}=B^{-1}A^{-1}=
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
}
$$
