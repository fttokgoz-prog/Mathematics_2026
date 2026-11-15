
# EXERCISE 5 – A 3×3 MATRIX

## 1. GIVEN

We are given the following matrix:

$$
A =
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}
$$

Our task is to find the inverse of A using the Gauss-Jordan elimination method and verify the result by multiplication.

## 2. AUGMENTED MATRIX

First, we create the augmented matrix [A | I], where I is the 3×3 identity matrix.

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
1 & 0 & 1 & 0 & 0 & 1
\end{array}
\right]
$$

## 3. STEP-BY-STEP GAUSS-JORDAN ELIMINATION

**Step 1: Eliminate the first element in the third row.**

Apply the row operation:

$$
R_3 \rightarrow R_3 - R_1
$$

The new augmented matrix is:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
0 & -1 & 1 & -1 & 0 & 1
\end{array}
\right]
$$

**Step 2: Eliminate the second element in the third row.**

Apply the row operation:

$$
R_3 \rightarrow R_3 + R_2
$$

The new augmented matrix is:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
0 & 0 & 2 & -1 & 1 & 1
\end{array}
\right]
$$

**Step 3: Make the third pivot equal to 1.**

Apply the row operation:

$$
R_3 \rightarrow \frac{1}{2}R_3
$$

The new augmented matrix is:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 1 & 0 & 1 & 0 \\
0 & 0 & 1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{array}
\right]
$$

**Step 4: Eliminate the second element in the second row.**

Apply the row operation:

$$
R_2 \rightarrow R_2 - R_3
$$

The new augmented matrix is:

$$
\left[
\begin{array}{ccc|ccc}
1 & 1 & 0 & 1 & 0 & 0 \\
0 & 1 & 0 & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
0 & 0 & 1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{array}
\right]
$$

**Step 5: Eliminate the second element in the first row.**

Apply the row operation:

$$
R_1 \rightarrow R_1 - R_2
$$

The final augmented matrix is:

$$
\left[
\begin{array}{ccc|ccc}
1 & 0 & 0 & \frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
0 & 1 & 0 & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
0 & 0 & 1 & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{array}
\right]
$$

## 4. FINDING THE INVERSE MATRIX

After applying all row operations, the left side becomes the identity matrix.

$$
[A|I] \rightarrow [I|A^{-1}]
$$

Therefore, the right side represents the inverse of A.

$$
\boxed{
A^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
\frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
}
$$

## 5. VERIFICATION BY MULTIPLICATION

To verify our result, we calculate AA⁻¹.

$$
AA^{-1} =
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
\frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
$$

Calculating each element:

$$
AA^{-1} =
\begin{pmatrix}
\frac{1}{2}+\frac{1}{2}+0 &
-\frac{1}{2}+\frac{1}{2}+0 &
\frac{1}{2}-\frac{1}{2}+0 \\

0+\frac{1}{2}-\frac{1}{2} &
0+\frac{1}{2}+\frac{1}{2} &
0-\frac{1}{2}+\frac{1}{2} \\

\frac{1}{2}+0-\frac{1}{2} &
-\frac{1}{2}+0+\frac{1}{2} &
\frac{1}{2}+0+\frac{1}{2}
\end{pmatrix}
$$

Simplifying:

$$
AA^{-1} =
\begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
$$

We obtain the identity matrix.

Therefore, the calculated inverse is correct.

## 6. CONCLUSION

Using the Gauss-Jordan elimination method, we transformed the augmented matrix [A | I] into [I | A⁻¹].

We then verified the result by multiplying A by its inverse.

Since the product gives the identity matrix, our answer is correct.

The final result is:

$$
\boxed{
A^{-1} =
\begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
\frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
}
$$
