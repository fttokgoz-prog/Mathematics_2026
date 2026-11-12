
# EXERCISE 14
# A SYSTEM OF EQUATIONS AND THE DETERMINANT

---

## 1. GIVEN

We are given the following system of linear equations:

```math
Ax=b
```

where the coefficient matrix is:

```math
A=
\begin{pmatrix}
1 & 2 \\
k & 4
\end{pmatrix}
```

The vector of unknowns is:

```math
x=
\begin{pmatrix}
x_1 \\
x_2
\end{pmatrix}
```

The right-hand side is:

```math
b=
\begin{pmatrix}
b_1 \\
b_2
\end{pmatrix}
```

We need to determine:

1. For which values of k does the system have exactly one solution for every possible vector b?
2. For the remaining value of k, give an example of a right-hand side b that produces infinitely many solutions.
3. Give another example of a right-hand side b that produces no solution.

---

## 2. CALCULATE THE DETERMINANT

A square matrix has a unique solution for every right-hand side if and only if its determinant is non-zero.

For our matrix:

```math
A=
\begin{pmatrix}
1 & 2 \\
k & 4
\end{pmatrix}
```

The determinant of a 2×2 matrix is calculated using:

```math
\det(A)=ad-bc
```

Substitute the matrix entries:

```math
\det(A)=1\cdot4-2\cdot k
```

Simplifying:

```math
\det(A)=4-2k
```

Factor out 2:

```math
\det(A)=2(2-k)
```

---

## 3. FIND WHEN THE SYSTEM HAS A UNIQUE SOLUTION

For the system to have exactly one solution for every possible b, the determinant must not equal zero.

Therefore:

```math
\det(A)\neq0
```

Substitute the determinant:

```math
4-2k\neq0
```

Solving for k:

```math
4\neq2k
```

```math
k\neq2
```

Therefore, for every value of k except 2, the system has exactly one solution for every right-hand side vector b.

---

## 4. EXAMINE THE SPECIAL CASE k = 2

Now consider the remaining value:

```math
k=2
```

Substitute it into the coefficient matrix:

```math
A=
\begin{pmatrix}
1 & 2 \\
2 & 4
\end{pmatrix}
```

The determinant becomes:

```math
\det(A)=1\cdot4-2\cdot2
```

```math
\det(A)=4-4=0
```

The matrix is singular and is not invertible.

The system becomes:

```math
x_1+2x_2=b_1
```

```math
2x_1+4x_2=b_2
```

Notice that the second equation has a left-hand side that is exactly twice the first equation.

Therefore, the two equations are dependent.

---

## 5. EXAMPLE WITH INFINITELY MANY SOLUTIONS

Choose the following right-hand side:

```math
b=
\begin{pmatrix}
1 \\
2
\end{pmatrix}
```

The system becomes:

```math
x_1+2x_2=1
```

```math
2x_1+4x_2=2
```

The second equation is exactly twice the first equation.

Therefore, both equations represent the same line.

We can express the first variable in terms of the second:

```math
x_1=1-2x_2
```

Let:

```math
x_2=t
```

Then:

```math
x_1=1-2t
```

The general solution is:

```math
x=
\begin{pmatrix}
1-2t \\
t
\end{pmatrix}
```

where t can be any real number.

Therefore, the system has infinitely many solutions.

---

## 6. EXAMPLE WITH NO SOLUTION

Now choose a different right-hand side:

```math
b=
\begin{pmatrix}
1 \\
3
\end{pmatrix}
```

The system becomes:

```math
x_1+2x_2=1
```

```math
2x_1+4x_2=3
```

Multiply the first equation by 2:

```math
2x_1+4x_2=2
```

However, the second equation requires:

```math
2x_1+4x_2=3
```

This produces a contradiction:

```math
2=3
```

Therefore, the system has no solution.

---

## 7. SUMMARY OF THE RESULTS

| Condition | Result |
|---|---|
| k ≠ 2 | Exactly one solution for every b |
| k = 2 and b₂ = 2b₁ | Infinitely many solutions |
| k = 2 and b₂ ≠ 2b₁ | No solution |

The special case k = 2 occurs because the two rows of the coefficient matrix are linearly dependent.

---

## 8. CONCLUSION

The determinant of the coefficient matrix is:

```math
\det(A)=4-2k
```

When k is not equal to 2, the determinant is non-zero and the system has exactly one solution for every possible right-hand side vector.

When k equals 2, the determinant becomes zero and the matrix is not invertible.

Depending on the right-hand side vector, the system can have either infinitely many solutions or no solution.

Therefore, the final condition for a unique solution for every b is:

```math
k\neq2
```

This exercise demonstrates the relationship between determinants, invertibility, and the number of solutions of a linear system.
