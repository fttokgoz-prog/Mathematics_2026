
# EXERCISE 15 – TWO METHODS FOR SOLVING THE SAME SYSTEM

## 1. GIVEN

We are given the following linear system:

$$
Ax=b
$$

Where:

$$
A=
\begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
$$

And:

$$
b=
\begin{pmatrix}
7 \\
8
\end{pmatrix}
$$

Our task is to solve the system using two different methods:

1. Using the inverse matrix method: x = A⁻¹b.
2. Using Gaussian elimination.

Then, we will compare both methods.

## 2. FIRST METHOD – USING THE INVERSE MATRIX

We use the formula:

$$
x=A^{-1}b
$$

First, we calculate the determinant of A.

$$
\det(A)=2(3)-1(1)
$$

$$
\det(A)=6-1=5
$$

Since the determinant is not zero, the inverse exists.

Using the 2×2 inverse formula:

$$
A^{-1}=
\frac{1}{5}
\begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
$$

Therefore:

$$
A^{-1}=
\begin{pmatrix}
\frac{3}{5} & -\frac{1}{5} \\
-\frac{1}{5} & \frac{2}{5}
\end{pmatrix}
$$

Now, we calculate x:

$$
x=A^{-1}b
$$

$$
x=
\begin{pmatrix}
\frac{3}{5} & -\frac{1}{5} \\
-\frac{1}{5} & \frac{2}{5}
\end{pmatrix}
\begin{pmatrix}
7 \\
8
\end{pmatrix}
$$

Calculating each element:

$$
x=
\begin{pmatrix}
\frac{3}{5}(7)-\frac{1}{5}(8) \\
-\frac{1}{5}(7)+\frac{2}{5}(8)
\end{pmatrix}
$$

Simplifying:

$$
x=
\begin{pmatrix}
\frac{21-8}{5} \\
\frac{-7+16}{5}
\end{pmatrix}
$$

Therefore:

$$
\boxed{
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5}
\end{pmatrix}
}
$$

## 3. SECOND METHOD – GAUSSIAN ELIMINATION

Now, we solve the same system using Gaussian elimination.

First, we write the augmented matrix:

$$
\left[
\begin{array}{cc|c}
2 & 1 & 7 \\
1 & 3 & 8
\end{array}
\right]
$$

**Step 1: Swap the two rows.**

Apply the row operation:

$$
R_1 \leftrightarrow R_2
$$

The new augmented matrix is:

$$
\left[
\begin{array}{cc|c}
1 & 3 & 8 \\
2 & 1 & 7
\end{array}
\right]
$$

**Step 2: Eliminate the first element in the second row.**

Apply the row operation:

$$
R_2 \rightarrow R_2-2R_1
$$

Calculation:

$$
(2,1,7)-2(1,3,8)
$$

$$
=(2,1,7)-(2,6,16)
$$

$$
=(0,-5,-9)
$$

The new augmented matrix is:

$$
\left[
\begin{array}{cc|c}
1 & 3 & 8 \\
0 & -5 & -9
\end{array}
\right]
$$

**Step 3: Solve for x₂ using back substitution.**

From the second row:

$$
-5x_2=-9
$$

Therefore:

$$
\boxed{x_2=\frac{9}{5}}
$$

**Step 4: Solve for x₁.**

From the first row:

$$
x_1+3x_2=8
$$

Substituting x₂:

$$
x_1+3\left(\frac{9}{5}\right)=8
$$

$$
x_1=8-\frac{27}{5}
$$

$$
x_1=\frac{40}{5}-\frac{27}{5}
$$

Therefore:

$$
\boxed{x_1=\frac{13}{5}}
$$

The final solution using Gaussian elimination is:

$$
\boxed{
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5}
\end{pmatrix}
}
$$

## 4. COMPARING BOTH METHODS

Both methods give exactly the same solution.

**First method – Inverse matrix:**

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5}
\end{pmatrix}
$$

**Second method – Gaussian elimination:**

$$
x=
\begin{pmatrix}
\frac{13}{5} \\
\frac{9}{5}
\end{pmatrix}
$$

The results are identical.

### Comparison of essential steps

| Inverse Matrix Method | Gaussian Elimination |
|---|---|
| Calculate the determinant | Create the augmented matrix |
| Find the inverse matrix | Swap the rows |
| Multiply A⁻¹ by b | Eliminate one variable |
| | Use back substitution |

For this example, Gaussian elimination is simpler because we only need to solve one system.

The inverse matrix method requires calculating the entire inverse matrix before multiplying it by b.

Gaussian elimination allows us to find the solution directly without calculating the full inverse.

## 5. CONCLUSION

We solved the same linear system using two different methods.

Both methods produced the same result:

$$
\boxed{
x_1=\frac{13}{5}, \qquad x_2=\frac{9}{5}
}
$$

Gaussian elimination was simpler in this example because it required fewer essential calculations and did not require finding the complete inverse matrix.

However, the inverse matrix method is also useful when the inverse is already known or when the same matrix is used to solve several different systems.
