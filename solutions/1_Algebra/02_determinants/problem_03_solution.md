
# EXERCISE 3
# SWAPPING TWO ROWS

---

## 1. GIVEN

We are given the following matrix:

```math
A =
\begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1
\end{pmatrix}
```

We need to:

1. Calculate det(A).
2. Create matrix B by swapping the first and second rows of A.
3. Predict det(B) using a determinant property.
4. Verify the result by calculation.

---

## 2. CALCULATE THE DETERMINANT OF MATRIX A

Using Sarrus' rule:

```math
\det(A)
=
1\cdot3\cdot1
+
2\cdot1\cdot2
+
0\cdot0\cdot1
```

Subtract the upward diagonal products:

```math
-
\left(
0\cdot3\cdot2
+
2\cdot0\cdot1
+
1\cdot1\cdot1
\right)
```

Simplifying:

```math
\det(A)=3+4+0-(0+0+1)
```

Therefore:

```math
\boxed{\det(A)=6}
```

---

## 3. CREATE MATRIX B BY SWAPPING TWO ROWS

We interchange the first and second rows of matrix A.

The row operation is:

```math
R_1 \leftrightarrow R_2
```

The resulting matrix is:

```math
B =
\begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1
\end{pmatrix}
```

---

## 4. PREDICT THE NEW DETERMINANT

One important property of determinants states:

When two rows of a matrix are interchanged, the determinant changes its sign.

Therefore:

```math
\det(B)=-\det(A)
```

Since we already calculated:

```math
\det(A)=6
```

We predict:

```math
\boxed{\det(B)=-6}
```

---

## 5. VERIFY THE RESULT BY CALCULATION

Now we calculate the determinant of matrix B directly.

Using Sarrus' rule:

```math
\det(B)
=
0\cdot2\cdot1
+
3\cdot0\cdot2
+
1\cdot1\cdot1
```

Subtract the upward diagonal products:

```math
-
\left(
1\cdot2\cdot2
+
3\cdot1\cdot1
+
0\cdot0\cdot1
\right)
```

Simplifying:

```math
\det(B)=0+0+1-(4+3+0)
```

Therefore:

```math
\boxed{\det(B)=-6}
```

The calculated result matches our prediction.

---

## 6. COMPARISON OF THE RESULTS

| Matrix | Determinant |
|---|---:|
| A | 6 |
| B | -6 |

We can see that:

```math
\det(B)=-\det(A)
```

The determinant changes its sign because two rows have been interchanged.

---

## 7. CONCLUSION

We calculated the determinant of matrix A and obtained 6.

After swapping the first and second rows, we created matrix B.

The determinant of B is -6.

This confirms the determinant property that interchanging two rows changes the sign of the determinant, while its absolute value remains unchanged.
