
# EXERCISE 11 – A PARAMETER IN A SYSTEM OF THREE EQUATIONS

## Given

Analyze the number of solutions depending on the parameter t:

$$
\begin{cases}
x+y+z=1\\
x+ty+z=2\\
x+y+tz=3
\end{cases}
$$

Use elimination and separately analyze the parameter values for which a standard calculation step ceases to be valid.

## Solution

### Step 1 – Write the Augmented Matrix

$$
\left[
\begin{array}{ccc|c}
1&1&1&1\\
1&t&1&2\\
1&1&t&3
\end{array}
\right]
$$

### Step 2 – Eliminate the First Column

Apply the following row operations:

$$
R_2\rightarrow R_2-R_1
$$

$$
R_3\rightarrow R_3-R_1
$$

The new matrix is:

$$
\left[
\begin{array}{ccc|c}
1&1&1&1\\
0&t-1&0&1\\
0&0&t-1&2
\end{array}
\right]
$$

### Step 3 – Analyze the Parameter

The second row represents:

$$
(t-1)y=1
$$

The third row represents:

$$
(t-1)z=2
$$

To calculate y and z, we would normally divide by t-1.

However, this division is only valid when:

$$
t-1\neq 0
$$

Therefore, we must consider two separate cases.

### Step 4 – Case 1: t is Not Equal to 1

If t is not equal to 1, we can divide by t-1.

From the second row:

$$
y=\frac{1}{t-1}
$$

From the third row:

$$
z=\frac{2}{t-1}
$$

Using the first equation:

$$
x+y+z=1
$$

Substitute the values of y and z:

$$
x+\frac{1}{t-1}+\frac{2}{t-1}=1
$$

$$
x=1-\frac{3}{t-1}
$$

Simplify:

$$
x=\frac{t-4}{t-1}
$$

Therefore, the unique solution is:

$$
x=\frac{t-4}{t-1}
$$

$$
y=\frac{1}{t-1}
$$

$$
z=\frac{2}{t-1}
$$

where t is any real number except 1.

### Step 5 – Check the Solution

We substitute the calculated values into all three original equations.

**First equation:**

$$
x+y+z=1
$$

$$
\frac{t-4}{t-1}+\frac{1}{t-1}+\frac{2}{t-1}=1
$$

$$
\frac{t-1}{t-1}=1
$$

**Second equation:**

$$
x+ty+z=2
$$

$$
\frac{t-4}{t-1}+\frac{t}{t-1}+\frac{2}{t-1}=2
$$

$$
\frac{2t-2}{t-1}=2
$$

**Third equation:**

$$
x+y+tz=3
$$

$$
\frac{t-4}{t-1}+\frac{1}{t-1}+\frac{2t}{t-1}=3
$$

$$
\frac{3t-3}{t-1}=3
$$

All three equations are satisfied when t is not equal to 1.

### Step 6 – Case 2: t = 1

Now substitute t = 1 into the reduced augmented matrix.

$$
\left[
\begin{array}{ccc|c}
1&1&1&1\\
0&0&0&1\\
0&0&0&2
\end{array}
\right]
$$

The second row represents:

$$
0=1
$$

The third row represents:

$$
0=2
$$

Both statements are impossible.

Therefore, the system has no solution when t = 1.

### Step 7 – Final Classification

There are two possible cases:

**If t is not equal to 1:**

The system has exactly one solution:

$$
x=\frac{t-4}{t-1}
$$

$$
y=\frac{1}{t-1}
$$

$$
z=\frac{2}{t-1}
$$

**If t = 1:**

The system has no solution because elimination produces contradictions.

**Infinitely many solutions:**

This case never occurs.

### Explanation

During Gaussian elimination, we obtain the expressions (t-1)y=1 and (t-1)z=2.

Dividing by t-1 is valid only when t is not equal to 1.

When t equals 1, the resulting equations become 0=1 and 0=2, which are contradictions.

Therefore, the system has one unique solution for every real value of t except 1, and no solution when t equals 1.

### Conclusion

The number of solutions depends on the parameter:

- t ≠ 1: Exactly one solution.
- t = 1: No solution.
- Infinitely many solutions: Never occurs.
