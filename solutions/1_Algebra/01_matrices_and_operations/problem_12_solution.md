
# EXERCISE 12
# FORMULA FOR A MATRIX POWER

---

## 1. GIVEN

We are given the following matrix:

```math
A =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

We need to calculate A², A³ and A⁴.

Then, we must formulate a conjecture for Aⁿ and prove it using mathematical induction.

---

## 2. CALCULATE THE FIRST MATRIX POWERS

### STEP 1 - Calculate A²

By definition:

```math
A^2=A\cdot A
```

Substitute the matrix:

```math
A^2 =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

Multiply the matrices:

```math
A^2 =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
```

### STEP 2 - Calculate A³

We use the result of A²:

```math
A^3=A^2\cdot A
```

Substitute:

```math
A^3 =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

The result is:

```math
A^3 =
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
```

### STEP 3 - Calculate A⁴

We multiply A³ by A:

```math
A^4=A^3\cdot A
```

Substitute:

```math
A^4 =
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

The result is:

```math
A^4 =
\begin{pmatrix}
1 & 4 \\
0 & 1
\end{pmatrix}
```

---

## 3. OBSERVE THE PATTERN

The first four powers are:

```math
A^1 =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

```math
A^2 =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
```

```math
A^3 =
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
```

```math
A^4 =
\begin{pmatrix}
1 & 4 \\
0 & 1
\end{pmatrix}
```

We observe that:

- The diagonal entries always remain equal to 1.
- The lower-left entry always remains 0.
- The upper-right entry increases by 1 with every multiplication.

Therefore, we conjecture that the general formula is:

```math
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
```

---

## 4. MATHEMATICAL INDUCTION PROOF

We will prove that the formula is true for every positive integer n.

### STEP 1 - Base Case

For n = 1, the formula gives:

```math
A^1 =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

This is exactly the original matrix A.

Therefore, the formula is true for n = 1.

### STEP 2 - Induction Hypothesis

Assume that the formula is true for some positive integer n.

In other words, assume:

```math
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
```

We must now prove that the formula is also true for n + 1.

### STEP 3 - Induction Step

By the definition of matrix powers:

```math
A^{n+1}=A^n\cdot A
```

Using our induction hypothesis:

```math
A^{n+1} =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
```

Multiply the matrices:

```math
A^{n+1} =
\begin{pmatrix}
1\cdot1+n\cdot0 & 1\cdot1+n\cdot1 \\
0\cdot1+1\cdot0 & 0\cdot1+1\cdot1
\end{pmatrix}
```

Simplifying each entry gives:

```math
A^{n+1} =
\begin{pmatrix}
1 & n+1 \\
0 & 1
\end{pmatrix}
```

This is exactly the same formula with n replaced by n + 1.

Therefore, if the formula is true for n, it is also true for n + 1.

### STEP 4 - Induction Conclusion

We have shown that:

1. The formula is true for n = 1.
2. If it is true for n, it is also true for n + 1.

By mathematical induction, the formula is true for every positive integer n.

---

## 5. FINAL FORMULA

The general formula for the powers of matrix A is:

```math
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
```

This formula is valid for every positive integer n.

---

## 6. CONCLUSION

By calculating the first four powers, we identified a clear pattern in the matrix.

We observed that the upper-right entry increases by one with each multiplication, while the other entries remain unchanged.

Using mathematical induction, we proved that the general formula is:

```math
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
```

This exercise demonstrates how repeated matrix multiplication can produce a general formula and how mathematical induction can be used to prove it.
