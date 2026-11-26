
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

The augmented matrix represents the following equations:

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

Since the third column has no pivot, z can be chosen freely.

Let:

$$
z=t,\quad t\in\mathbb{R}
$$

From the second equation:

$$
y+2z=1
$$

Substitute z=t:

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

Substitute y=1-2t and z=t:

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

The parametric solution is:

$$
x=1+5t
$$

$$
y=1-2t
$$

$$
z=t
$$

where t can be any real number.

In ordered triple form:

$$
(x,y,z)=(1+5t,1-2t,t)
$$

### Step 6 – Determine the Number of Solutions

There are three variables and two pivot columns.

Therefore, there is one free variable.

The third row represents 0=0, so the system is consistent.

Since the free variable can take any real value, the system has infinitely many solutions.

### Explanation

In row echelon form, pivot columns correspond to leading variables, while columns without pivots correspond to free variables.

The number of free variables is equal to the number of non-pivot columns.

In this matrix, there are two pivot columns and one non-pivot column. Therefore, z is the only free variable.

Since there is no contradictory row, the system is consistent and has infinitely many solutions.

### Final Answer

The system has infinitely many solutions:

$$
x=1+5t
$$

$$
y=1-2t
$$

$$
z=t
$$

where:

$$
t\in\mathbb{R}
$$
