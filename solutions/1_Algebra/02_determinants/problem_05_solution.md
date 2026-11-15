
# EXERCISE 5 – ROW OPERATIONS

## 1. GIVEN

We are given the following matrix:

$$
A =
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
$$

Our task is to calculate the determinant by simplifying the matrix using row operations.

## 2. STEP-BY-STEP SOLUTION

**Step 1:**

Apply the following row operation:

$$
R_2 \rightarrow R_2 - 2R_1
$$

Calculation:

$$
(2,1,0)-2(1,2,3)
$$

$$
=(2,1,0)-(2,4,6)
$$

$$
=(0,-3,-6)
$$

The determinant does not change because we subtract a multiple of one row from another row.

The new matrix is:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2
\end{pmatrix}
$$

**Step 2:**

Apply the following row operation:

$$
R_3 \rightarrow R_3 + R_1
$$

Calculation:

$$
(-1,4,2)+(1,2,3)=(0,6,5)
$$

The determinant does not change.

The new matrix is:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5
\end{pmatrix}
$$

**Step 3:**

Apply the following row operation:

$$
R_3 \rightarrow R_3 + 2R_2
$$

Calculation:

$$
(0,6,5)+2(0,-3,-6)
$$

$$
=(0,6,5)+(0,-6,-12)
$$

$$
=(0,0,-7)
$$

The determinant does not change.

The final upper triangular matrix is:

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7
\end{pmatrix}
$$

## 3. DETERMINANT CALCULATION

For an upper triangular matrix, the determinant is the product of the diagonal elements.

$$
\det(A)=1 \cdot (-3) \cdot (-7)
$$

$$
\det(A)=21
$$

## 4. ROW OPERATIONS SUMMARY

| Row Operation | Effect on Determinant |
|---|---|
| R2 -> R2 - 2R1 | No change |
| R3 -> R3 + R1 | No change |
| R3 -> R3 + 2R2 | No change |

## 5. CONCLUSION

All row operations used in this solution preserve the determinant because adding or subtracting a multiple of one row to another row does not change the determinant.

Therefore, the final result is:

$$
\boxed{\det(A)=21}
$$
