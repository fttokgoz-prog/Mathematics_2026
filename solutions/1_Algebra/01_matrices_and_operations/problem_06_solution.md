# Exercise 6. Transpose

## Question

For the matrices

$$
A=\begin{pmatrix}
1 & 2 & 3\\
4 & 5 & 6
\end{pmatrix},
\qquad
B=\begin{pmatrix}
1 & 0\\
2 & 1\\
-1 & 3
\end{pmatrix}
$$

compute \(A^T\), \(B^T\), and \(AB\). Then verify in this example that

$$
(AB)^T=B^T A^T.
$$

**Why this exercise:** Teaches transposition and an important property that reverses the order of factors.

## Solution

### Step 1: Understand the transpose of a matrix

The transpose of a matrix is obtained by exchanging its rows and columns. Each row of the original matrix becomes a column of the transposed matrix, and each column becomes a row.

The transpose of a matrix \(A\) is denoted by \(A^T\).

For example, if

$$
A=\begin{pmatrix}
a & b & c\\
d & e & f
\end{pmatrix},
$$

then

$$
A^T=\begin{pmatrix}
a & d\\
b & e\\
c & f
\end{pmatrix}.
$$

Since \(A\) has dimensions \(2\times3\), its transpose \(A^T\) will have dimensions \(3\times2\).

Similarly, \(B\) has dimensions \(3\times2\), so \(B^T\) will have dimensions \(2\times3\).

### Step 2: Calculate \(A^T\)

The original matrix is

$$
A=\begin{pmatrix}
1 & 2 & 3\\
4 & 5 & 6
\end{pmatrix}.
$$

The first row, \((1,2,3)\), becomes the first column. The second row, \((4,5,6)\), becomes the second column.

Therefore,

$$
\boxed{
A^T=\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}
}
$$

The original matrix has dimensions \(2\times3\), while its transpose has dimensions \(3\times2\).

### Step 3: Calculate \(B^T\)

The original matrix is

$$
B=\begin{pmatrix}
1 & 0\\
2 & 1\\
-1 & 3
\end{pmatrix}.
$$

The first column, \((1,2,-1)\), becomes the first row. The second column, \((0,1,3)\), becomes the second row.

Therefore,

$$
\boxed{
B^T=\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
}
$$

The original matrix has dimensions \(3\times2\), while its transpose has dimensions \(2\times3\).

### Step 4: Calculate \(AB\)

We are given

$$
A=\begin{pmatrix}
1 & 2 & 3\\
4 & 5 & 6
\end{pmatrix},
\qquad
B=\begin{pmatrix}
1 & 0\\
2 & 1\\
-1 & 3
\end{pmatrix}.
$$

Matrix \(A\) has 3 columns, and matrix \(B\) has 3 rows. Therefore, \(AB\) is defined. The result has dimensions \(2\times2\).

$$
AB=
\begin{pmatrix}
1 & 2 & 3\\
4 & 5 & 6
\end{pmatrix}
\begin{pmatrix}
1 & 0\\
2 & 1\\
-1 & 3
\end{pmatrix}
$$

**Entry in row 1, column 1:**

$$
1\cdot1+2\cdot2+3\cdot(-1)
=1+4-3=2
$$

**Entry in row 1, column 2:**

$$
1\cdot0+2\cdot1+3\cdot3
=0+2+9=11
$$

**Entry in row 2, column 1:**

$$
4\cdot1+5\cdot2+6\cdot(-1)
=4+10-6=8
$$

**Entry in row 2, column 2:**

$$
4\cdot0+5\cdot1+6\cdot3
=0+5+18=23
$$

Combining these entries gives

$$
\boxed{
AB=\begin{pmatrix}
2 & 11\\
8 & 23
\end{pmatrix}
}
$$

### Step 5: Calculate \((AB)^T\)

From Step 4, we obtained

$$
AB=\begin{pmatrix}
2 & 11\\
8 & 23
\end{pmatrix}.
$$

To calculate \((AB)^T\), exchange the rows and columns. The first row becomes the first column, and the second row becomes the second column.

Therefore,

$$
\boxed{
(AB)^T=\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}
}
$$

### Step 6: Calculate \(B^T A^T\)

We have already calculated

$$
B^T=\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
$$

and

$$
A^T=\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}.
$$

The matrix \(B^T\) has dimensions \(2\times3\), and \(A^T\) has dimensions \(3\times2\). Therefore, their product is defined and has dimensions \(2\times2\).

$$
B^T A^T=
\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}
$$

**Entry in row 1, column 1:**

$$
1\cdot1+2\cdot2+(-1)\cdot3
=1+4-3=2
$$

**Entry in row 1, column 2:**

$$
1\cdot4+2\cdot5+(-1)\cdot6
=4+10-6=8
$$

**Entry in row 2, column 1:**

$$
0\cdot1+1\cdot2+3\cdot3
=0+2+9=11
$$

**Entry in row 2, column 2:**

$$
0\cdot4+1\cdot5+3\cdot6
=0+5+18=23
$$

Therefore,

$$
\boxed{
B^T A^T=\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}
}
$$

### Step 7: Verify the transpose property

We calculated both sides of the required identity.

The transpose of the product is

$$
(AB)^T=\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}.
$$

The product of the transposed matrices in reverse order is

$$
B^T A^T=\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}.
$$

Both matrices are identical. Therefore, the identity is verified:

$$
\boxed{(AB)^T=B^T A^T}
$$

Notice that the order of the matrices is reversed. The transpose of \(AB\) is \(B^T A^T\), not \(A^T B^T\).

### Final Answer

The transpose of \(A\) is

$$
\boxed{
A^T=\begin{pmatrix}
1 & 4\\
2 & 5\\
3 & 6
\end{pmatrix}
}
$$

The transpose of \(B\) is

$$
\boxed{
B^T=\begin{pmatrix}
1 & 2 & -1\\
0 & 1 & 3
\end{pmatrix}
}
$$

The product of \(A\) and \(B\) is

$$
\boxed{
AB=\begin{pmatrix}
2 & 11\\
8 & 23
\end{pmatrix}
}
$$

Finally,

$$
(AB)^T=B^T A^T=
\begin{pmatrix}
2 & 8\\
11 & 23
\end{pmatrix}.
$$

Thus, the identity \((AB)^T=B^T A^T\) is verified. Transposing a product reverses the order of its factors.
