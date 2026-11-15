
# EXERCISE 3 – WHEN DOES THE INVERSE NOT EXIST?

## 1. GIVEN

We are given the following matrix:

$$
A =
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}
$$

Our task is to explain why the inverse of A does not exist in two different ways: using the determinant and using the dependence between the rows.

## 2. FIRST METHOD – USING THE DETERMINANT

For a 2×2 matrix, the determinant is calculated using:

$$
\det(A)=ad-bc
$$

Substituting the values from matrix A:

$$
\det(A)=2(2)-4(1)
$$

$$
\det(A)=4-4
$$

$$
\boxed{\det(A)=0}
$$

A matrix has an inverse only if its determinant is not equal to zero.

Since the determinant of A is zero, the inverse does not exist.

Therefore:

$$
\boxed{A^{-1}\text{ does not exist}}
$$

## 3. SECOND METHOD – USING ROW DEPENDENCE

Now, we examine the relationship between the two rows.

The matrix is:

$$
A =
\begin{pmatrix}
2 & 4 \\
1 & 2
\end{pmatrix}
$$

The first row is:

$$
R_1=(2,4)
$$

The second row is:

$$
R_2=(1,2)
$$

We can see that the first row is exactly two times the second row.

$$
R_1=2R_2
$$

This means that the rows are linearly dependent.

One row does not provide any new independent information.

Therefore, the matrix does not have an inverse.

## 4. CONCLUSION

We have shown in two different ways why the inverse of matrix A does not exist.

**First method:** The determinant is zero.

$$
\det(A)=0
$$

**Second method:** The rows are linearly dependent because:

$$
R_1=2R_2
$$

Both methods lead to the same conclusion.

Therefore:

$$
\boxed{A^{-1}\text{ does not exist}}
$$
