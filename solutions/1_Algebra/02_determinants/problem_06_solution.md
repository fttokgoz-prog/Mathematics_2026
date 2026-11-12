
# EXERCISE 6
# PARAMETER AND INVERTIBILITY

---

## 1. GIVEN

We are given a matrix depending on the parameter t:

```math
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t
\end{pmatrix}
```

We need to find all values of t for which the matrix is not invertible and explain the relationship with its determinant.

---

## 2. DETERMINANT FORMULA

For a 2×2 matrix:

```math
M=
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
```

The determinant is:

```math
\det(M)=ad-bc
```

A square matrix is not invertible if and only if its determinant equals zero.

---

## 3. CALCULATE THE DETERMINANT

For our matrix:

```math
A(t)=
\begin{pmatrix}
t & 1 \\
2 & t
\end{pmatrix}
```

Using the determinant formula:

```math
\det(A(t))=t\cdot t-1\cdot2
```

Simplifying:

```math
\det(A(t))=t^2-2
```

Therefore:

```math
\boxed{\det(A(t))=t^2-2}
```

---

## 4. FIND THE VALUES OF t

The matrix is not invertible when its determinant is zero.

Therefore, we solve:

```math
t^2-2=0
```

Move 2 to the other side:

```math
t^2=2
```

Take the square root of both sides:

```math
t=\pm\sqrt{2}
```

Therefore, the required values are:

```math
\boxed{t=\sqrt{2}\quad\text{or}\quad t=-\sqrt{2}}
```

---

## 5. CHECK THE RESULT

When t = √2:

```math
\det(A(\sqrt{2}))=(\sqrt{2})^2-2
```

```math
=2-2=0
```

When t = -√2:

```math
\det(A(-\sqrt{2}))=(-\sqrt{2})^2-2
```

```math
=2-2=0
```

In both cases, the determinant is zero.

Therefore, the matrix is not invertible for both values.

---

## 6. FINAL ANSWER

The determinant of the matrix is:

```math
\boxed{\det(A(t))=t^2-2}
```

The matrix is not invertible when:

```math
\boxed{t\in\{-\sqrt{2},\sqrt{2}\}}
```

For all other real values of t, the matrix is invertible.

---

## 7. CONCLUSION

The determinant determines whether a square matrix is invertible.

If the determinant is zero, the matrix has no inverse.

In this exercise, the determinant equals zero when t is either √2 or -√2.

Therefore, these are exactly the two values for which the given matrix is not invertible.
