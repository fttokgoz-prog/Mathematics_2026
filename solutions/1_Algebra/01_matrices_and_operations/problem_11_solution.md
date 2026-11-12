
# EXERCISE 11
# WHEN DO MATRICES COMMUTE?

---

## 1. GIVEN

We are given two matrices:

```math
A =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

```math
B =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
```

Find the conditions on $a$, $b$, $c$, and $d$ under which $AB=BA$.

Describe the general form of all matrices $B$ satisfying this condition.

---

## 2. SOLUTION

### STEP 1 - Calculate AB

Multiply matrix A by matrix B:

```math
AB =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
```

Multiply the corresponding rows and columns:

```math
AB =
\begin{pmatrix}
a+c & b+d \\
c & d
\end{pmatrix}
```

### STEP 2 - Calculate BA

Now multiply matrix B by matrix A:

```math
BA =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

The result is:

```math
BA =
\begin{pmatrix}
a & a+b \\
c & c+d
\end{pmatrix}
```

### STEP 3 - Apply the Condition AB = BA

For the matrices to commute, their corresponding entries must be equal.

Therefore:

```math
\begin{pmatrix}
a+c & b+d \\
c & d
\end{pmatrix}
=
\begin{pmatrix}
a & a+b \\
c & c+d
\end{pmatrix}
```

Comparing the corresponding entries gives the following equations:

First entry:

```math
a+c=a
```

Therefore:

```math
\boxed{c=0}
```

Second entry:

```math
b+d=a+b
```

Subtracting $b$ from both sides:

```math
\boxed{d=a}
```

Third entry:

```math
c=c
```

This equation is always true.

Fourth entry:

```math
d=c+d
```

Therefore:

```math
c=0
```

This confirms the first condition.

### STEP 4 - Determine the Conditions

The two required conditions are:

```math
\boxed{c=0,\qquad d=a}
```

There are no restrictions on $a$ and $b$.

Both can be any real numbers.

---

## 3. GENERAL FORM OF MATRIX B

Substituting the conditions $c=0$ and $d=a$ into the original matrix:

```math
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
```

Therefore, the general form of all matrices B that commute with A is:

```math
\boxed{
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
}
```

where $a,b\in\mathbb{R}$.

---

## 4. VERIFICATION

We can verify that these conditions make $AB=BA$.

Using the general form:

```math
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
```

Calculate AB:

```math
AB =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
```

```math
AB =
\begin{pmatrix}
a & a+b \\
0 & a
\end{pmatrix}
```

Now calculate BA:

```math
BA =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

```math
BA =
\begin{pmatrix}
a & a+b \\
0 & a
\end{pmatrix}
```

Both products are identical.

Therefore:

```math
\boxed{AB=BA}
```

---

## 5. CONCLUSION

Two matrices do not always commute, meaning that their multiplication order usually matters.

In this exercise, we found the exact conditions under which $AB=BA$.

These conditions are:

- $c=0$
- $d=a$

The general form of matrix B is:

```math
\boxed{
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
}
```

where $a$ and $b$ can be any real numbers.

This demonstrates that matrix multiplication is not generally commutative, but certain matrices satisfy the commutative property.
