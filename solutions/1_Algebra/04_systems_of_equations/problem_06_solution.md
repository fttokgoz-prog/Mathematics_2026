
# EXERCISE 6 – A SYSTEM WITH A PARAMETER: WHICH CASES ACTUALLY OCCUR?

## Given

Analyze the following system depending on the real parameter alpha:

$$
\begin{cases}
x+y=2\\
\alpha x+\alpha y=4
\end{cases}
$$

Among the three possibilities — exactly one solution, infinitely many solutions, or no solution — determine which actually occur and for which values of alpha. If one type cannot occur, explain why.

## Solution

### Step 1 – Write the Augmented Matrix

The system can be written as the following augmented matrix:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
\alpha&\alpha&4
\end{array}
\right]
$$

### Step 2 – Apply Gaussian Elimination

Apply the row operation:

$$
R_2 \rightarrow R_2-\alpha R_1
$$

The new matrix becomes:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
0&0&4-2\alpha
\end{array}
\right]
$$

The second row represents:

$$
0x+0y=4-2\alpha
$$

Therefore:

$$
0=4-2\alpha
$$

### Step 3 – Analyze the Cases

We consider the possible values of alpha.

**Case 1: alpha = 2**

Substitute alpha = 2 into the system:

$$
\begin{cases}
x+y=2\\
2x+2y=4
\end{cases}
$$

The second equation is exactly twice the first equation.

The reduced augmented matrix becomes:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
0&0&0
\end{array}
\right]
$$

The second row represents 0 = 0, which is always true.

There is one free variable.

Let:

$$
y=t,\quad t\in\mathbb{R}
$$

From the first equation:

$$
x=2-t
$$

Therefore, the solutions are:

$$
x=2-t
$$

$$
y=t
$$

where t can be any real number.

The system has infinitely many solutions.

**Case 2: alpha is not equal to 2**

If alpha is not equal to 2, then:

$$
4-2\alpha\neq 0
$$

The second row represents:

$$
0=4-2\alpha
$$

This is a contradiction because the left side is zero and the right side is nonzero.

Therefore, the system has no solution.

### Step 4 – Check Whether Exactly One Solution Can Occur

For exactly one solution, both variables must have pivot positions.

However, the coefficient matrix is:

$$
\begin{pmatrix}
1&1\\
\alpha&\alpha
\end{pmatrix}
$$

The second row is always a multiple of the first row.

Therefore, the coefficient matrix never has two independent rows.

Its determinant is:

$$
\det(A)=1(\alpha)-1(\alpha)=0
$$

Since the determinant is always zero, the system cannot have exactly one solution for any value of alpha.

### Step 5 – Final Classification

The possible cases are:

- If alpha = 2, the system has infinitely many solutions.
- If alpha is not equal to 2, the system has no solution.
- Exactly one solution never occurs.

### Final Answer

**Infinitely many solutions:**

$$
\alpha=2
$$

The solutions are:

$$
x=2-t,\quad y=t,\quad t\in\mathbb{R}
$$

**No solution:**

$$
\alpha\neq 2
$$

**Exactly one solution:**

There is no value of alpha for which the system has exactly one solution.

### Explanation

The two equations always have proportional coefficient rows because the coefficients of x and y in the second equation are both multiplied by alpha.

When alpha equals 2, the second equation becomes twice the first equation, so both equations describe the same line and there are infinitely many solutions.

When alpha is different from 2, the equations contradict each other because they have the same left-hand side relationship but different required constants.

A unique solution is impossible because the coefficient matrix always has determinant zero and cannot have two independent rows.
