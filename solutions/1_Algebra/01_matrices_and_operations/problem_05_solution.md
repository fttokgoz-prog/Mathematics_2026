# Exercise 5. Matrix Times Vector

## Question

Let

$$
A=\begin{pmatrix}
2 & -1\\
1 & 3
\end{pmatrix},
\qquad
x=\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

Compute \(Ax\). Then express \(Ax\) as a linear combination of the columns of \(A\), with coefficients coming from the vector \(x\).

**Why this exercise:** Shows that multiplying a matrix by a vector can be understood as a linear combination of the matrix columns.

## Solution

### Step 1: Understand the dimensions

The matrix \(A\) has 2 rows and 2 columns, so its dimensions are \(2\times2\).

The vector \(x\) has 2 rows and 1 column, so its dimensions are \(2\times1\).

Matrix multiplication is possible because the number of columns in \(A\) equals the number of rows in \(x\). Therefore, the result \(Ax\) will be a \(2\times1\) vector.

### Step 2: Calculate \(Ax\)

We are given

$$
A=\begin{pmatrix}
2 & -1\\
1 & 3
\end{pmatrix},
\qquad
x=\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

Multiply each row of \(A\) by the column vector \(x\):

$$
Ax=
\begin{pmatrix}
2 & -1\\
1 & 3
\end{pmatrix}
\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

**First entry:**

Multiply the first row of \(A\), \((2,-1)\), by the vector \(x\):

$$
2\cdot4+(-1)\cdot2=8-2=6
$$

**Second entry:**

Multiply the second row of \(A\), \((1,3)\), by the vector \(x\):

$$
1\cdot4+3\cdot2=4+6=10
$$

Combining the two entries gives

$$
\boxed{
Ax=\begin{pmatrix}
6\\
10
\end{pmatrix}
}
$$

### Step 3: Identify the columns of \(A\)

To express \(Ax\) as a linear combination of the columns of \(A\), we first write the columns separately.

The first column of \(A\) is

$$
a_1=\begin{pmatrix}
2\\
1
\end{pmatrix}
$$

The second column of \(A\) is

$$
a_2=\begin{pmatrix}
-1\\
3
\end{pmatrix}
$$

Therefore, the matrix \(A\) can be written using its column vectors as

$$
A=\begin{pmatrix}a_1 & a_2\end{pmatrix}
$$

The vector \(x\) contains the coefficients \(4\) and \(2\):

$$
x=\begin{pmatrix}
4\\
2
\end{pmatrix}
$$

The first coefficient is \(4\), and the second coefficient is \(2\).

### Step 4: Express \(Ax\) as a linear combination

A matrix multiplied by a vector can be expressed as a linear combination of the matrix's columns. Each column is multiplied by the corresponding entry of the vector.

In general, if

$$
A=\begin{pmatrix}a_1 & a_2\end{pmatrix},
\qquad
x=\begin{pmatrix}x_1\\x_2\end{pmatrix},
$$

then

$$
Ax=x_1a_1+x_2a_2
$$

For this exercise, \(x_1=4\) and \(x_2=2\). Therefore,

$$
Ax=4a_1+2a_2
$$

Substitute the column vectors:

$$
Ax=
4\begin{pmatrix}
2\\
1
\end{pmatrix}
+
2\begin{pmatrix}
-1\\
3
\end{pmatrix}
$$

Multiply each vector by its coefficient:

$$
Ax=
\begin{pmatrix}
8\\
4
\end{pmatrix}
+
\begin{pmatrix}
-2\\
6
\end{pmatrix}
$$

Add the corresponding entries:

$$
Ax=
\begin{pmatrix}
8+(-2)\\
4+6
\end{pmatrix}
=
\begin{pmatrix}
6\\
10
\end{pmatrix}
$$

Thus, the linear combination gives the same result as the direct matrix multiplication.

### Step 5: Explain the result

We calculated \(Ax\) in two different ways.

Using direct matrix multiplication:

$$
Ax=\begin{pmatrix}
6\\
10
\end{pmatrix}
$$

Using a linear combination of the columns of \(A\):

$$
Ax=
4\begin{pmatrix}
2\\
1
\end{pmatrix}
+
2\begin{pmatrix}
-1\\
3
\end{pmatrix}
=
\begin{pmatrix}
6\\
10
\end{pmatrix}
$$

Both methods produce the same vector.

This demonstrates that multiplying a matrix by a vector means taking a weighted sum of the matrix's columns. The entries of the vector provide the coefficients used to multiply each column.

### Final Answer

The matrix-vector product is

$$
\boxed{
Ax=\begin{pmatrix}
6\\
10
\end{pmatrix}
}
$$

The linear combination of the columns of \(A\) is

$$
\boxed{
Ax=
4\begin{pmatrix}
2\\
1
\end{pmatrix}
+
2\begin{pmatrix}
-1\\
3
\end{pmatrix}
}
$$

The coefficients \(4\) and \(2\) come directly from the vector \(x\), and the linear combination produces the same result as the matrix-vector multiplication.
