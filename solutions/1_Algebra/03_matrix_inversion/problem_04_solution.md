
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

## 2. SUCCESSIVE ROW OPERATIONS

**Step 1: Eliminate the first element in the second row.**

Apply the row operation:

$$
R_2 \rightarrow R_2 - 3R_1
$$

Calculation:

$$
(3,5)-3(1,2)=(0,-1)
$$

We apply the same operation to the entire augmented row, including the right side.

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

Apply the row operation:

$$
R_2 \rightarrow -R_2
$$

The entire second row changes sign.

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

Apply the row operation:

$$
R_1 \rightarrow R_1 - 2R_2
$$

Calculation on the left side:

$$
(1,2)-2(0,1)=(1,0)
$$

Calculation on the right side:

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

After all row operations, the left side becomes the identity matrix.

We have transformed:

$$
[A|I] \rightarrow [I|A^{-1}]
$$

Therefore, the right side of the final augmented matrix is the inverse of A.

$$
\boxed{
A^{-1} =
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
}
$$

## 4. WHY DOES OBTAINING I ON THE LEFT GIVE THE INVERSE ON THE RIGHT?

Each elementary row operation can be represented by multiplication with an elementary matrix.

Let E₁, E₂, and E₃ represent the three row operations.

Applying these operations to the augmented matrix gives:

$$
E_3E_2E_1[A|I]
=
[E_3E_2E_1A|E_3E_2E_1I]
$$

Since the left side becomes the identity matrix:

$$
E_3E_2E_1A=I
$$

By the definition of the inverse matrix, this means:

$$
E_3E_2E_1=A^{-1}
$$

Therefore, applying the same operations to the identity matrix produces:

$$
E_3E_2E_1I=A^{-1}
$$

This explains why, when the left side becomes I, the right side becomes the inverse of the original matrix.

## 5. CONCLUSION

Using the Gauss-Jordan method, we transformed the augmented matrix [A | I] into [I | A⁻¹].

We showed every intermediate augmented matrix after each row operation.

We also explained that the same elementary row operations transform the identity matrix into the inverse of A.

The final result is:

$$
\boxed{
A^{-1} =
\begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
}
$$
