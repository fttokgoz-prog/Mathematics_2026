
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

and

```math
B =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
```

Find the conditions on $a$, $b$, $c$, and $d$ under which:

```math
AB=BA
```

Describe the general form of all matrices $B$ satisfying this condition.

---

## 2. CALCULATE AB

First, multiply matrix A by matrix B:

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

---

## 3. CALCULATE BA

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

Multiply the corresponding rows and columns:

```math
BA =
\begin{pmatrix}
a & a+b \\
c & c+d
\end{pmatrix}
```

---

## 4. SET AB EQUAL TO BA

For the matrices to commute, we need:

```math
AB=BA
```

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

Corresponding entries must be equal.

This gives us the following equations:

**First entry:**

```math
a+c=a
```

Therefore:

```math
c=0
```

**Second entry:**

```math
b+d=a+b
```

Therefore:

```math
d=a
```

**Third entry:**

```math
c=c
```

This equation is always satisfied.

**Fourth entry:**

```math
d=c+d
```

Therefore:

```math
c=0
```

This confirms our first condition.

---

## 5. FIND THE GENERAL FORM OF B

We have obtained two conditions:

```math
c=0
```

and

```math
d=a
```

The variable $b$ is unrestricted.

Substitute these conditions into the original matrix B:

```math
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
```

Therefore, every matrix of this form commutes with A:

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

---

## 6. VERIFICATION

To verify our result, substitute the general form of B into both products.

First:

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
AB=BA
```

Our general form is correct.

---

## 7. CONCLUSION

Matrix multiplication is not generally commutative.

However, for the given matrix A, we found a specific family of matrices B that satisfies $AB=BA$.

The required conditions are:

- $c=0$
- $d=a$
- $a$ and $b$ are unrestricted real numbers.

The general form is:

```math
\boxed{
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
}
```

This exercise demonstrates that although matrix multiplication is generally noncommutative, certain matrices can commute when their entries satisfy specific algebraic conditions.

This demonstrates that matrix multiplication is not generally commutative, but certain matrices satisfy the commutative property.
