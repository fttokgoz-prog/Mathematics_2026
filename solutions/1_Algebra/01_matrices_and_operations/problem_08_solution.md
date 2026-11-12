# EXERCISE 8
# ROW OPERATIONS AND THEIR REVERSIBILITY

---

## 1. GIVEN

The initial matrix is:

$$
A =
\begin{pmatrix}
1 & 2 & -1 \\
2 & 4 & 1 \\
-1 & 1 & 3
\end{pmatrix}
$$

We must perform the following operations in order:

1. \(R_2 \leftarrow R_2 - 2R_1\)
2. \(R_3 \leftarrow R_3 + R_1\)
3. Interchange \(R_2\) and \(R_3\).

---

## 2. SOLUTION

### STEP 1 – First Row Operation

Operation:

$$
R_2 \leftarrow R_2 - 2R_1
$$

Calculate the new second row:

$$
(2,4,1)-2(1,2,-1)
$$

$$
=(2,4,1)-(2,4,-2)
$$

$$
=(0,0,3)
$$

The resulting matrix is:

$$
A_1 =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
-1 & 1 & 3
\end{pmatrix}
$$

**Inverse operation:**

$$
R_2 \leftarrow R_2 + 2R_1
$$

This restores the original second row.

---

### STEP 2 – Second Row Operation

Operation:

$$
R_3 \leftarrow R_3 + R_1
$$

Calculate the new third row:

$$
(-1,1,3)+(1,2,-1)
$$

$$
=(0,3,2)
$$

The resulting matrix is:

$$
A_2 =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2
\end{pmatrix}
$$

**Inverse operation:**

$$
R_3 \leftarrow R_3 - R_1
$$

This restores the original third row before Step 2.

---

### STEP 3 – Interchange the Second and Third Rows

Operation:

$$
R_2 \leftrightarrow R_3
$$

We exchange the second and third rows of matrix \(A_2\).

Before the operation:

$$
A_2 =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 0 & 3 \\
0 & 3 & 2
\end{pmatrix}
$$

After exchanging the rows:

$$
A_3 =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}
$$

**Inverse operation:**

$$
R_2 \leftrightarrow R_3
$$

Exchanging the same two rows again restores the previous matrix.

---

## 3. FINAL SUMMARY

| Step | Operation | Inverse Operation |
|---|---|---|
| 1 | \(R_2 \leftarrow R_2-2R_1\) | \(R_2 \leftarrow R_2+2R_1\) |
| 2 | \(R_3 \leftarrow R_3+R_1\) | \(R_3 \leftarrow R_3-R_1\) |
| 3 | \(R_2 \leftrightarrow R_3\) | \(R_2 \leftrightarrow R_3\) |

---

## 4. CONCLUSION

All three elementary row operations are reversible.

- Adding a multiple of one row to another row can be reversed by subtracting the same multiple.
- Interchanging two rows can be reversed by interchanging them again.

Therefore, every operation can be undone, and the original matrix can be recovered.

The final matrix is:

$$
\boxed{
A_3 =
\begin{pmatrix}
1 & 2 & -1 \\
0 & 3 & 2 \\
0 & 0 & 3
\end{pmatrix}
}
$$
