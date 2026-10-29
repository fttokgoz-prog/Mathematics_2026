# Exercise 10. Columns of a Matrix Product

## Question

Given

$$
A=\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix},
\qquad
B=\begin{pmatrix}
1 & 2\\
-1 & 0\\
3 & 1
\end{pmatrix}.
$$

Denote the columns of \(B\) by \(b_1,b_2\).

1. Compute \(Ab_1\) and \(Ab_2\).
2. Compute the matrix \(AB\).
3. Compare the results and explain why the columns of \(AB\) are exactly the vectors \(Ab_1\) and \(Ab_2\).

**Why this exercise:** Extends the interpretation of matrix-vector multiplication to a full product of two matrices instead of simply repeating another \(Ax\) exercise.

## Solution

### Step 1: Understand the dimensions of the matrices

The given matrices are

$$
A=\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix},
\qquad
B=\begin{pmatrix}
1 & 2\\
-1 & 0\\
3 & 1
\end{pmatrix}.
$$

Matrix \(A\) has 2 rows and 3 columns, so its dimensions are \(2\times3\).

Matrix \(B\) has 3 rows and 2 columns, so its dimensions are \(3\times2\).

Since the number of columns of \(A\) equals the number of rows of \(B\), the product \(AB\) is defined. The result will have 2 rows and 2 columns.

### Step 2: Identify the columns of \(B\)

The first column of \(B\) is denoted by \(b_1\):

$$
b_1=\begin{pmatrix}
1\\
-1\\
3
\end{pmatrix}.
$$

The second column of \(B\) is denoted by \(b_2\):

$$
b_2=\begin{pmatrix}
2\\
0\\
1
\end{pmatrix}.
$$

Therefore, we can write \(B\) in terms of its columns as

$$
B=\begin{pmatrix}b_1 & b_2\end{pmatrix}.
$$

### Step 3: Calculate \(Ab_1\)

We multiply matrix \(A\) by the first column of \(B\):

$$
Ab_1=
\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1\\
-1\\
3
\end{pmatrix}.
$$

The first entry is obtained by multiplying the first row of \(A\) by \(b_1\):

$$
1\cdot1+2\cdot(-1)+0\cdot3
=1-2+0=-1.
$$

The second entry is obtained by multiplying the second row of \(A\) by \(b_1\):

$$
0\cdot1+1\cdot(-1)+1\cdot3
=0-1+3=2.
$$

Combining the entries gives

$$
\boxed{
Ab_1=\begin{pmatrix}
-1\\
2
\end{pmatrix}
}
$$

### Step 4: Calculate \(Ab_2\)

Now we multiply matrix \(A\) by the second column of \(B\):

$$
Ab_2=
\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
2\\
0\\
1
\end{pmatrix}.
$$

The first entry is

$$
1\cdot2+2\cdot0+0\cdot1
=2+0+0=2.
$$

The second entry is

$$
0\cdot2+1\cdot0+1\cdot1
=0+0+1=1.
$$

Therefore,

$$
\boxed{
Ab_2=\begin{pmatrix}
2\\
1
\end{pmatrix}
}
$$

### Step 5: Calculate the matrix product \(AB\)

We now calculate the full product of the two matrices:

$$
AB=
\begin{pmatrix}
1 & 2 & 0\\
0 & 1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2\\
-1 & 0\\
3 & 1
\end{pmatrix}.
$$

The result has dimensions \(2\times2\).

**Entry in row 1, column 1:**

$$
1\cdot1+2\cdot(-1)+0\cdot3=-1
$$

**Entry in row 1, column 2:**

$$
1\cdot2+2\cdot0+0\cdot1=2
$$

**Entry in row 2, column 1:**

$$
0\cdot1+1\cdot(-1)+1\cdot3=2
$$

**Entry in row 2, column 2:**

$$
0\cdot2+1\cdot0+1\cdot1=1
$$

Putting these four entries into the result matrix gives

$$
\boxed{
AB=\begin{pmatrix}
-1 & 2\\
2 & 1
\end{pmatrix}
}
$$

### Step 6: Compare the results

From Steps 3 and 4, we obtained

$$
Ab_1=\begin{pmatrix}
-1\\
2
\end{pmatrix},
\qquad
Ab_2=\begin{pmatrix}
2\\
1
\end{pmatrix}.
$$

From Step 5, we calculated

$$
AB=\begin{pmatrix}
-1 & 2\\
2 & 1
\end{pmatrix}.
$$

The first column of \(AB\) is

$$
\begin{pmatrix}
-1\\
2
\end{pmatrix}=Ab_1.
$$

The second column of \(AB\) is

$$
\begin{pmatrix}
2\\
1
\end{pmatrix}=Ab_2.
$$

Thus, the matrix product can be written as

$$
\boxed{AB=\begin{pmatrix}Ab_1 & Ab_2\end{pmatrix}}
$$

### Step 7: Explain why the columns of \(AB\) are \(Ab_1\) and \(Ab_2\)

Matrix multiplication combines each row of \(A\) with each column of \(B\). Consequently, the entries in the first column of \(AB\) are calculated by multiplying the rows of \(A\) by the first column \(b_1\). This is exactly the calculation of \(Ab_1\).

Similarly, the entries in the second column of \(AB\) are calculated by multiplying the rows of \(A\) by the second column \(b_2\). This is exactly the calculation of \(Ab_2\).

Therefore, multiplying \(A\) by \(B\) is equivalent to multiplying \(A\) separately by each column of \(B\) and then placing the resulting vectors side by side.

This gives the general rule

$$
A\begin{pmatrix}b_1 & b_2\end{pmatrix}
=
\begin{pmatrix}Ab_1 & Ab_2\end{pmatrix}.
$$

The same principle applies to matrices with any compatible dimensions, not only to \(2\times3\) and \(3\times2\) matrices.

### Final Answer

The first column of \(B\) gives

$$
\boxed{
Ab_1=\begin{pmatrix}
-1\\
2
\end{pmatrix}
}
$$

The second column of \(B\) gives

$$
\boxed{
Ab_2=\begin{pmatrix}
2\\
1
\end{pmatrix}
}
$$

The complete matrix product is

$$
\boxed{
AB=\begin{pmatrix}
-1 & 2\\
2 & 1
\end{pmatrix}
}
$$

The columns of \(AB\) are exactly \(Ab_1\) and \(Ab_2\), because each column of the product is obtained by multiplying \(A\) by the corresponding column of \(B\).
