
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
2 & 1\\
1 & 3
\end{pmatrix}
$$

And:

$$
b=
\begin{pmatrix}
7\\
8
\end{pmatrix}
$$

Our task is to solve the system using two methods:

1. The inverse matrix method: x = A⁻¹b.
2. Gaussian elimination.

After solving, we must compare both solutions, count the essential steps, and identify which method is simpler in this example.

## 2. FIRST METHOD – USING THE INVERSE MATRIX

We use the formula:

$$
x=A^{-1}b
$$

**Step 1: Calculate the determinant.**

$$
\det(A)=2(3)-1(1)
$$

$$
\det(A)=6-1=5
$$

Since the determinant is not zero, the inverse exists.

**Step 2: Calculate the inverse matrix.**

Using the 2×2 inverse formula:

$$
A^{-1}=
\frac{1}{5}
\begin{pmatrix}
3 & -1\\
-1 & 2
\end{pmatrix}
$$

Therefore:

$$
A^{-1}=
\begin{pmatrix}
\frac{3}{5} & -\frac{1}{5}\\
-\frac{1}{5} & \frac{2}{5}
\end{pmatrix}
$$

**Step 3: Calculate x = A⁻¹b.**

$$
x=
\begin{pmatrix}
\frac{3}{5} & -\frac{1}{5}\\
-\frac{1}{5} & \frac{2}{5}
\end{pmatrix}
\begin{pmatrix}
7\\
8
\end{pmatrix}
$$

Calculating each element:

$$
x=
\begin{pmatrix}
\frac{3}{5}(7)-\frac{1}{5}(8)\\
-\frac{1}{5}(7)+\frac{2}{5}(8)
\end{pmatrix}
$$

Simplifying:

$$
x=
\begin{pmatrix}
\frac{21-8}{5}\\
\frac{-7+16}{5}
\end{pmatrix}
$$

Therefore:

$$
\boxed{
x=
\begin{pmatrix}
\frac{13}{5}\\
\frac{9}{5}
\end{pmatrix}
}
$$

## 3. SECOND METHOD – GAUSSIAN ELIMINATION

Now, we solve the same system using Gaussian elimination.

**Step 1: Create the augmented matrix.**

$$
\left[
\begin{array}{cc|c}
2 & 1 & 7\\
1 & 3 & 8
\end{array}
\right]
$$

**Step 2: Eliminate the first element in the second row.**

To avoid fractions, we use:

$$
R_2 \rightarrow 2R_2-R_1
$$

Calculation:

$$
2(1,3,8)-(2,1,7)
$$

$$
=(2,6,16)-(2,1,7)
$$

$$
=(0,5,9)
$$

The new augmented matrix is:

$$
\left[
\begin{array}{cc|c}
2 & 1 & 7\\
0 & 5 & 9
\end{array}
\right]
$$

**Step 3: Use back substitution.**

From the second row:

$$
5x_2=9
$$

Therefore:

$$
x_2=\frac{9}{5}
$$

Now, we substitute this value into the first equation:

$$
2x_1+x_2=7
$$

$$
2x_1+\frac{9}{5}=7
$$

$$
2x_1=\frac{35}{5}-\frac{9}{5}
$$

$$
2x_1=\frac{26}{5}
$$

Therefore:

$$
x_1=\frac{13}{5}
$$

The final solution is:

$$
\boxed{
x=
\begin{pmatrix}
\frac{13}{5}\\
\frac{9}{5}
\end{pmatrix}
}
$$

## 4. COMPARISON OF BOTH METHODS

Both methods produce exactly the same solution.

**Inverse matrix method:**

$$
x=
\begin{pmatrix}
\frac{13}{5}\\
\frac{9}{5}
\end{pmatrix}
$$

**Gaussian elimination:**

$$
x=
\begin{pmatrix}
\frac{13}{5}\\
\frac{9}{5}
\end{pmatrix}
$$

Therefore, both methods give the same result.

### Comparison of essential steps

For a fair comparison, we count the main calculation stages rather than every individual arithmetic operation.

| Inverse Matrix Method | Gaussian Elimination |
|---|---|
| 1. Calculate the determinant | 1. Create the augmented matrix |
| 2. Calculate the inverse matrix | 2. Perform row elimination |
| 3. Multiply A⁻¹ by b | 3. Use back substitution |

Both methods require 3 main calculation stages in this example.

### Which method is simpler?

Gaussian elimination is simpler in this particular example.

The reason is that we only need to solve one linear system. Gaussian elimination requires just one row elimination followed by back substitution.

The inverse matrix method requires calculating the complete inverse matrix before multiplying it by b.

Therefore, Gaussian elimination avoids the additional work of finding the full inverse matrix.

## 5. CONCLUSION

We solved the same linear system using two different methods.

Both methods produced the same result:

$$
\boxed{
x=
\begin{pmatrix}
\frac{13}{5}\\
\frac{9}{5}
\end{pmatrix}
}
$$

We compared the essential calculation stages and found that both methods require three main stages in this example.

However, Gaussian elimination is simpler because it solves the system directly without calculating the complete inverse matrix.

Therefore, Gaussian elimination is the more convenient method for this particular system.
