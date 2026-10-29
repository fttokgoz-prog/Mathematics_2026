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

1. $$R_2 \leftarrow R_2-2R_1$$
2. $$R_3 \leftarrow R_3+R_1$$
3. Interchange \(R_2\) and \(R_3\).

Write the matrix after each step. Then, for each of the three operations, state an operation that reverses it.

**Why this exercise:** Prepares for elimination by showing that row operations are controlled and reversible transformations of a matrix.

## Solution

### Step 1: Perform the first row operation

The first operation is

$$
R_2 \leftarrow R_2-2R_1.
$$

This means that we replace the second row with the second row minus twice the first row. The other rows remain unchanged.

The original matrix is

$$
A=\begin{pmatrix}
1 & 2 & -1\\
2 & 4 & 1\\
-1 & 1 & 3
\end{pmatrix}.
$$

The first row is

$$
R_1=(1,2,-1).
$$

The second row is

$$
R_2=(2,4,1).
$$

First, multiply the first row by \(2\):

$$
2R_1=(2,4,-2).
$$

Now subtract \(2R_1\) from \(R_2\):

$$
R_2-2R_1=(2,4,1)-(2,4,-2).
$$

Subtract the corresponding entries:

$$
R_2-2R_1=(2-2,\;4-4,\;1-(-2)).
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

**Inverse operation:**

To reverse the operation, add \(2R_1\) back to \(R_2\):

$$
\boxed{R_2 \leftarrow R_2+2R_1}
$$

This restores the original second row.

### Step 2: Perform the second row operation

The second operation is

$$
R_3 \leftarrow R_3+R_1.
$$

We apply it to the matrix obtained in Step 1:

$$
A_1=\begin{pmatrix}
1 & 2 & -1\\
0 & 0 & 3\\
-1 & 1 & 3
\end{pmatrix}.
$$

The first row is

$$
R_1=(1,2,-1),
$$

and the third row is

$$
R_3=(-1,1,3).
$$

Add the corresponding entries:

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

**Inverse operation:**

To reverse the operation, subtract \(R_1\) from \(R_3\):

$$
\boxed{R_3 \leftarrow R_3-R_1}
$$

This restores the third row to its value before Step 2.

### Step 3: Interchange \(R_2\) and \(R_3\)

Before the interchange, the matrix is

$$
A_2=\begin{pmatrix}
1 & 2 & -1
