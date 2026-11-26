
# EXERCISE 2 – GAUSSIAN ELIMINATION: ONE SOLUTION

## Given

Solve the following system using Gaussian elimination:

$$
\begin{cases}
x+y+z=6\\
2x-y+z=3\\
x+2y-z=2
\end{cases}
$$

After solving, substitute the result into all equations and check consistency.

## Solution

### Step 1 – Write the Augmented Matrix

$$
\left[
\begin{array}{ccc|c}
1&1&1&6\\
2&-1&1&3\\
1&2&-1&2
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
\begin{array}{ccc|c}
1&1&1&6\\
0&-3&-1&-9\\
1&2&-1&2
\end{array}
\right]
$$

Now apply:

$$
R_3\rightarrow R_3-R_1
$$

The new matrix is:

$$
\left[
\begin{array}{ccc|c}
1&1&1&6\\
0&-3&-1&-9\\
0&1&-2&-4
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
1&1&1&6\\
0&1&-2&-4\\
0&-3&-1&-9
\end{array}
\right]
$$

### Step 4 – Eliminate the Second Column

Apply:

$$
R_3\rightarrow R_3+3R_2
$$

The new matrix is:

$$
\left[
\begin{array}{ccc|c}
1&1&1&6\\
0&1&-2&-4\\
0&0&-7&-21
\end{array}
\right]
$$

The matrix is now in row echelon form.

### Step 5 – Back Substitution

From the third row:

$$
-7z=-21
$$

$$
z=3
$$

From the second row:

$$
y-2z=-4
$$

Substitute z = 3:

$$
y-2(3)=-4
$$

$$
y=2
$$

From the first row:

$$
x+y+z=6
$$

Substitute y = 2 and z = 3:

$$
x+2+3=6
$$

$$
x=1
$$

### Step 6 – Final Solution

$$
\boxed{
x=1,\quad y=2,\quad z=3
}
$$

### Step 7 – Check the Result

Substitute the solution into all original equations.

**First equation:**

$$
x+y+z=6
$$

$$
1+2+3=6
$$

$$
6=6
$$

**Second equation:**

$$
2x-y+z=3
$$

$$
2(1)-2+3=3
$$

$$
3=3
$$

**Third equation:**

$$
x+2y-z=2
$$

$$
1+2(2)-3=2
$$

$$
2=2
$$

### Conclusion

All three original equations are satisfied by the solution.

Therefore, the system is consistent and has exactly one solution:

$$
\boxed{
(x,y,z)=(1,2,3)
}
$$
