# Exercise 7. Identity Matrix, Zero Matrix, and Powers

## Question

For

$$
A=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

compute

$$
AI,\qquad IA,\qquad A+0,\qquad A^2,\qquad A^3.
$$

Explain the roles of the matrices \(I\) and \(0\), and describe the pattern you observe in successive powers of \(A\).

**Why this exercise:** Organizes the roles of neutral elements and reveals regularity in successive powers of a matrix.

## Solution

### Step 1: Understand the identity matrix and the zero matrix

The identity matrix \(I\) is a square matrix with ones on its main diagonal and zeros everywhere else. For a \(2\times2\) matrix, it is

$$
I=\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}.
$$

Multiplying a matrix by the identity matrix does not change the matrix. This is similar to multiplying an ordinary number by \(1\).

The zero matrix \(0\) contains only zeros. For a \(2\times2\) matrix, it is

$$
0=\begin{pmatrix}
0 & 0\\
0 & 0
\end{pmatrix}.
$$

Adding the zero matrix to a matrix does not change its entries. This is similar to adding \(0\) to an ordinary number.

We are given

$$
A=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}.
$$

### Step 2: Calculate \(AI\)

We multiply \(A\) by the identity matrix:

$$
AI=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}.
$$

Calculate each entry.

First row, first column:

$$
2\cdot1+1\cdot0=2
$$

First row, second column:

$$
2\cdot0+1\cdot1=1
$$

Second row, first column:

$$
0\cdot1+2\cdot0=0
$$

Second row, second column:

$$
0\cdot0+2\cdot1=2
$$

Therefore,

$$
\boxed{
AI=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}=A
}
$$

Multiplication by the identity matrix leaves \(A\) unchanged.

### Step 3: Calculate \(IA\)

Now we reverse the order:

$$
IA=
\begin{pmatrix}
1 & 0\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}.
$$

First row, first column:

$$
1\cdot2+0\cdot0=2
$$

First row, second column:

$$
1\cdot1+0\cdot2=1
$$

Second row, first column:

$$
0\cdot2+1\cdot0=0
$$

Second row, second column:

$$
0\cdot1+1\cdot2=2
$$

Therefore,

$$
\boxed{
IA=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}=A
}
$$

The identity matrix leaves \(A\) unchanged whether it is multiplied on the left or on the right. Thus,

$$
\boxed{AI=IA=A}
$$

### Step 4: Calculate \(A+0\)

We add the zero matrix to \(A\):

$$
A+0=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
+
\begin{pmatrix}
0 & 0\\
0 & 0
\end{pmatrix}.
$$

Matrix addition is performed by adding corresponding entries.

$$
A+0=
\begin{pmatrix}
2+0 & 1+0\\
0+0 & 2+0
\end{pmatrix}.
$$

Simplifying each entry gives

$$
\boxed{
A+0=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}=A
}
$$

The zero matrix is the additive identity because adding it does not change the original matrix.

### Step 5: Calculate \(A^2\)

The notation \(A^2\) means multiplying \(A\) by itself:

$$
A^2=A\cdot A.
$$

Therefore,

$$
A^2=
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}.
$$

First row, first column:

$$
2\cdot2+1\cdot0=4
$$

First row, second column:

$$
2\cdot1+1\cdot2=2+2=4
$$

Second row, first column:

$$
0\cdot2+2\cdot0=0
$$

Second row, second column:

$$
0\cdot1+2\cdot2=4
$$

Combining the entries gives

$$
\boxed{
A^2=\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
}
$$

Notice that the diagonal entries have increased from \(2\) to \(4\), and the upper-right entry has increased from \(1\) to \(4\).

### Step 6: Calculate \(A^3\)

The notation \(A^3\) means multiplying \(A^2\) by \(A\):

$$
A^3=A^2A.
$$

Using the result from Step 5,

$$
A^3=
\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}.
$$

First row, first column:

$$
4\cdot2+4\cdot0=8
$$

First row, second column:

$$
4\cdot1+4\cdot2=4+8=12
$$

Second row, first column:

$$
0\cdot2+4\cdot0=0
$$

Second row, second column:

$$
0\cdot1+4\cdot2=8
$$

Therefore,

$$
\boxed{
A^3=\begin{pmatrix}
8 & 12\\
0 & 8
\end{pmatrix}
}
$$

### Step 7: Describe the pattern in successive powers of \(A\)

We obtained the following matrices:

$$
A=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
$$

$$
A^2=\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
$$

$$
A^3=\begin{pmatrix}
8 & 12\\
0 & 8
\end{pmatrix}
$$

The diagonal entries follow the pattern

$$
2,\quad 4,\quad 8.
$$

Each diagonal entry is twice the previous one. For \(A^n\), the diagonal entries are \(2^n\).

The lower-left entry remains \(0\) in every power because the product of upper-triangular matrices is also upper triangular.

The upper-right entries are

$$
1,\quad 4,\quad 12.
$$

For this particular matrix, the general pattern is

$$
A^n=
\begin{pmatrix}
2^n & n2^{n-1}\\
0 & 2^n
\end{pmatrix},
\qquad n\geq1.
$$

For example, when \(n=2\), the upper-right entry is

$$
2\cdot2^{2-1}=2\cdot2=4.
$$

When \(n=3\), it is

$$
3\cdot2^{3-1}=3\cdot4=12.
$$

This formula matches the results calculated for \(A^2\) and \(A^3\).

### Step 8: Explain the roles of \(I\) and \(0\)

The identity matrix \(I\) is the multiplicative identity. Multiplying \(A\) by \(I\) on either side leaves \(A\) unchanged:

$$
AI=IA=A.
$$

The zero matrix \(0\) is the additive identity. Adding it to \(A\) leaves \(A\) unchanged:

$$
A+0=A.
$$

These matrices play roles similar to the numbers \(1\) and \(0\), respectively, in ordinary arithmetic.

### Final Answer

The identity-matrix products are

$$
\boxed{
AI=IA=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
}
$$

The sum with the zero matrix is

$$
\boxed{
A+0=\begin{pmatrix}
2 & 1\\
0 & 2
\end{pmatrix}
}
$$

The second power is

$$
\boxed{
A^2=\begin{pmatrix}
4 & 4\\
0 & 4
\end{pmatrix}
}
$$

The third power is

$$
\boxed{
A^3=\begin{pmatrix}
8 & 12\\
0 & 8
\end{pmatrix}
}
$$

The identity matrix leaves a matrix unchanged under multiplication, while the zero matrix leaves it unchanged under addition. In successive powers of \(A\), the diagonal entries double at each step, the lower-left entry remains zero, and the upper-right entry follows the pattern \(n2^{n-1}\).
