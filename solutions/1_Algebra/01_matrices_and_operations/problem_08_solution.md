# Exercise 8. Row Operations and Their Reversibility

## Question

For

$$
A=\begin{pmatrix}
1 & 2 & -1\\
2 & 4 & 1\\
-1 & 1 & 3
\end{pmatrix}
$$

perform, in order:

1. \(R_2\leftarrow R_2-2R_1\)
2. \(R_3\leftarrow R_3+R_1\)
3. Interchange \(R_2\) and \(R_3\).

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

**Why this exercise:** Prepares for elimination by showing that row operations are controlled and reversible transformations of a matrix.

## Solution

### Step 1: Understand elementary row operations

An elementary row operation changes one or more rows of a matrix in a specific way. These operations are commonly used to simplify matrices when solving systems of linear equations.

There are three main types of elementary row operations:

1. Interchanging two rows.
2. Multiplying a row by a nonzero scalar.
3. Adding a multiple of one row to another row.

Each operation is reversible. This means that after performing a row operation, we can apply another operation to recover the original matrix.

The original matrix is

$$
A=\begin{pmatrix}
1 & 2 & -1\\
2 & 4 & 1\\
-1 & 1 & 3
\end{pmatrix}.
$$

We will apply the three given operations in the specified order.

### Step 2: Perform the first row operation

The first operation is

$$
R_2\leftarrow R_2-2R_1.
$$

This means that we replace the second row with the second row minus twice the first row. The other rows remain unchanged.

The original rows are

$$
R_1=(1,2,-1)
$$

$$
R_2=(2,4,1)
$$

$$
R_3=(-1,1,3).
$$

First, calculate twice the first row:

$$
2R_1=2(1,2,-1)=(2,4,-2).
$$

Now subtract this result from the second row:

$$
R_2-2R_1=(2,4,1)-(2,4,-2).
$$

Subtract the corresponding entries:

$$
R_2-2R_1=
(2-2,\;4-4,\;1-(-2)).
$$

Therefore, the new second row is

$$
R_2=(0,0,3).
$$

The first and third rows remain unchanged. The matrix after the first operation is

$$
\boxed{
A_1=\begin{pmatrix}
1 & 2 & -1\\
0 & 0 & 3\\
-1 & 1 & 3
\end{pmatrix}
}
$$

**How to reverse the first operation:**

The original operation subtracts \(2R_1\) from \(R_2\). To reverse it, add \(2R_1\) back to \(R_2\):

$$
\boxed{R_2\leftarrow R_2+2R_1}
$$

This restores the original second row.

### Step 3: Perform the second row operation

The second operation is

$$
R_3\leftarrow R_3+R_1.
$$

We apply this operation to the matrix obtained in Step 2:

$$
A_1=\begin{pmatrix}
1 & 2 & -1\\
0 & 0 & 3\\
-1 & 1 & 3
\end{pmatrix}.
$$

The first and second rows remain unchanged. We replace the third row with the sum of the third row and the first row.

The relevant rows are

$$
R_3=(-1,1,3)
$$

and

$$
R_1=(1,2,-1).
$$

Add their corresponding entries:

$$
R_3+R_1=(-1+1,\;1+2,\;3+(-1)).
$$

Simplifying gives

$$
R_3+R_1=(0,3,2).
$$

Therefore, the new third row is

$$
R_3=(0,3,2).
$$

The matrix after the second operation is

$$
\boxed{
A_2=\begin{pmatrix}
1 & 2 & -1\\
0 & 0 & 3\\
0 & 3 & 2
\end{pmatrix}
}
$$

**How to reverse the second operation:**

The original operation adds \(R_1\) to \(R_3\). To reverse it, subtract \(R_1\) from \(R_3\):

$$
\boxed{R_3\leftarrow R_3-R_1}
$$

This restores the third row to its value before the second operation.

### Step 4: Perform the third row operation

The third operation is to interchange \(R_2\) and \(R_3\).

Before the interchange, the matrix is

$$
A_2=\begin{pmatrix}
1 & 2 & -1\\
0 & 0 & 3\\
0 & 3 & 2
\end{pmatrix}.
$$

The second row is

$$
R_2=(0,0,3),
$$

and the third row is

$$
R_3=(0,3,2).
$$

Interchanging the two rows means that the second row becomes \((0,3,2)\), while the third row becomes \((0,0,3)\). The first row stays unchanged.

The resulting matrix is

$$
\boxed{
A_3=\begin{pmatrix}
1 & 2 & -1\\
0 & 3 & 2\\
0 & 0 & 3
\end{pmatrix}
}
$$

**How to reverse the third operation:**

Interchanging the same two rows again restores their original positions:

$$
\boxed{\text{Interchange }R_2\text{ and }R_3}
$$

Swapping two rows twice returns the matrix to its original arrangement.

### Step 5: Summarize the three operations and their inverses

| Step | Original operation | Resulting matrix | Inverse operation |
|---|---|---|---|
| 1 | \(R_2\leftarrow R_2-2R_1\) | \(A_1\) | \(R_2\leftarrow R_2+2R_1\) |
| 2 | \(R_3\leftarrow R_3+R_1\) | \(A_2\) | \(R_3\leftarrow R_3-R_1\) |
| 3 | Interchange \(R_2\) and \(R_3\) | \(A_3\) | Interchange \(R_2\) and \(R_3\) again |

Each inverse operation undoes the corresponding original operation. To reverse the entire sequence, the operations must be undone in reverse order: first swap \(R_2\) and \(R_3\), then subtract \(R_1\) from \(R_3\), and finally add \(2R_1\) to \(R_2\).

### Final Answer

After the first operation,

$$
\boxed{
A_1=\begin{pmatrix}
1 & 2 & -1\\
0 & 0 & 3\\
-1 & 1 & 3
\end{pmatrix}
}
$$

After the second operation,

$$
\boxed{
A_2=\begin{pmatrix}
1 & 2 & -1\\
0 & 0 & 3\\
0 & 3 & 2
\end{pmatrix}
}
$$

After the third operation,

$$
\boxed{
A_3=\begin{pmatrix}
1 & 2 & -1\\
0 & 3 & 2\\
0 & 0 & 3
\end{pmatrix}
}
$$

The inverse operations are, respectively,

$$
R_2\leftarrow R_2+2R_1,
$$

$$
R_3\leftarrow R_3-R_1,
$$

and interchanging \(R_2\) and \(R_3\) again.

These calculations demonstrate that elementary row operations are reversible. This property is important in Gaussian elimination, where row operations simplify matrices while preserving the solutions of the corresponding system of linear equations.
