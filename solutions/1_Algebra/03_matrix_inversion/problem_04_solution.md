
# EXERCISE 4 – GAUSS-JORDAN METHOD

## 1. GIVEN

We are given the following matrix:

$$
A =
\begin{pmatrix}
1 & 2 \\
3 & 5
\end{pmatrix}
$$

Our task is to find the inverse of A using the Gauss-Jordan method.

We start by creating the augmented matrix [A | I], where I is the identity matrix.

$$
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
3 & 5 & 0 & 1
\end{array}
\right]
$$

## 2. STEP-BY-STEP SOLUTION

**Step 1: Eliminate the first element in the second row.**

Apply the following row operation:

$$
R_2 \rightarrow R_2 - 3R_1
$$

Calculation:

$$
(3,5)-(3,6)=(0,-1)
$$

The new augmented matrix is:

$$
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
0 & -1 & -3 & 1
\end{array}
\right]
$$

**Step 2: Make the second pivot equal to 1.**

Apply the following row operation:

$$
R_2 \rightarrow -R_2
$$

The new augmented matrix is:

$$
\left[
\begin{array}{cc|cc}
1 & 2 & 1 & 0 \\
0 & 1 & 3 & -1
\end{array}
\right]
$$

**Step 3: Eliminate the second element in the first row.**

Apply the following row operation:

$$
R_1 \rightarrow R_1 - 2R_2
$$

Calculation:

$$
(1,2)-(0,2)=(1,0)
$$

For the right side:

$$
(1,0)-2(3,-1)=(-5,2)
$$

The final augmented matrix is:

$$
\left[
\begin{array}{cc|cc}
1 & 0 & -5 & 2 \\
0 & 1 & 3 & -1
\end{array}
\right]
$$

## 3. FINDING THE INVERSE MATRIX

After applying the row operations, the left side becomes the identity matrix.

$$
[A|I] \rightarrow [I|A^{-1}]
$$

Therefore, the right side of the final augmented matrix represents the inverse of A.

$$
\boxed{
A^{-1} =
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
}
$$

## 4. WHY DOES THIS METHOD WORK?

The Gauss-Jordan method applies the same elementary row operations to both sides of the augmented matrix.

When the left side becomes the identity matrix, the right side becomes the inverse of the original matrix.

This is because the row operations transform A into I while applying the same transformations to the identity matrix.

Therefore:

$$
[A|I] \rightarrow [I|A^{-1}]
$$

## 5. CONCLUSION

Using the Gauss-Jordan method, we successfully transformed the original matrix into the identity matrix on the left side.

The resulting matrix on the right side is the inverse of A.

The final answer is:

$$
\boxed{
A^{-1} =
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
}
$$
