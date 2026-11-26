
# EXERCISE 5 – ROW ECHELON FORM AND NUMBER OF SOLUTIONS

## Given

For the augmented matrix:

$$
\left[
\begin{array}{ccc|c}
1&2&-1&3\\
0&1&2&1\\
0&0&0&0
\end{array}
\right]
$$

Determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

## Solution

### Step 1 – Identify the Pivot Columns

The given matrix is already in row echelon form.

The first pivot is in column 1, and the second pivot is in column 2.

There is no pivot in column 3.

Therefore:

- x is a pivot variable.
- y is a pivot variable.
- z is a free variable.

### Step 2 – Write the Equations

The matrix represents the following equations:

$$
x+2y-z=3
$$

$$
y+2z=1
$$

The third row represents:

$$
0=0
$$

This equation does not create a contradiction or an additional restriction.

### Step 3 – Choose the Free Variable

Since column 3 has no pivot, z can be chosen freely.

Let:

$$
z=t,\qquad t\in\mathbb{R}
$$

From the second equation:

$$
y+2z=1
$$

Substitute z = t:

$$
y+2t=1
$$

Therefore:

$$
y=1-2t
$$

### Step 4 – Calculate x

Using the first equation:

$$
x+2y-z=3
$$

Substitute y = 1 - 2t and z = t:

$$
x+2(1-2t)-t=3
$$

Simplify:

$$
x+2-4t-t=3
$$

$$
x-5t=1
$$

Therefore:

$$
x=1+5t
$$

### Step 5 – Write the Parametric Solution

The solution is:

$$
\boxed{
\begin{aligned}
x&=1+5t\\
y&=1-2t\\
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
5\\-2\\1
\end{pmatrix},
\quad t\in\mathbb{R}
}
$$

### Step 6 – Determine the Number of Solutions

There are two pivot columns and one non-pivot column.

The non-pivot column corresponds to one free variable, z.

The zero row represents 0 = 0, so the system is consistent.

Since the free variable can take any real value, the system has infinitely many solutions.

### Explanation

In row echelon form, each pivot column corresponds to a leading variable, while each non-pivot column corresponds to a free variable.

The number of free variables is equal to the number of columns without pivots.

Here, there are three variables and two pivot columns, so there is one free variable.

Because the system is consistent and has one free variable, it has infinitely many solutions.

### Final Answer

$$
\boxed{
(x,y,z)=(1+5t,\ 1-2t,\ t),
\quad t\in\mathbb{R}
}
$$

The system has infinitely many solutions because it contains one free variable and no contradictory row.
