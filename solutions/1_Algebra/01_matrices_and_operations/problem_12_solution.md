
# EXERCISE 12
# FORMULA FOR A MATRIX POWER

---

## 1. GIVEN

We are given the following matrix:

$$
A=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Compute $A^2$, $A^3$, and $A^4$.

Use the results to formulate a conjecture for $A^n$.

Then prove the formula using mathematical induction:

1. Verify the formula for the initial case.
2. Assume the formula is true for an arbitrary positive integer $n$.
3. Multiply both sides by A.
4. Show that the resulting expression is exactly the formula for $n+1$.

---

## 2. CALCULATE A²

By definition:

$$
A^2=A\cdot A
$$

Substitute the matrix:

$$
A^2=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Multiply the rows and columns:

$$
A^2=
\begin{pmatrix}
1\cdot1+1\cdot0 & 1\cdot1+1\cdot1 \\
0\cdot1+1\cdot0 & 0\cdot1+1\cdot1
\end{pmatrix}
$$

Therefore:

$$
A^2=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
$$

---

## 3. CALCULATE A³

We use the previous result:

$$
A^3=A^2\cdot A
$$

Substitute the matrices:

$$
A^3=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Multiply the matrices:

$$
A^3=
\begin{pmatrix}
1\cdot1+2\cdot0 & 1\cdot1+2\cdot1 \\
0\cdot1+1\cdot0 & 0\cdot1+1\cdot1
\end{pmatrix}
$$

Therefore:

$$
A^3=
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
$$

---

## 4. CALCULATE A⁴

Again, use the previous result:

$$
A^4=A^3\cdot A
$$

Substitute the matrices:

$$
A^4=
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

Multiply the matrices:

$$
A^4=
\begin{pmatrix}
1\cdot1+3\cdot0 & 1\cdot1+3\cdot1 \\
0\cdot1+1\cdot0 & 0\cdot1+1\cdot1
\end{pmatrix}
$$

Therefore:

$$
A^4=
\begin{pmatrix}
1 & 4 \\
0 & 1
\end{pmatrix}
$$

---

## 5. OBSERVE THE PATTERN

We have calculated:

$$
A^1=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

$$
A^2=
\begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
$$

$$
A^3=
\begin{pmatrix}
1 & 3 \\
0 & 1
\end{pmatrix}
$$

$$
A^4=
\begin{pmatrix}
1 & 4 \\
0 & 1
\end{pmatrix}
$$

We observe that:

- The top-left entry is always 1.
- The bottom-left entry is always 0.
- The bottom-right entry is always 1.
- The top-right entry increases by 1 with each multiplication.

This suggests the following general formula:

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
$$

We will now prove this formula using mathematical induction.

---

## 6. PROOF BY MATHEMATICAL INDUCTION

### Step 1 - Base Case

For $n=1$, the formula gives:

$$
A^1=
\begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
$$

This is exactly the original matrix A.

Therefore, the formula is true for $n=1$.

### Step 2 - Induction Hypothesis

Assume that the formula is true for some positive integer $n$.

Thus, we assume:

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
$$

This is our induction hypothesis.

### Step 3 - Prove the Formula for n+1

We need to show that:

$$
A^{n+1}=
\begin{pmatrix}
1 & n+1 \\
0 & 1
\end{pmatrix}
$$

Using the definition of matrix powers:

$$
A^{n+1}=A^n\cdot A
$$

Substitute the induction hypothesis:

$$
A^{n+1}=
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
A^{n+1}=
\begin{pmatrix}
1\cdot1+n\cdot0 & 1\cdot1+n\cdot1 \\
0\cdot1+1\cdot0 & 0\cdot1+1\cdot1
\end{pmatrix}
$$

Simplify each entry:

$$
A^{n+1}=
\begin{pmatrix}
1 & 1+n \\
0 & 1
\end{pmatrix}
$$

Since $1+n=n+1$, we obtain:

$$
A^{n+1}=
\begin{pmatrix}
1 & n+1 \\
0 & 1
\end{pmatrix}
$$

This is exactly the required formula.

Therefore, the induction step is complete.

---

## 7. FINAL FORMULA

By mathematical induction, the formula holds for every positive integer $n$:

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
$$

---

## 8. CONCLUSION

We calculated the first four powers of matrix A and identified a clear pattern.

The top-right entry increases by one with each multiplication, while the other three entries remain unchanged.

We then used mathematical induction to prove that the pattern continues for every positive integer n.

The final result is:

$$
A^n=
\begin{pmatrix}
1 & n \\
0 & 1
\end{pmatrix}
$$

This exercise demonstrates how repeated matrix multiplication can reveal a general formula and how mathematical induction can be used to prove that formula for all positive integers.
