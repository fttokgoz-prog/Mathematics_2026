
# EXERCISE 12
# FORMULA FOR A MATRIX POWER

---

## 1. GIVEN

We are given the following matrix:

$$
A =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

We need to:

1. Calculate A², A³, and A⁴.
2. Find a general formula for Aⁿ.
3. Prove the formula using mathematical induction.

---

## 2. SOLUTION

### STEP 1 - Calculate A²

Multiply matrix A by itself:

$$
A^2 = A \cdot A
$$

$$
A^2 =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

After multiplication:

$$
A^2 =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
$$

---

### STEP 2 - Calculate A³

Multiply A² by A:

$$
A^3 = A^2 \cdot A
$$

$$
A^3 =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

After multiplication:

$$
A^3 =
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
$$

---

### STEP 3 - Calculate A⁴

Multiply A³ by A:

$$
A^4 = A^3 \cdot A
$$

$$
A^4 =
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

After multiplication:

$$
A^4 =
\begin{pmatrix}
1 & 4 \\
0 & 1
\end{pmatrix}
$$

---

## 3. FINDING THE PATTERN

Looking at the results, we notice:

- A² has 2 in the upper-right corner.
- A³ has 3 in the upper-right corner.
- A⁴ has 4 in the upper-right corner.

All other entries remain unchanged.

Therefore, we can guess the general formula:

$$
\boxed{
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
}
$$

for every integer n ≥ 1.

---

## 4. PROOF BY MATHEMATICAL INDUCTION

### STEP 1 - Base Case

For n = 1:

$$
A^1 =
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

This is exactly our original matrix.

Therefore, the formula is true for n = 1.

---

### STEP 2 - Induction Hypothesis

Assume that the formula is true for some integer n ≥ 1.

This means:

$$
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
$$

We now need to prove that it is also true for n + 1.

---

### STEP 3 - Induction Step

We know that:

$$
A^{n+1} = A^n \cdot A
$$

Substitute the assumed formula:

$$
A^{n+1} =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Multiply the matrices:

$$
A^{n+1} =
\begin{pmatrix}
1 \cdot 1+n \cdot 0 & 1 \cdot 1+n \cdot 1 \\
0 \cdot 1+1 \cdot 0 & 0 \cdot 1+1 \cdot 1
\end{pmatrix}
$$

Simplify:

$$
A^{n+1} =
\begin{pmatrix}
1 & 1+n \\
0 & 1
\end{pmatrix}
$$

Therefore:

$$
\boxed{
A^{n+1} =
\begin{pmatrix}
1 & n+1 \\
0 & 1
\end{pmatrix}
}
$$

This is exactly the required formula for n + 1.

The induction step is complete.

---

## 5. FINAL ANSWERS

### Matrix A²

$$
A^2 =
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
$$

### Matrix A³

$$
A^3 =
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
$$

### Matrix A⁴

$$
A^4 =
\begin{pmatrix}
1 & 4 \\
0 & 1
\end{pmatrix}
$$

### General Formula

$$
\boxed{
A^n =
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
}
$$

---

## 6. CONCLUSION

By calculating A², A³, and A⁴, we found a pattern in the upper-right entry of the matrix.

We then used mathematical induction to prove that the formula is valid for every positive integer n.

The base case is true, and assuming the formula for n allows us to prove it for n + 1.

Therefore, the general formula is proven.
