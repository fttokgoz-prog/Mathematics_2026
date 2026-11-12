
# EXERCISE 2
# DETERMINANT OF A 3×3 MATRIX

---

## 1. GIVEN

We are given the following matrix:

```math
A =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
2 & 1 & 5
\end{pmatrix}
```

We need to calculate det(A) using Sarrus' rule and check the result using a determinant property.

---

## 2. SARRUS' RULE

For a 3×3 matrix, Sarrus' rule calculates the determinant by adding the three downward diagonal products and subtracting the three upward diagonal products.

The general formula is:

```math
\det(A)=aei+bfg+cdh-ceg-bdi-afh
```

---

## 3. CALCULATE THE POSITIVE DIAGONALS

Using our matrix:

First downward diagonal:

```math
1 \cdot 3 \cdot 5=15
```

Second downward diagonal:

```math
2 \cdot 4 \cdot 2=16
```

Third downward diagonal:

```math
(-1)\cdot 0\cdot 1=0
```

The positive sum is:

```math
15+16+0=31
```

---

## 4. CALCULATE THE NEGATIVE DIAGONALS

First upward diagonal:

```math
(-1)\cdot 3\cdot 2=-6
```

Second upward diagonal:

```math
2\cdot 0\cdot 5=0
```

Third upward diagonal:

```math
1\cdot 4\cdot 1=4
```

The negative sum is:

```math
-6+0+4=-2
```

---

## 5. FINAL DETERMINANT CALCULATION

Subtract the sum of the upward diagonals from the sum of the downward diagonals:

```math
\det(A)=31-(-2)
```

Therefore:

```math
\boxed{\det(A)=33}
```

---

## 6. CHECK USING A DETERMINANT PROPERTY

We can check our answer using the row operation property.

Adding a multiple of one row to another row does not change the determinant.

Apply the following operation:

```math
R_3 \leftarrow R_3-2R_1
```

The new matrix becomes:

```math
A' =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 4 \\
0 & -3 & 7
\end{pmatrix}
```

Since this row operation does not change the determinant:

```math
\det(A')=\det(A)
```

Now expand along the first column:

```math
\det(A')=
1\cdot
\begin{vmatrix}
3 & 4 \\
-3 & 7
\end{vmatrix}
```

Calculate the 2×2 determinant:

```math
\det(A')=1\cdot(3\cdot7-4\cdot(-3))
```

```math
\det(A')=21+12
```

Therefore:

```math
\boxed{\det(A')=33}
```

Both methods give the same result.

---

## 7. CONCLUSION

Using Sarrus' rule, we calculated the determinant of the given matrix.

We obtained:

```math
\boxed{\det(A)=33}
```

We also checked the result using the row operation property of determinants.

The second calculation gives the same answer, confirming that our result is correct.
