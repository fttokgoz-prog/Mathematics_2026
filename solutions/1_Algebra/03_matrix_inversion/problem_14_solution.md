
# EXERCISE 14 – A MATRIX THAT IS ITS OWN INVERSE

## 1. GIVEN

Assume that a square matrix A satisfies:

$$
A^2=I
$$

This means:

$$
AA=I
$$

Our task is to show that:

$$
A^{-1}=A
$$

Then, we will give an example of a 2×2 matrix different from I and -I that satisfies this condition and verify it by multiplication.

## 2. MATHEMATICAL PROOF

According to the definition of the inverse matrix, a matrix A⁻¹ satisfies:

$$
AA^{-1}=A^{-1}A=I
$$

We are given that:

$$
A^2=I
$$

Since A² means multiplying A by itself, we can write:

$$
AA=I
$$

Comparing this with the definition of the inverse, we see that A multiplied by A gives the identity matrix.

Therefore, A is its own inverse.

Hence:

$$
\boxed{A^{-1}=A}
$$

## 3. EXAMPLE OF A 2×2 MATRIX

Now, we choose a matrix different from the identity matrix I and negative identity matrix -I.

Let:

$$
A=
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
$$

This matrix is different from both I and -I.

The identity matrix is:

$$
I=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

The negative identity matrix is:

$$
-I=
\begin{pmatrix}
-1 & 0 \\
0 & -1
\end{pmatrix}
$$

## 4. VERIFICATION BY MULTIPLICATION

To verify that our example satisfies A² = I, we multiply A by itself.

$$
A^2=A \cdot A
$$

$$
A^2=
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
$$

Calculating each element:

$$
A^2=
\begin{pmatrix}
0(0)+1(1) & 0(1)+1(0) \\
1(0)+0(1) & 1(1)+0(0)
\end{pmatrix}
$$

Simplifying:

$$
A^2=
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

Therefore:

$$
\boxed{A^2=I}
$$

Since A multiplied by itself gives the identity matrix, we can conclude that:

$$
\boxed{A^{-1}=A}
$$

## 5. CONCLUSION

We proved that if a square matrix satisfies A² = I, then the matrix is its own inverse.

We also provided a 2×2 example different from I and -I:

$$
A=
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
$$

By multiplying the matrix by itself, we obtained the identity matrix.

Therefore, the example satisfies the given condition.

The final result is:

$$
\boxed{A^{-1}=A}
$$
