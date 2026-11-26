
# EXERCISE 8 – TWO SYSTEMS WITH THE SAME COEFFICIENT MATRIX

## Given

Solve by elimination the following two systems:

**System 1:**

$$
\begin{cases}
2x+y=5\\
x-y=1
\end{cases}
$$

**System 2:**

$$
\begin{cases}
2x+y=1\\
x-y=4
\end{cases}
$$

Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

## Solution

### Step 1 – Identify the Coefficient Matrix

Both systems have the same coefficients for x and y.

The coefficient matrix is:

$$
A=
\begin{pmatrix}
2&1\\
1&-1
\end{pmatrix}
$$

Only the right-hand side vectors are different.

### Step 2 – Solve System 1

The first system is:

$$
\begin{cases}
2x+y=5\\
x-y=1
\end{cases}
$$

Write the augmented matrix:

$$
\left[
\begin{array}{cc|c}
2&1&5\\
1&-1&1
\end{array}
\right]
$$

Apply the row operation:

$$
R_2\rightarrow 2R_2-R_1
$$

The new matrix is:

$$
\left[
\begin{array}{cc|c}
2&1&5\\
0&-3&-3
\end{array}
\right]
$$

The second row gives:

$$
-3y=-3
$$

Therefore:

$$
y=1
$$

Substitute y = 1 into the first equation:

$$
2x+1=5
$$

$$
2x=4
$$

$$
x=2
$$

The solution of System 1 is:

$$
x=2,\quad y=1
$$

### Step 3 – Check System 1

Substitute the values into the original equations.

First equation:

$$
2(2)+1=5
$$

Second equation:

$$
2-1=1
$$

Both equations are satisfied.

### Step 4 – Solve System 2

The second system is:

$$
\begin{cases}
2x+y=1\\
x-y=4
\end{cases}
$$

Write the augmented matrix:

$$
\left[
\begin{array}{cc|c}
2&1&1\\
1&-1&4
\end{array}
\right]
$$

Apply the same row operation:

$$
R_2\rightarrow 2R_2-R_1
$$

The new matrix is:

$$
\left[
\begin{array}{cc|c}
2&1&1\\
0&-3&7
\end{array}
\right]
$$

The second row gives:

$$
-3y=7
$$

Therefore:

$$
y=-\frac{7}{3}
$$

Substitute this value into the first equation:

$$
2x-\frac{7}{3}=1
$$

$$
2x=1+\frac{7}{3}
$$

$$
2x=\frac{10}{3}
$$

Therefore:

$$
x=\frac{5}{3}
$$

The solution of System 2 is:

$$
x=\frac{5}{3},\quad y=-\frac{7}{3}
$$

### Step 5 – Check System 2

Substitute the values into the original equations.

First equation:

$$
2\left(\frac{5}{3}\right)-\frac{7}{3}=1
$$

$$
\frac{10}{3}-\frac{7}{3}=1
$$

Second equation:

$$
\frac{5}{3}-\left(-\frac{7}{3}\right)=4
$$

$$
\frac{12}{3}=4
$$

Both equations are satisfied.

### Step 6 – Compare the Elimination Steps

The same row operation is used in both systems:

$$
R_2\rightarrow 2R_2-R_1
$$

In both cases, the first entry of the second row becomes zero.

The coefficient part of the calculation is identical because both systems have the same coefficient matrix.

However, the right-hand side calculations are different.

For System 1:

$$
2(1)-5=-3
$$

For System 2:

$$
2(4)-1=7
$$

Therefore, the elimination produces the same coefficient row but different constant values.

### Final Answers

**System 1:**

$$
x=2,\quad y=1
$$

**System 2:**

$$
x=\frac{5}{3},\quad y=-\frac{7}{3}
$$

### Conclusion

Both systems have the same coefficient matrix, so the elimination steps involving the coefficients are identical.

The only difference is the right-hand side vector, which changes the final values obtained during elimination.

This demonstrates that the coefficient matrix determines the elimination structure, while the right-hand side determines the particular solution.
