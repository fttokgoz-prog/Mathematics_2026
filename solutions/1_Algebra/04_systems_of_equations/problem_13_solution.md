
# EXERCISE 13 – DOES EVERY EQUATION ADD NEW INFORMATION?

## Given

Consider the system:

$$
\begin{cases}
x_1+x_2=10\\
x_2+x_3=8\\
x_1-x_3=2
\end{cases}
$$

Solve the system and check whether all three equations are independently necessary to describe the solution set. If one equation follows from the others, show this by calculation.

## Solution

### Step 1 – Write the Augmented Matrix

The system can be written as:

$$
\left[
\begin{array}{ccc|c}
1&1&0&10\\
0&1&1&8\\
1&0&-1&2
\end{array}
\right]
$$

### Step 2 – Apply Gaussian Elimination

Apply the row operation:

$$
R_3\rightarrow R_3-R_1
$$

The new matrix becomes:

$$
\left[
\begin{array}{ccc|c}
1&1&0&10\\
0&1&1&8\\
0&-1&-1&-8
\end{array}
\right]
$$

Now apply:

$$
R_3\rightarrow R_3+R_2
$$

The resulting matrix is:

$$
\left[
\begin{array}{ccc|c}
1&1&0&10\\
0&1&1&8\\
0&0&0&0
\end{array}
\right]
$$

### Step 3 – Write the Remaining Equations

The final matrix represents:

$$
x_1+x_2=10
$$

$$
x_2+x_3=8
$$

The third row represents:

$$
0=0
$$

This means that the third equation does not provide any additional information.

There are two independent equations and three unknown variables.

### Step 4 – Identify the Free Variable

There is no pivot in the third column.

Therefore, x3 is a free variable.

Let:

$$
x_3=t,\quad t\in\mathbb{R}
$$

From the second equation:

$$
x_2+x_3=8
$$

Substitute x3=t:

$$
x_2+t=8
$$

Therefore:

$$
x_2=8-t
$$

From the first equation:

$$
x_1+x_2=10
$$

Substitute x2=8-t:

$$
x_1+8-t=10
$$

Therefore:

$$
x_1=2+t
$$

### Step 5 – Write the Parametric Solution

The complete solution is:

$$
x_1=2+t
$$

$$
x_2=8-t
$$

$$
x_3=t
$$

where:

$$
t\in\mathbb{R}
$$

In ordered triple form:

$$
(x_1,x_2,x_3)=(2+t,8-t,t)
$$

### Step 6 – Check All Three Equations

Substitute the parametric solution into the original system.

**First equation:**

$$
x_1+x_2=10
$$

$$
(2+t)+(8-t)=10
$$

$$
10=10
$$

**Second equation:**

$$
x_2+x_3=8
$$

$$
(8-t)+t=8
$$

$$
8=8
$$

**Third equation:**

$$
x_1-x_3=2
$$

$$
(2+t)-t=2
$$

$$
2=2
$$

All three equations are satisfied for every real value of t.

### Step 7 – Check Whether All Three Equations Are Necessary

We can show that the first equation follows directly from the second and third equations.

The second equation is:

$$
x_2+x_3=8
$$

The third equation is:

$$
x_1-x_3=2
$$

Add these two equations:

$$
(x_2+x_3)+(x_1-x_3)=8+2
$$

Simplify:

$$
x_1+x_2=10
$$

This is exactly the first equation.

Therefore, the first equation is redundant because it can be obtained by adding the second and third equations.

It does not provide any new information about the solution set.

### Final Answer

The system has infinitely many solutions:

$$
x_1=2+t
$$

$$
x_2=8-t
$$

$$
x_3=t
$$

where:

$$
t\in\mathbb{R}
$$

The first equation is redundant because it follows directly from the second and third equations.

Only two independent equations are necessary to describe the solution set.

### Conclusion

Not every equation in a system necessarily provides new information.

In this example, the first equation is the sum of the second and third equations.

Gaussian elimination confirms this because the final row becomes 0=0.

Therefore, the system has two independent equations, one free variable, and infinitely many solutions.
