
# EXERCISE 11 – PARAMETER AND INVERTIBILITY

## 1. GIVEN

We are given a matrix depending on the parameter t:

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1
\end{pmatrix}
$$

Our task is to find all values of t for which the matrix is invertible, calculate a general formula for A(t)⁻¹, and explain what happens at the excluded values.

## 2. CALCULATING THE DETERMINANT

First, we calculate the determinant of A(t).

For a 2×2 matrix:

$$
\det(A)=ad-bc
$$

Substituting the values:

$$
\det(A(t))=1(1)-t(t)
$$

Simplifying:

$$
\det(A(t))=1-t^2
$$

A matrix is invertible only if its determinant is not equal to zero.

Therefore:

$$
1-t^2 \neq 0
$$

Factoring:

$$
(1-t)(1+t)\neq 0
$$

This means:

$$
\boxed{t\neq 1 \quad \text{and} \quad t\neq -1}
$$

Therefore, the matrix is invertible for all real values of t except 1 and -1.

## 3. FINDING THE INVERSE FORMULA

Using the inverse formula for a 2×2 matrix:

$$
A^{-1}=
\frac{1}{ad-bc}
\begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

For our matrix:

$$
A(t)=
\begin{pmatrix}
1 & t \\
t & 1
\end{pmatrix}
$$

Substituting the values:

$$
A(t)^{-1}=
\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1
\end{pmatrix}
$$

Therefore, the general inverse formula is:

$$
\boxed{
A(t)^{-1}=
\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1
\end{pmatrix}
}
$$

This formula is valid only when:

$$
t\neq 1,\quad t\neq -1
$$

## 4. WHAT HAPPENS AT THE EXCLUDED VALUES?

We must examine the two excluded values separately.

**Case 1: When t = 1**

Substituting t = 1 into the original matrix:

$$
A(1)=
\begin{pmatrix}
1 & 1 \\
1 & 1
\end{pmatrix}
$$

The determinant is:

$$
\det(A(1))=1-1^2=0
$$

Both rows are identical, so they are linearly dependent.

Therefore, the inverse does not exist.

**Case 2: When t = -1**

Substituting t = -1 into the original matrix:

$$
A(-1)=
\begin{pmatrix}
1 & -1 \\
-1 & 1
\end{pmatrix}
$$

The determinant is:

$$
\det(A(-1))=1-(-1)^2=0
$$

The second row is the negative of the first row.

Therefore, the rows are linearly dependent, and the inverse does not exist.

## 5. CONCLUSION

The determinant of A(t) is:

$$
\det(A(t))=1-t^2
$$

The matrix is invertible whenever its determinant is not zero.

Therefore, the inverse exists for:

$$
\boxed{t\in\mathbb{R}\setminus\{-1,1\}}
$$

The general inverse formula is:

$$
\boxed{
A(t)^{-1}=
\frac{1}{1-t^2}
\begin{pmatrix}
1 & -t \\
-t & 1
\end{pmatrix}
}
$$

At t = 1 and t = -1, the denominator becomes zero. This means the inverse formula is undefined at these values.

At both excluded values, the rows are linearly dependent, so the inverse does not exist.
