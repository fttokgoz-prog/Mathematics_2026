
# EXERCISE 13
# A RECURRENCE WRITTEN IN MATRIX FORM

---

## 1. GIVEN

We are given the Fibonacci matrix:

$$
F=
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

The Fibonacci sequence is:

$$
0,\ 1,\ 1,\ 2,\ 3,\ 5,\ 8,\ 13,\ 21,\ldots
$$

Each term after the first two is obtained by adding the two previous terms.

The recurrence relation is:

$$
F_{n+2}=F_{n+1}+F_n
$$

We are asked to:

1. Compute $F^2$, $F^3$, $F^4$, and $F^5$.
2. Compare the resulting matrix entries with the Fibonacci sequence.
3. Describe the relationship between matrix powers and Fibonacci numbers.
4. Compute the product of F with a general column vector.
5. Explain how this multiplication performs one step of the Fibonacci recurrence.

---

## 2. CALCULATE F²

By definition:

$$
F^2=F\cdot F
$$

Substitute the matrix:

$$
F^2=
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

Multiply the rows and columns:

$$
F^2=
\begin{pmatrix}
1\cdot1+1\cdot1 & 1\cdot1+1\cdot0 \\
1\cdot1+0\cdot1 & 1\cdot1+0\cdot0
\end{pmatrix}
$$

Therefore:

$$
F^2=
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
$$

---

## 3. CALCULATE F³

We use the previous result:

$$
F^3=F^2\cdot F
$$

Substitute the matrices:

$$
F^3=
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

Multiply the matrices:

$$
F^3=
\begin{pmatrix}
2\cdot1+1\cdot1 & 2\cdot1+1\cdot0 \\
1\cdot1+1\cdot1 & 1\cdot1+1\cdot0
\end{pmatrix}
$$

Therefore:

$$
F^3=
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
$$

---

## 4. CALCULATE F⁴

Using the previous result:

$$
F^4=F^3\cdot F
$$

Substitute:

$$
F^4=
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

Multiply the matrices:

$$
F^4=
\begin{pmatrix}
3\cdot1+2\cdot1 & 3\cdot1+2\cdot0 \\
2\cdot1+1\cdot1 & 2\cdot1+1\cdot0
\end{pmatrix}
$$

Therefore:

$$
F^4=
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
$$

---

## 5. CALCULATE F⁵

Again, use the previous result:

$$
F^5=F^4\cdot F
$$

Substitute:

$$
F^5=
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

Multiply the matrices:

$$
F^5=
\begin{pmatrix}
5\cdot1+3\cdot1 & 5\cdot1+3\cdot0 \\
3\cdot1+2\cdot1 & 3\cdot1+2\cdot0
\end{pmatrix}
$$

Therefore:

$$
F^5=
\begin{pmatrix}
8 & 5 \\
5 & 3
\end{pmatrix}
$$

---

## 6. OBSERVE THE FIBONACCI PATTERN

We have calculated:

$$
F^1=
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

$$
F^2=
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
$$

$$
F^3=
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
$$

$$
F^4=
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
$$

$$
F^5=
\begin{pmatrix}
8 & 5 \\
5 & 3
\end{pmatrix}
$$

We can observe that the entries correspond to consecutive Fibonacci numbers.

The general pattern is:

$$
F^n=
\begin{pmatrix}
F_{n+1} & F_n \\
F_n & F_{n-1}
\end{pmatrix}
$$

for every positive integer $n$, where $F_0=0$ and $F_1=1$.

For example, when $n=5$:

$$
F^5=
\begin{pmatrix}
F_6 & F_5 \\
F_5 & F_4
\end{pmatrix}
$$

Substituting the Fibonacci numbers:

$$
F^5=
\begin{pmatrix}
8 & 5 \\
5 & 3
\end{pmatrix}
$$

This matches our calculation.

---

## 7. MULTIPLY F BY A GENERAL VECTOR

Consider an arbitrary column vector:

$$
v=
\begin{pmatrix}
a \\
b
\end{pmatrix}
$$

Multiply it by the Fibonacci matrix:

$$
Fv=
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
a \\
b
\end{pmatrix}
$$

Multiply each row by the column:

$$
Fv=
\begin{pmatrix}
1\cdot a+1\cdot b \\
1\cdot a+0\cdot b
\end{pmatrix}
$$

Simplifying:

$$
Fv=
\begin{pmatrix}
a+b \\
a
\end{pmatrix}
$$

Therefore, the result is:

$$
F
\begin{pmatrix}
a \\
b
\end{pmatrix}
=
\begin{pmatrix}
a+b \\
a
\end{pmatrix}
$$

---

## 8. EXPLAIN THE RECURRENCE STEP

The multiplication produces the vector:

$$
\begin{pmatrix}
a+b \\
a
\end{pmatrix}
$$

This represents one step of the Fibonacci recurrence.

- The new first entry is the sum of the previous two entries.
- The new second entry is the previous first entry.

For example, start with:

$$
v=
\begin{pmatrix}
5 \\
3
\end{pmatrix}
$$

Multiply by F:

$$
Fv=
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
5 \\
3
\end{pmatrix}
$$

The result is:

$$
Fv=
\begin{pmatrix}
8 \\
5
\end{pmatrix}
$$

We obtain the next Fibonacci number, 8, while keeping 5 as the second entry.

This is exactly the same process used to generate the Fibonacci sequence.

---

## 9. CONCLUSION

We calculated the first five powers of the Fibonacci matrix and identified the relationship between matrix powers and Fibonacci numbers.

The general formula is:

$$
F^n=
\begin{pmatrix}
F_{n+1} & F_n \\
F_n & F_{n-1}
\end{pmatrix}
$$

We also demonstrated that multiplying the Fibonacci matrix by a general column vector gives:

$$
F
\begin{pmatrix}
a \\
b
\end{pmatrix}
=
\begin{pmatrix}
a+b \\
a
\end{pmatrix}
$$

This multiplication performs exactly one step of the Fibonacci recurrence.

Therefore, matrix multiplication provides a convenient way to represent and generate the Fibonacci sequence.
