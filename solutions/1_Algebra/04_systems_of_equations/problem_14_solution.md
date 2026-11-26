
# EXERCISE 14 – A SMALL CHANGE IN THE RIGHT-HAND SIDE

## Given

Compare the following systems.

**System 1:**

$$
\begin{cases}
x+y=2\\
2x-y=1\\
3x=3
\end{cases}
$$

**System 2:**

$$
\begin{cases}
x+y=2\\
2x-y=1\\
3x=3.1
\end{cases}
$$

Check the consistency of each system and explain why a small change in one number can change the type of the system.

## Solution

### Step 1 – Write the Augmented Matrix for System 1

The first system is:

$$
\begin{cases}
x+y=2\\
2x-y=1\\
3x=3
\end{cases}
$$

Its augmented matrix is:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
2&-1&1\\
3&0&3
\end{array}
\right]
$$

### Step 2 – Apply Gaussian Elimination to System 1

First, apply:

$$
R_2\rightarrow R_2-2R_1
$$

$$
R_3\rightarrow R_3-3R_1
$$

The new matrix becomes:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
0&-3&-3\\
0&-3&-3
\end{array}
\right]
$$

Now apply:

$$
R_3\rightarrow R_3-R_2
$$

The resulting matrix is:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
0&-3&-3\\
0&0&0
\end{array}
\right]
$$

### Step 3 – Find the Solution of System 1

The second row represents:

$$
-3y=-3
$$

Therefore:

$$
y=1
$$

Using the first equation:

$$
x+y=2
$$

$$
x+1=2
$$

Therefore:

$$
x=1
$$

The solution is:

$$
x=1,\quad y=1
$$

### Step 4 – Check System 1

Substitute x=1 and y=1 into all three original equations.

First equation:

$$
1+1=2
$$

Second equation:

$$
2(1)-1=1
$$

Third equation:

$$
3(1)=3
$$

All three equations are satisfied.

Therefore, System 1 is consistent and has exactly one solution.

### Step 5 – Write the Augmented Matrix for System 2

The second system is:

$$
\begin{cases}
x+y=2\\
2x-y=1\\
3x=3.1
\end{cases}
$$

Its augmented matrix is:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
2&-1&1\\
3&0&3.1
\end{array}
\right]
$$

### Step 6 – Apply Gaussian Elimination to System 2

Apply the same row operations used in System 1:

$$
R_2\rightarrow R_2-2R_1
$$

$$
R_3\rightarrow R_3-3R_1
$$

The new matrix becomes:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
0&-3&-3\\
0&-3&-2.9
\end{array}
\right]
$$

Now apply:

$$
R_3\rightarrow R_3-R_2
$$

The resulting matrix is:

$$
\left[
\begin{array}{cc|c}
1&1&2\\
0&-3&-3\\
0&0&0.1
\end{array}
\right]
$$

### Step 7 – Analyze the Consistency of System 2

The last row represents:

$$
0x+0y=0.1
$$

Simplifying:

$$
0=0.1
$$

This is a contradiction because zero cannot equal 0.1.

Therefore, System 2 is inconsistent and has no solution.

### Step 8 – Compare the Two Systems

Both systems have the same first two equations.

The only difference is the right-hand side of the third equation:

- System 1 has 3x=3.
- System 2 has 3x=3.1.

The first two equations imply:

$$
x=1,\quad y=1
$$

Therefore:

$$
3x=3
$$

This satisfies the third equation in System 1.

However, the third equation in System 2 requires:

$$
3x=3.1
$$

This contradicts the value obtained from the first two equations.

### Final Classification

**System 1:**

The system is consistent and has exactly one solution:

$$
x=1,\quad y=1
$$

**System 2:**

The system is inconsistent and has no solution because elimination produces:

$$
0=0.1
$$

### Conclusion

A small change in the right-hand side can change the consistency of a system.

In this exercise, changing the constant from 3 to 3.1 creates a contradiction.

The first system has exactly one solution, while the second system has no solution.

This demonstrates that even a small numerical change can completely change the type of a linear system.
