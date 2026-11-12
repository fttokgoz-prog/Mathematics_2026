
# EXERCISE 4
# TRIANGULAR MATRIX

---

## 1. GIVEN

We are given the following upper triangular matrix:

```math id="a1b2c3"
A =
\begin{pmatrix}
2 & 4 & 1 \\
0 & -3 & 5 \\
0 & 0 & 7
\end{pmatrix}
```

We need to calculate the determinant without expanding it and explain the general rule for triangular matrices.

---

## 2. PROPERTY OF A TRIANGULAR MATRIX

An important property of triangular matrices is that their determinant is equal to the product of the entries on the main diagonal.

For a 3×3 upper triangular matrix:

```math id="d4e5f6"
A =
\begin{pmatrix}
a & b & c \\
0 & d & e \\
0 & 0 & f
\end{pmatrix}
```

The determinant is:

```math id="g7h8i9"
\det(A)=a\cdot d\cdot f
```

This means that we only need to multiply the diagonal entries.

---

## 3. CALCULATE THE DETERMINANT

The main diagonal entries of our matrix are:

- First diagonal entry: 2
- Second diagonal entry: -3
- Third diagonal entry: 7

Multiply these entries:

```math id="j1k2l3"
\det(A)=2\cdot(-3)\cdot7
```

First:

```math id="m4n5o6"
2\cdot(-3)=-6
```

Then:

```math id="p7q8r9"
-6\cdot7=-42
```

Therefore:

```math id="s1t2u3"
\boxed{\det(A)=-42}
```

---

## 4. GENERAL RULE FOR TRIANGULAR MATRICES

For any upper or lower triangular square matrix, the determinant is the product of all entries on its main diagonal.

For an n×n triangular matrix:

```math id="v4w5x6"
\det(A)=a_{11}\cdot a_{22}\cdot a_{33}
\cdots a_{nn}
```

This rule works because all entries either above or below the main diagonal are zero.

---

## 5. EXPLANATION USING OUR EXAMPLE

Our matrix is upper triangular because all entries below the main diagonal are zero.

The diagonal entries are 2, -3, and 7.

We do not need to expand the determinant or use Sarrus' rule.

We simply multiply the diagonal entries:

```math id="y7z8a9"
2\cdot(-3)\cdot7=-42
```

---

## 6. CONCLUSION

The determinant of a triangular matrix is always equal to the product of its main diagonal entries.

For the given matrix:

```math id="b1c2d3"
\boxed{\det(A)=-42}
```

This property allows us to calculate the determinant of triangular matrices quickly without performing a full determinant expansion.
