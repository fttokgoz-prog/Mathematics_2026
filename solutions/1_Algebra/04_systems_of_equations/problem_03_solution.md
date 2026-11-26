
# EXERCISE 3 – INCONSISTENT SYSTEM

## Given

Solve or show that the following system is inconsistent:

$$
\begin{cases}
x+2y=3\\
2x+4y=7
\end{cases}
$$

Show how the contradiction appears in the augmented matrix after elimination and interpret it in terms of equations.

## Solution

### Step 1 – Write the Augmented Matrix

We write the coefficients and constants in an augmented matrix.

$$
\left[
\begin{array}{cc|c}
1&2&3\\
2&4&7
\end{array}
\right]
$$

### Step 2 – Eliminate the First Column

Apply the row operation:

$$
R_2\rightarrow R_2-2R_1
$$

The new matrix is:

$$
\left[
\begin{array}{cc|c}
1&2&3\\
0&0&1
\end{array}
\right]
$$

### Step 3 – Identify the Contradiction

The second row represents the equation:

$$
0x+0y=1
$$

Simplifying gives:

$$
0=1
$$

This statement is impossible because zero can never be equal to one.

### Step 4 – Interpret the Result

The original equations are:

$$
x+2y=3
$$

$$
2x+4y=7
$$

If we multiply the first equation by 2, we get:

$$
2x+4y=6
$$

However, the second equation states:

$$
2x+4y=7
$$

The left-hand sides are identical, but the right-hand sides are different.

Therefore, the two equations cannot be true at the same time.

### Final Answer

The augmented matrix produces the contradiction:

$$
\left[
\begin{array}{cc|c}
1&2&3\\
0&0&1
\end{array}
\right]
$$

Since the second row represents 0 = 1, the system has no solution.

$$
\boxed{\text{No solution}}
$$

### Conclusion

The system is inconsistent because Gaussian elimination produces an impossible equation.

The contradiction shows that there is no pair of values for x and y that satisfies both original equations simultaneously.
