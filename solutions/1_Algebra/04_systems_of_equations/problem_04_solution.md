
# EXERCISE 4 – INFINITELY MANY SOLUTIONS

## Given

Solve the following system:

$$
\begin{cases}
x+y+z=2\\
2x+2y+2z=4\\
x-y+z=0
\end{cases}
$$

Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point really satisfies the system.

## Solution

### Step 1 – Write the Augmented Matrix

$$
\left[
\begin{array}{ccc|c}
1&1&1&2\\
2&2&2&4\\
1&-1&1&0
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
1&1&1&2\\
0&0&0&0\\
0&-2&0&-2
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
1&1&1&2\\
0&-2&0&-2\\
0&0&0&0
\end{array}
\right]
$$

### Step 4 – Make the Second Pivot Equal to 1

Apply:

$$
R_2\rightarrow -\frac{1}{2}R_2
$$

The new matrix is:

$$
\left[
\begin{array}{ccc|c}
1&1&1&2\\
0&1&0&1\\
0&0&0&0
\end{array}
\right]
$$

### Step 5 – Eliminate the Second Entry in Row 1

Apply:

$$
R_1\rightarrow R_1-R_2
$$

The final matrix is:

$$
\left[
\begin{array}{ccc|c}
1&0&1&1\\
0&1&0&1\\
0&0&0&0
\end{array}
\right]
$$

### Step 6 – Identify the Free Variable

The matrix represents the equations:

$$
x+z=1
$$

$$
y=1
$$

There is no pivot in the third column, so z is a free variable.

Let:

$$
z=t,\qquad t\in\mathbb{R}
$$

From the first equation:

$$
x=1-z=1-t
$$

And:

$$
y=1
$$

### Step 7 – Write the Parametric Solution

Therefore, the solution is:

$$
\boxed{
\begin{aligned}
x&=1-t\\
y&=1\\
z&=t
\end{aligned}
\qquad t\in\mathbb{R}
}
$$

In vector form:

$$
\boxed{
\begin{pmatrix}
x\\y\\z
\end{pmatrix}
=
\begin{pmatrix}
1\\1\\0
\end{pmatrix}
+
t
\begin{pmatrix}
-1\\0\\1
\end{pmatrix},
\quad t\in\mathbb{R}
}
$$

### Step 8 – Check One Chosen Parameter Value

Choose:

$$
t=0
$$

Then:

$$
x=1,\qquad y=1,\qquad z=0
$$

Substitute these values into the original equations.

**First equation:**

$$
1+1+0=2
$$

**Second equation:**

$$
2(1)+2(1)+2(0)=4
$$

**Third equation:**

$$
1-1+0=0
$$

All three equations are satisfied.

### Final Answer

$$
\boxed{(x,y,z)=(1-t,1,t),\quad t\in\mathbb{R}}
$$

The system has infinitely many solutions because z is a free variable and can take any real value.
