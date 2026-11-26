
# EXERCISE 10 – A POLYNOMIAL THROUGH THREE POINTS

## Given

Find a polynomial:

$$
p(x)=ax^2+bx+c
$$

whose graph passes through the points:

$$
(0,1),\quad (1,3),\quad (2,9)
$$

Reduce the problem to a system of equations and check the result by substituting all three points.

## Solution

### Step 1 – Substitute the First Point

The first point is (0,1).

Since p(0)=1, substitute x=0 into the polynomial:

$$
a(0)^2+b(0)+c=1
$$

Therefore:

$$
c=1
$$

### Step 2 – Substitute the Second Point

The second point is (1,3).

Since p(1)=3:

$$
a(1)^2+b(1)+c=3
$$

Simplify:

$$
a+b+c=3
$$

Since c=1:

$$
a+b=2
$$

### Step 3 – Substitute the Third Point

The third point is (2,9).

Since p(2)=9:

$$
a(2)^2+b(2)+c=9
$$

Simplify:

$$
4a+2b+c=9
$$

Since c=1:

$$
4a+2b=8
$$

Divide both sides by 2:

$$
2a+b=4
$$

### Step 4 – Write the System of Equations

The three equations are:

$$
\begin{cases}
c=1\\
a+b=2\\
2a+b=4
\end{cases}
$$

We can write the system in matrix form:

$$
\left[
\begin{array}{ccc|c}
0&0&1&1\\
1&1&0&2\\
2&1&0&4
\end{array}
\right]
$$

### Step 5 – Solve the System

Subtract the second equation from the third equation:

$$
(2a+b)-(a+b)=4-2
$$

Therefore:

$$
a=2
$$

Substitute a=2 into the second equation:

$$
2+b=2
$$

Therefore:

$$
b=0
$$

From the first equation:

$$
c=1
$$

The coefficients are:

$$
a=2,\quad b=0,\quad c=1
$$

### Step 6 – Find the Polynomial

Substitute the coefficients into the original polynomial:

$$
p(x)=ax^2+bx+c
$$

$$
p(x)=2x^2+0x+1
$$

Therefore:

$$
p(x)=2x^2+1
$$

### Step 7 – Check All Three Points

We substitute each x-coordinate into the polynomial and verify that the result matches the corresponding y-coordinate.

**First point: (0,1)**

$$
p(0)=2(0)^2+1
$$

$$
p(0)=1
$$

The result matches the point (0,1).

**Second point: (1,3)**

$$
p(1)=2(1)^2+1
$$

$$
p(1)=3
$$

The result matches the point (1,3).

**Third point: (2,9)**

$$
p(2)=2(2)^2+1
$$

$$
p(2)=8+1
$$

$$
p(2)=9
$$

The result matches the point (2,9).

### Final Answer

The polynomial passing through all three given points is:

$$
p(x)=2x^2+1
$$

### Conclusion

The three points produce a system of three linear equations with three unknown coefficients.

After solving the system, we obtain a=2, b=0, and c=1.

Substituting all three original points confirms that the polynomial satisfies every given condition.
