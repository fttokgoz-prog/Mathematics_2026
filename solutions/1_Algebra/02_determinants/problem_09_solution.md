
# EXERCISE 9
# AREA AND THE DETERMINANT

---

## 1. GIVEN

We are given two vectors:

```math id="q9v1a2"
u =
\begin{pmatrix}
3 \\
1
\end{pmatrix}
```

```math id="b7c3d4"
v =
\begin{pmatrix}
1 \\
4
\end{pmatrix}
```

These vectors span a parallelogram.

We need to:

1. Calculate the area of the parallelogram using a determinant.
2. Reverse the order of the vectors.
3. Explain what changes in the determinant and what remains unchanged in the area.

---

## 2. DETERMINANT FORMULA

The area of a parallelogram formed by two vectors in two dimensions is the absolute value of the determinant of the matrix containing these vectors as columns.

The general formula is:

```math id="e5f6g7"
\text{Area}=|\det(u,v)|
```

The determinant of a 2×2 matrix is:

```math id="h8i9j1"
\det
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
=ad-bc
```

---

## 3. CALCULATE THE AREA

Place the two vectors as columns of a matrix:

```math id="k2l3m4"
A=
\begin{pmatrix}
3 & 1 \\
1 & 4
\end{pmatrix}
```

Calculate the determinant:

```math id="n5o6p7"
\det(A)=3\cdot4-1\cdot1
```

Multiply the entries:

```math id="r8s9t1"
\det(A)=12-1
```

Therefore:

```math id="u2v3w4"
\det(A)=11
```

The area is the absolute value of the determinant:

```math id="x5y6z7"
\text{Area}=|11|=11
```

The area of the parallelogram is 11 square units.

---

## 4. REVERSE THE ORDER OF THE VECTORS

Now we reverse the order of the vectors.

The new matrix is:

```math id="a8b9c1"
B=
\begin{pmatrix}
1 & 3 \\
4 & 1
\end{pmatrix}
```

Calculate its determinant:

```math id="d2e3f4"
\det(B)=1\cdot1-3\cdot4
```

Simplifying:

```math id="g5h6i7"
\det(B)=1-12
```

Therefore:

```math id="j8k9l1"
\det(B)=-11
```

---

## 5. COMPARE THE DETERMINANTS AND AREAS

The original determinant is:

```math id="m2n3o4"
\det(u,v)=11
```

After reversing the vectors:

```math id="p5q6r7"
\det(v,u)=-11
```

The determinant changes its sign because swapping the two columns of a matrix changes the sign of its determinant.

However, the area is calculated using the absolute value of the determinant.

Original area:

```math id="s8t9u1"
|11|=11
```

Reversed area:

```math id="v2w3x4"
|-11|=11
```

Therefore, the area remains unchanged.

---

## 6. FINAL RESULTS

| Calculation | Result |
|---|---:|
| Original determinant | 11 |
| Reversed determinant | -11 |
| Original area | 11 |
| Reversed area | 11 |

The determinant changes sign, but the area does not change.

---

## 7. GEOMETRICAL EXPLANATION

The two vectors form a parallelogram.

Reversing the order of the vectors changes the orientation of the parallelogram.

The determinant records this orientation through its sign:

- A positive determinant represents one orientation.
- A negative determinant represents the opposite orientation.

However, the geometric area cannot be negative.

Therefore, we always use the absolute value of the determinant when calculating area.

---

## 8. CONCLUSION

The determinant of the matrix formed by the two vectors is 11.

After reversing the vectors, the determinant becomes -11.

Although the sign changes, the area remains the same because area is always non-negative.

The final area of the parallelogram is 11 square units.

This demonstrates the geometric meaning of the determinant and its relationship with orientation and area.
