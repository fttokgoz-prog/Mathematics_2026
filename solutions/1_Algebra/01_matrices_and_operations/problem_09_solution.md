# Exercise 9. Composing Transformations

## Question

Let

$$
S=\begin{pmatrix}
2 & 0\\
0 & 1
\end{pmatrix},
\qquad
R=\begin{pmatrix}
0 & -1\\
1 & 0
\end{pmatrix}.
$$

The matrix \(S\) describes nonuniform scaling, while \(R\) describes a \(90^\circ\) counterclockwise rotation. For

$$
x=\begin{pmatrix}
1\\
2
\end{pmatrix}
$$

compute \(RSx\) and \(SRx\). Compare the results and explain geometrically why the order of these transformations matters.

**Why this exercise:** Interprets matrix multiplication as composition of transformations.

## Solution

### Step 1: Understand the transformations

We are given three matrices or vectors:

$$
S=\begin{pmatrix}
2 & 0\\
0 & 1
\end{pmatrix},
\qquad
R=\begin{pmatrix}
0 & -1\\
1 & 0
\end{pmatrix},
\qquad
x=\begin{pmatrix}
1\\
2
\end{pmatrix}.
$$

The matrix \(S\) represents nonuniform scaling. It multiplies the horizontal coordinate by \(2\) and leaves the vertical coordinate unchanged.

For a general vector

$$
\begin{pmatrix}
a\\
b
\end{pmatrix},
$$

the scaling transformation gives

$$
S\begin{pmatrix}
a\\
b
\end{pmatrix}
=
\begin{pmatrix}
2a\\
b
\end{pmatrix}.
$$

The matrix \(R\) represents a \(90^\circ\) counterclockwise rotation. It transforms a vector according to the rule

$$
R\begin{pmatrix}
a\\
b
\end{pmatrix}
=
\begin{pmatrix}
-b\\
a
\end{pmatrix}.
$$

The original vector is

$$
x=\begin{pmatrix}
1\\
2
\end{pmatrix}.
$$

We will calculate \(RSx\) and \(SRx\) separately because the order of the transformations is different.

### Step 2: Calculate \(RSx\)

The expression \(RSx\) means

$$
RSx=R(Sx).
$$

Matrix multiplication is performed from right to left. Therefore, we first apply the scaling transformation \(S\) to \(x\), then rotate the resulting vector using \(R\).

**First, calculate \(Sx\):**

$$
Sx=
\begin{pmatrix}
2 & 0\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1\\
2
\end{pmatrix}.
$$

Calculate the first entry:

$$
2\cdot1+0\cdot2=2.
$$

Calculate the second entry:

$$
0\cdot1+1\cdot2=2.
$$

Therefore,

$$
Sx=\begin{pmatrix}
2\\
2
\end{pmatrix}.
$$

**Next, apply the rotation \(R\):**

$$
RSx=
\begin{pmatrix}
0 & -1\\
1 & 0
\end{pmatrix}
\begin{pmatrix}
2\\
2
\end{pmatrix}.
$$

Calculate the first entry:

$$
0\cdot2+(-1)\cdot2=-2.
$$

Calculate the second entry:

$$
1\cdot2+0\cdot2=2.
$$

Thus,

$$
\boxed{
RSx=\begin{pmatrix}
-2\\
2
\end{pmatrix}
}
$$

The final vector is \((-2,2)\).

### Step 3: Calculate \(SRx\)

The expression \(SRx\) means

$$
SRx=S(Rx).
$$

This time, we first rotate the original vector using \(R\), then apply the scaling transformation \(S\).

**First, calculate \(Rx\):**

$$
Rx=
\begin{pmatrix}
0 & -1\\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1\\
2
\end{pmatrix}.
$$

Calculate the first entry:

$$
0\cdot1+(-1)\cdot2=-2.
$$

Calculate the second entry:

$$
1\cdot1+0\cdot2=1.
$$

Therefore,

$$
Rx=\begin{pmatrix}
-2\\
1
\end{pmatrix}.
$$

**Next, apply the scaling transformation \(S\):**

$$
SRx=
\begin{pmatrix}
2 & 0\\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-2\\
1
\end{pmatrix}.
$$

Calculate the first entry:

$$
2\cdot(-2)+0\cdot1=-4.
$$

Calculate the second entry:

$$
0\cdot(-2)+1\cdot1=1.
$$

Thus,

$$
\boxed{
SRx=\begin{pmatrix}
-4\\
1
\end{pmatrix}
}
$$

The final vector is \((-4,1)\).

### Step 4: Compare the results

We obtained

$$
RSx=\begin{pmatrix}
-2\\
2
\end{pmatrix}
$$

and

$$
SRx=\begin{pmatrix}
-4\\
1
\end{pmatrix}.
$$

The two vectors are different:

$$
\boxed{RSx\neq SRx}
$$

The first result is \((-2,2)\), while the second result is \((-4,1)\). This demonstrates that applying the same two transformations in different orders can produce different final positions.

### Step 5: Explain geometrically why the order matters

The matrix \(S\) stretches vectors horizontally by a factor of \(2\), while leaving their vertical coordinates unchanged. The matrix \(R\) rotates vectors \(90^\circ\) counterclockwise.

**Case 1: Scale first, then rotate**

Starting with

$$
x=\begin{pmatrix}
1\\
2
\end{pmatrix},
$$

scaling gives

$$
Sx=\begin{pmatrix}
2\\
2
\end{pmatrix}.
$$

Rotating this vector gives

$$
RSx=\begin{pmatrix}
-2\\
2
\end{pmatrix}.
$$

The horizontal coordinate is doubled before the rotation takes place.

**Case 2: Rotate first, then scale**

Starting with the same vector, rotation gives

$$
Rx=\begin{pmatrix}
-2\\
1
\end{pmatrix}.
$$

Scaling this vector gives

$$
SRx=\begin{pmatrix}
-4\\
1
\end{pmatrix}.
$$

Here, the rotation moves the original horizontal coordinate into the vertical position and the original vertical coordinate into the horizontal position, with a negative sign. The subsequent horizontal scaling doubles the new horizontal coordinate from \(-2\) to \(-4\).

The final positions differ because the scaling acts along the horizontal direction, and the rotation changes how the vector is oriented relative to that direction.

Therefore, scaling and rotation do not commute in this example.

### Final Answer

Scaling followed by rotation gives

$$
\boxed{
RSx=\begin{pmatrix}
-2\\
2
\end{pmatrix}
}
$$

Rotation followed by scaling gives

$$
\boxed{
SRx=\begin{pmatrix}
-4\\
1
\end{pmatrix}
}
$$

Since

$$
\boxed{RSx\neq SRx},
$$

the order of the transformations matters. Nonuniform scaling and rotation produce different results when their order is reversed.
