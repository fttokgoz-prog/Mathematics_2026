# EXERCISE 11
# WHEN DO MATRICES COMMUTE?

---

## 1. GIVEN

The following matrices are given:

Matrix A:

$$
A =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Matrix B:

$$
B =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

## 2. QUESTION

Find the conditions on \(a, b, c, d\) under which:

$$
AB = BA
$$

Describe the general form of all such matrices B.

---

## 3. SOLUTION

### STEP 1 – Calculate AB

Multiply matrix A by matrix B:

$$
AB =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
$$

$$
AB =
\begin{pmatrix}
a+c & b+d \\
c & d
\end{pmatrix}
$$

### STEP 2 – Calculate BA

Now multiply matrix B by matrix A:

$$
BA =
\begin{pmatrix}
a & b \\
c & d
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

$$
BA =
\begin{pmatrix}
a & a+b \\
c & c+d
\end{pmatrix}
$$

### STEP 3 – Compare AB and BA

For the matrices to commute, their corresponding entries must be equal.

Therefore:

$$
\begin{aligned}
a+c &= a \\
b+d &= a+b \\
c &= c \\
d &= c+d
\end{aligned}
$$

Simplifying these equations:

From the first equation:

$$
c=0
$$

From the second equation:

$$
d=a
$$

The remaining equations give the same condition or are automatically satisfied.

Therefore, the required conditions are:

$$
\boxed{c=0,\quad d=a}
$$

---

## 4. GENERAL FORM OF MATRIX B

Substitute the conditions \(c=0\) and \(d=a\) into matrix B:

$$
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
$$

Here, \(a\) and \(b\) can be any real numbers.

This is the general form of all matrices B that commute with A.

---

## 5. FINAL ANSWER

The matrices A and B commute when:

$$
\boxed{c=0,\quad d=a}
$$

The general form of matrix B is:

$$
\boxed{
B =
\begin{pmatrix}
a & b \\
0 & a
\end{pmatrix}
}
$$

where \(a,b \in \mathbb{R}\).

---

## 6. CONCLUSION

Two matrices commute when multiplying them in either order gives the same result.

In this exercise, the condition \(AB=BA\) requires the lower-left entry of B to be zero and both diagonal entries to be equal.

Therefore, not every matrix B commutes with A. Only matrices with the form shown above satisfy this condition.
