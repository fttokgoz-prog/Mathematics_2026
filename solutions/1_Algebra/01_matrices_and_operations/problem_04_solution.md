# Exercise 4. Matrix Multiplication and Noncommutativity

## Question

For the matrices

$$
A=\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix},
\qquad
B=\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
$$

compute \(AB\) and \(BA\). Is \(AB=BA\)? Use this example to explain what noncommutativity of matrix multiplication means.

**Why this exercise:** Shows one of the most important differences between matrix multiplication and multiplication of numbers.

## Solution

### Step 1: Understand the matrix multiplication rule

To multiply two matrices, the number of columns in the first matrix must equal the number of rows in the second matrix.

Both \(A\) and \(B\) are \(2\times2\) matrices. Therefore, both products \(AB\) and \(BA\) are defined, and each result is also a \(2\times2\) matrix.

Each entry of the result is calculated by multiplying the elements of a row of the first matrix by the corresponding elements of a column of the second matrix and then adding the products.

### Step 2: Calculate \(AB\)

We multiply matrix \(A\) by matrix \(B\):

$$
AB=
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
$$

**Entry in row 1, column 1:**

$$
1\cdot2+2\cdot3=2+6=8
$$

**Entry in row 1, column 2:**

$$
1\cdot0+2\cdot1=0+2=2
$$

**Entry in row 2, column 1:**

$$
0\cdot2+1\cdot3=0+3=3
$$

**Entry in row 2, column 2:**

$$
0\cdot0+1\cdot1=0+1=1
$$

Combining these four entries gives

$$
\boxed{
AB=\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
}
$$

### Step 3: Calculate \(BA\)

Now we reverse the order and multiply matrix \(B\) by matrix \(A\):

$$
BA=
\begin{pmatrix}
2 & 0\\
3 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 2\\
0 & 1
\end{pmatrix}
$$

**Entry in row 1, column 1:**

$$
2\cdot1+0\cdot0=2+0=2
$$

**Entry in row 1, column 2:**

$$
2\cdot2+0\cdot1=4+0=4
$$

**Entry in row 2, column 1:**

$$
3\cdot1+1\cdot0=3+0=3
$$

**Entry in row 2, column 2:**

$$
3\cdot2+1\cdot1=6+1=7
$$

Combining these entries gives

$$
\boxed{
BA=\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
}
$$

### Step 4: Compare \(AB\) and \(BA\)

We obtained

$$
AB=\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
$$

and

$$
BA=\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
$$

Two matrices are equal only if all their corresponding entries are equal.

However, their top-left entries are different:

$$
8\neq2
$$

Their top-right entries are also different:

$$
2\neq4
$$

Therefore,

$$
\boxed{AB\neq BA}
$$

### Step 5: Explain noncommutativity

For ordinary numbers, multiplication is commutative. This means that changing the order of the factors does not change the result:

$$
2\cdot3=3\cdot2=6
$$

However, matrix multiplication is **not commutative in general**. Reversing the order of two matrices can produce a different result.

In this example,

$$
AB=
\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
\neq
\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
=BA
$$

This difference occurs because reversing the order changes which rows and columns are multiplied together.

Noncommutativity does not mean that \(AB\) and \(BA\) are always different. Some pairs of matrices do satisfy \(AB=BA\). It means that, unlike ordinary number multiplication, matrix multiplication does not guarantee the same result when the order is reversed.

### Final Answer

$$
AB=\begin{pmatrix}
8 & 2\\
3 & 1
\end{pmatrix}
$$

$$
BA=\begin{pmatrix}
2 & 4\\
3 & 7
\end{pmatrix}
$$

$$
\boxed{AB\neq BA}
$$

Matrix multiplication is not commutative in general because changing the order of the matrices can change the result.
