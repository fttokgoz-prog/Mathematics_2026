
# EXERCISE 1 – DEFINITION OF THE INVERSE

## 1. GIVEN

We are given two matrices:

$$
A =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
$$

$$
B =
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
$$

Our task is to check whether B is the inverse of A without using an inverse formula. We will calculate both AB and BA.

## 2. CALCULATING AB

First, we multiply matrix A by matrix B.

$$
AB =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
$$

Calculating each element:

$$
AB =
\begin{pmatrix}
2(1)+1(-1) & 2(-1)+1(2) \\
1(1)+1(-1) & 1(-1)+1(2)
\end{pmatrix}
$$

$$
AB =
\begin{pmatrix}
2-1 & -2+2 \\
1-1 & -1+2
\end{pmatrix}
$$

$$
AB =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

Therefore, AB = I.

## 3. CALCULATING BA

Now, we multiply matrix B by matrix A.

$$
BA =
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
$$

Calculating each element:

$$
BA =
\begin{pmatrix}
1(2)+(-1)(1) & 1(1)+(-1)(1) \\
(-1)(2)+2(1) & (-1)(1)+2(1)
\end{pmatrix}
$$

$$
BA =
\begin{pmatrix}
2-1 & 1-1 \\
-2+2 & -1+2
\end{pmatrix}
$$

$$
BA =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

Therefore, BA = I.

## 4. RELATION TO THE DEFINITION OF THE INVERSE

According to the definition of the inverse matrix, a matrix B is the inverse of matrix A if:

$$
AB = BA = I
$$

In our calculations, both products give the identity matrix.

$$
AB = BA =
\begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
$$

Therefore, B is the inverse of A.

## 5. CONCLUSION

We verified the inverse relationship by multiplying the matrices in both orders, without using an inverse formula.

The final result is:

$$
\boxed{B = A^{-1}}
$$
