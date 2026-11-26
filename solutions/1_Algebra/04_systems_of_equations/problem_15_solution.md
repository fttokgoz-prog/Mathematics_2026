
# EXERCISE 15 – CLASSIFYING THREE SYSTEMS

## Given

For each of the following systems, perform only as much elimination as necessary to recognize its type.

### System 1

$$
\begin{cases}
x+y=2\\
x-y=0
\end{cases}
$$

### System 2

$$
\begin{cases}
x+y=2\\
2x+2y=4
\end{cases}
$$

### System 3

$$
\begin{cases}
x+y=2\\
2x+2y=5
\end{cases}
$$

For each, justify the classification: one solution, infinitely many solutions, or no solution.

## Solution

### Step 1 – Analyze System 1

The first system is:

$$
\begin{cases}
x+y=2\\
x-y=0
\end{cases}
$$

Write the augmented matrix:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
1&-1&0
\end{array}
\right]
$$

Apply the row operation:

$$
R_2\rightarrow R_2-R_1
$$

The new matrix becomes:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
0&-2&-2
\end{array}
\right]
$$

There is a pivot in both variable columns.

Therefore, both variables have leading positions and there are no free variables.

The system has exactly one solution.

**Classification: One solution.**

### Step 2 – Analyze System 2

The second system is:

$$
\begin{cases}
x+y=2\\
2x+2y=4
\end{cases}
$$

Write the augmented matrix:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
2&2&4
\end{array}
\right]
$$

Apply the row operation:

$$
R_2\rightarrow R_2-2R_1
$$

The new matrix becomes:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
0&0&0
\end{array}
\right]
$$

The second row represents:

$$
0=0
$$

This is always true and does not create a contradiction.

There is one free variable because the second variable column has no pivot.

Therefore, the system has infinitely many solutions.

**Classification: Infinitely many solutions.**

### Step 3 – Analyze System 3

The third system is:

$$
\begin{cases}
x+y=2\\
2x+2y=5
\end{cases}
$$

Write the augmented matrix:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
2&2&5
\end{array}
\right]
$$

Apply the row operation:

$$
R_2\rightarrow R_2-2R_1
$$

The new matrix becomes:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
0&0&1
\end{array}
\right]
$$

The second row represents:

$$
0x+0y=1
$$

Simplifying:

$$
0=1
$$

This is a contradiction.

Therefore, the system is inconsistent and has no solution.

**Classification: No solution.**

### Step 4 – Compare the Three Systems

The three systems can be classified by examining their final augmented matrices.

| System | Final Row | Classification |
|---|---|---|
| System 1 | Two pivot positions | One solution |
| System 2 | 0 = 0 | Infinitely many solutions |
| System 3 | 0 = 1 | No solution |

### Final Answer

**System 1:**

Exactly one solution because both variable columns contain pivots.

**System 2:**

Infinitely many solutions because one variable is free and there is no contradiction.

**System 3:**

No solution because elimination produces the contradiction 0 = 1.

### Conclusion

Gaussian elimination allows us to classify a system without necessarily solving it completely.

- A pivot in every variable column indicates a unique solution.
- A consistent system with at least one free variable has infinitely many solutions.
- A row representing 0 = a nonzero number indicates no solution.

The three systems demonstrate all three basic possibilities for a linear system.
