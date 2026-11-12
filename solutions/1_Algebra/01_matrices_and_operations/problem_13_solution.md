
# EXERCISE 13
# A RECURRENCE WRITTEN IN MATRIX FORM

---

## 1. GIVEN

The following matrix is given:

$$
F =
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

We need to:

1. Calculate F², F³, F⁴, and F⁵.
2. Compare the results with the Fibonacci sequence.
3. Find the relationship between matrix powers and Fibonacci numbers.
4. Calculate the product of F and a general vector.

---

## 2. CALCULATING MATRIX POWERS

### STEP 1 - Calculate F²

$$
F^2 = F \cdot F
$$

$$
F^2 =
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

Result:

$$
\boxed{
F^2 =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
}
$$

---

### STEP 2 - Calculate F³

$$
F^3 = F^2 \cdot F
$$

$$
F^3 =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

Result:

$$
\boxed{
F^3 =
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
}
$$

---

### STEP 3 - Calculate F⁴

$$
F^4 = F^3 \cdot F
$$

$$
F^4 =
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

Result:

$$
\boxed{
F^4 =
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
}
$$

---

### STEP 4 - Calculate F⁵

$$
F^5 = F^4 \cdot F
$$

$$
F^5 =
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
$$

Result:

$$
\boxed{
F^5 =
\begin{pmatrix}
8 & 5 \\
5 & 3
\end{pmatrix}
}
$$

---

## 3. COMPARISON WITH THE FIBONACCI SEQUENCE

The Fibonacci sequence is:

**0, 1, 1, 2, 3, 5, 8, 13, ...**

Each number is obtained by adding the two previous numbers.

Comparing the matrix powers with the sequence:

| Matrix Power | Upper-Left | Upper-Right | Lower-Left | Lower-Right |
|:------------:|:----------:|:-----------:|:----------:|:-----------:|
| F² | 2 | 1 | 1 | 1 |
| F³ | 3 | 2 | 2 | 1 |
| F⁴ | 5 | 3 | 3 | 2 |
| F⁵ | 8 | 5 | 5 | 3 |

We can observe that the entries of each matrix are consecutive Fibonacci numbers.

The general formula is:

$$
\boxed{
F^n =
\begin{pmatrix}
Fib(n+1) & Fib(n) \\
Fib(n) & Fib(n-1)
\end{pmatrix}
}
$$

for n ≥ 1, where Fib(n) represents the nth Fibonacci number, with Fib(0) = 0 and Fib(1) = 1.

---

## 4. MULTIPLYING F BY A GENERAL VECTOR

Let the vector be:

$$
v =
\begin{pmatrix}
a \\
b
\end{pmatrix}
$$

Multiply F by this vector:

$$
Fv =
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
a \\
b
\end{pmatrix}
$$

Calculate each entry:

$$
Fv =
\begin{pmatrix}
1a+1b \\
1a+0b
\end{pmatrix}
$$

Therefore:

$$
\boxed{
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
}
$$

---

## 5. EXPLANATION OF THE RECURRENCE STEP

The multiplication produces a new vector:

$$
\begin{pmatrix}
a+b \\
a
\end{pmatrix}
$$

This means:

- The first entry becomes the sum of the previous two entries.
- The second entry becomes the previous first entry.

For example, if:

$$
v =
\begin{pmatrix}
3 \\
2
\end{pmatrix}
$$

then:

$$
Fv =
\begin{pmatrix}
3+2 \\
3
\end{pmatrix}
=
\begin{pmatrix}
5 \\
3
\end{pmatrix}
$$

This is exactly one step in the Fibonacci sequence.

---

## 6. FINAL ANSWERS

### Matrix Powers

$$
F^2 =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
$$

$$
F^3 =
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
$$

$$
F^4 =
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
$$

$$
F^5 =
\begin{pmatrix}
8 & 5 \\
5 & 3
\end{pmatrix}
$$

### General Formula

$$
F^n =
\begin{pmatrix}
Fib(n+1) & Fib(n) \\
Fib(n) & Fib(n-1)
\end{pmatrix}
$$

### Vector Multiplication

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

## 7. CONCLUSION

The powers of matrix F generate consecutive Fibonacci numbers.

Multiplying F by a vector containing two consecutive terms creates the next Fibonacci number while keeping the previous first term.

Therefore, matrix multiplication provides a simple way to represent and calculate the Fibonacci recurrence.
