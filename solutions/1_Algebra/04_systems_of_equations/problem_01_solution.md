
# EXERCISE 1 – FROM A SYSTEM TO A MATRIX

## Given

Write the following system of equations in the form Ax = b.

$$
\begin{cases}
2x-y+z=4\\
x+3y-2z=1\\
3x+y+z=7
\end{cases}
$$

Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

## Solution

### Step 1 – Identify the Coefficients

The coefficients of x, y, and z in each equation are:

- First equation: 2, -1, 1
- Second equation: 1, 3, -2
- Third equation: 3, 1, 1

### Step 2 – Write the Matrix Equation

The coefficient matrix is:

$$
A=
\begin{pmatrix}
2&-1&1\\
1&3&-2\\
3&1&1
\end{pmatrix}
$$

The vector of unknowns is:

$$
x=
\begin{pmatrix}
x\\
y\\
z
\end{pmatrix}
$$

The right-hand side vector is:

$$
b=
\begin{pmatrix}
4\\
1\\
7
\end{pmatrix}
$$

Therefore, the system can be written as:

$$
\boxed{Ax=b}
$$

$$
\begin{pmatrix}
2&-1&1\\
1&3&-2\\
3&1&1
\end{pmatrix}
\begin{pmatrix}
x\\
y\\
z
\end{pmatrix}
=
\begin{pmatrix}
4\\
1\\
7
\end{pmatrix}
$$

### Step 3 – Explain the Rows

Each row of the coefficient matrix represents one equation.

- The first row (2, -1, 1) represents the equation 2x - y + z = 4.
- The second row (1, 3, -2) represents the equation x + 3y - 2z = 1.
- The third row (3, 1, 1) represents the equation 3x + y + z = 7.

The right-hand side vector contains the constants from each equation in the same order.

### Final Answer

The coefficient matrix, unknown vector, and right-hand side vector are:

$$
\boxed{
A=
\begin{pmatrix}
2&-1&1\\
1&3&-2\\
3&1&1
\end{pmatrix}
}
$$

$$
\boxed{
x=
\begin{pmatrix}
x\\y\\z
\end{pmatrix},
\qquad
b=
\begin{pmatrix}
4\\1\\7
\end{pmatrix}
}
$$

---

# EXERCISE 2 – GAUSSIAN ELIMINATION: ONE SOLUTION

## Given

Solve the following system using Gaussian elimination:

$$
\begin{cases}
x+y+z=6\\
2x-y+z=3\\
x+2y-z=2
\end{cases}
$$

After solving, substitute the result into all equations and check consistency.

## Solution

### Step 1 – Write the Augmented Matrix

$$
\left[
\begin{array}{ccc|c}
1&1&1&6\\
2&-1&1&3\\
1&2&-1&2
\end{array}
\right]
$$

### Step 2 – Eliminate the First Column

Apply the row operations:

$$
R_2\rightarrow R_2-2R_1
$$

$$
R_3\rightarrow R_3-R_1
$$

The new matrix is:

$$
\left[
\begin{array}{ccc|c}
1&1&1&6\\
0&-3&-1&-9\\
0&1&-2&-4
\end{array}
\right]
$$

### Step 3 – Swap the Second and Third Rows

Apply:

$$
R_2\leftrightarrow R_3
$$

The new matrix is:

$$
\left[
\begin{array}{ccc|c}
1&1&1&6\\
0&1&-2&-4\\
0&-3&-1&-9
\end{array}
\right]
$$

### Step 4 – Eliminate the Second Column

Apply:

$$
R_3\rightarrow R_3+3R_2
$$

The new matrix is:

$$
\left[
\begin{array}{ccc|c}
1&1&1&6\\
0&1&-2&-4\\
0&0&-7&-21
\end{array}
\right]
$$

### Step 5 – Make the Third Pivot Equal to 1

Apply:

$$
R_3\rightarrow -\frac{1}{7}R_3
$$

The new matrix is:

$$
\left[
\begin{array}{ccc|c}
1&1&1&6\\
0&1&-2&-4\\
0&0&1&3
\end{array}
\right]
$$

### Step 6 – Eliminate the Remaining Entries

First, apply:

$$
R_2\rightarrow R_2+2R_3
$$

Then:

$$
R_1\rightarrow R_1-R_2-R_3
$$

The final matrix is:

$$
\left[
\begin{array}{ccc|c}
1&0&0&1\\
0&1&0&2\\
0&0&1&3
\end{array}
\right]
$$

Therefore:

$$
x=1,\qquad y=2,\qquad z=3
$$

### Step 7 – Check the Solution

Substitute the values into the original equations.

First equation:

$$
1+2+3=6
$$

Second equation:

$$
2(1)-2+3=3
$$

Third equation:

$$
1+2(2)-3=2
$$

All three equations are satisfied
