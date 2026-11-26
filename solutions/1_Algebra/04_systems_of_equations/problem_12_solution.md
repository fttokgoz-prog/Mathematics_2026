
# EXERCISE 12 – HOMOGENEOUS SYSTEM

## Given

Solve the following homogeneous system:

$$
\begin{cases}
x+2y-z=0\\
2x+4y-2z=0\\
x-y+2z=0
\end{cases}
$$

Give all solutions in parametric form and explain why (0,0,0) always satisfies a homogeneous system.

## Solution

### Step 1 – Write the Augmented Matrix

$$
\left[
\begin{array}{ccc|c}
1&2&-1&0\\
2&4&-2&0\\
1&-1&2&0
\end{array}
\right]
$$

### Step 2 – Eliminate the First Column

Apply the following row operations:

$$
R_2\rightarrow R_2-2R_1
$$

$$
R_3\rightarrow R_3-R_1
$$

The new matrix becomes:

$$
\left[
\begin{array}{ccc|c}
1&2&-1&0\\
0&0&0&0\\
0&-3&3&0
\end{array}
\right]
$$

### Step 3 – Swap the Second and Third Rows

Apply:

$$
R_2\leftrightarrow R_3
$$

The matrix becomes:

$$
\left[
\begin{array}{ccc|c}
1&2&-1&0\\
0&-3&3&0\\
0&0&0&0
\end{array}
\right]
$$

### Step 4 – Make the Second Pivot Equal to 1

Apply:

$$
R_2\rightarrow-\frac{1}{3}R_2
$$

The new matrix is:

$$
\left[
\begin{array}{ccc|c}
1&2&-1&0\\
0&1&-1&0\\
0&0&0&0
\end{array}
\right]
$$

### Step 5 – Eliminate the Second Entry in the First Row

Apply:

$$
R_1\rightarrow R_1-2R_2
$$

The final matrix becomes:

$$
\left[
\begin{array}{ccc|c}
1&0&1&0\\
0&1&-1&0\\
0&0&0&0
\end{array}
\right]
$$

### Step 6 – Write the Equations

The final matrix represents:

$$
x+z=0
$$

$$
y-z=0
$$

Therefore:

$$
x=-z
$$

$$
y=z
$$

### Step 7 – Identify the Free Variable

There is no pivot in the third column.

Therefore, z is a free variable.

Let:

$$
z=t,\quad t\in\mathbb{R}
$$

Then:

$$
x=-t
$$

$$
y=t
$$

$$
z=t
$$

The complete parametric solution is:

$$
(x,y,z)=(-t,t,t)
$$

where t can be any real number.

### Step 8 – Check the Parametric Solution

Substitute x=-t, y=t, and z=t into the original equations.

**First equation:**

$$
-t+2t-t=0
$$

$$
0=0
$$

**Second equation:**

$$
2(-t)+4t-2t=0
$$

$$
0=0
$$

**Third equation:**

$$
-t-t+2t=0
$$

$$
0=0
$$

All three equations are satisfied for every real value of t.

### Step 9 – Explain the Zero Solution

A homogeneous system has the form:

$$
Ax=0
$$

The right-hand side is always the zero vector.

If all unknown variables are set to zero, every equation becomes:

$$
0=0
$$

Therefore:

$$
(x,y,z)=(0,0,0)
$$

always satisfies a homogeneous system.

In our parametric solution, choosing t=0 gives:

$$
x=0,\quad y=0,\quad z=0
$$

This confirms that the zero solution is included.

### Final Answer

The complete solution is:

$$
x=-t
$$

$$
y=t
$$

$$
z=t
$$

where:

$$
t\in\mathbb{R}
$$

The system has infinitely many solutions because it contains one free variable.

### Conclusion

The given system is homogeneous because all right-hand side values are zero.

It has one free variable and infinitely many solutions.

The zero vector (0,0,0) is always a solution because substituting zero into a homogeneous system makes every equation equal to zero.
