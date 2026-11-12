
# EXERCISE 13
# A RECURRENCE WRITTEN IN MATRIX FORM

---

## 1. GIVEN

We are given the following Fibonacci matrix:

```math
F =
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
```

The Fibonacci sequence is:

```math
0,\ 1,\ 1,\ 2,\ 3,\ 5,\ 8,\ 13,\ 21,\ldots
```

We need to:

1. Calculate F², F³, F⁴ and F⁵.
2. Compare the entries with the Fibonacci sequence.
3. Describe the relationship between matrix powers and Fibonacci numbers.
4. Calculate the product of F and the vector (a,b)ᵀ.
5. Explain how this multiplication performs one recurrence step.

---

## 2. CALCULATE THE MATRIX POWERS

### STEP 1 - Calculate F²

By definition:

```math
F^2=F\cdot F
```

Substitute the matrix:

```math
F^2 =
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
```

Multiply the matrices:

```math
F^2 =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
```

### STEP 2 - Calculate F³

We multiply F² by F:

```math
F^3=F^2\cdot F
```

```math
F^3 =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
```

The result is:

```math
F^3 =
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
```

### STEP 3 - Calculate F⁴

We multiply F³ by F:

```math
F^4=F^3\cdot F
```

```math
F^4 =
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
```

The result is:

```math
F^4 =
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
```

### STEP 4 - Calculate F⁵

We multiply F⁴ by F:

```math
F^5=F^4\cdot F
```

```math
F^5 =
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
```

The result is:

```math
F^5 =
\begin{pmatrix}
8 & 5 \\
5 & 3
\end{pmatrix}
```

---

## 3. COMPARISON WITH THE FIBONACCI SEQUENCE

The Fibonacci sequence is:

```math
0,\ 1,\ 1,\ 2,\ 3,\ 5,\ 8,\ 13,\ldots
```

Our calculated matrices are:

```math
F^2 =
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
```

```math
F^3 =
\begin{pmatrix}
3 & 2 \\
2 & 1
\end{pmatrix}
```

```math
F^4 =
\begin{pmatrix}
5 & 3 \\
3 & 2
\end{pmatrix}
```

```math
F^5 =
\begin{pmatrix}
8 & 5 \\
5 & 3
\end{pmatrix}
```

We can observe that the entries of these matrices are consecutive Fibonacci numbers.

The general pattern is:

```math
F^n =
\begin{pmatrix}
F_{n+1} & F_n \\
F_n & F_{n-1}
\end{pmatrix}
```

Here, Fₙ represents the nth Fibonacci number, with F₀ = 0 and F₁ = 1.

---

## 4. MULTIPLY THE MATRIX BY A VECTOR

We now calculate the product of F and a general vector:

```math
F
\begin{pmatrix}
a \\
b
\end{pmatrix}
```

Substitute the matrix:

```math
=
\begin{pmatrix}
1 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
a \\
b
\end{pmatrix}
```

Multiply the rows by the column:

```math
=
\begin{pmatrix}
1\cdot a+1\cdot b \\
1\cdot a+0\cdot b
\end{pmatrix}
```

Simplifying gives:

```math
=
\begin{pmatrix}
a+b \\
a
\end{pmatrix}
```

Therefore, the final result is:

```math
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
```

---

## 5. EXPLANATION OF THE RECURRENCE STEP

The Fibonacci recurrence is defined by adding the two previous consecutive terms.

The rule is:

```math
F_{n+1}=F_n+F_{n-1}
```

The matrix multiplication produces:

```math
\begin{pmatrix}
a \\
b
\end{pmatrix}
\longrightarrow
\begin{pmatrix}
a+b \\
a
\end{pmatrix}
```

This means:

- The new first entry is the sum of the previous two entries.
- The new second entry is the previous first entry.

For example, if:

```math
\begin{pmatrix}
a \\
b
\end{pmatrix}
=
\begin{pmatrix}
3 \\
2
\end{pmatrix}
```

Then:

```math
F
\begin{pmatrix}
3 \\
2
\end{pmatrix}
=
\begin{pmatrix}
3+2 \\
3
\end{pmatrix}
=
\begin{pmatrix}
5 \\
3
\end{pmatrix}
```

This is exactly one step of the Fibonacci recurrence.

---

## 6. CONCLUSION

The powers of the Fibonacci matrix generate consecutive Fibonacci numbers.

We calculated F², F³, F⁴ and F⁵ and identified the general pattern.

The matrix multiplication also performs one recurrence step by adding two consecutive terms and keeping the previous first term.

Therefore, matrix multiplication provides a convenient way to represent and calculate the Fibonacci sequence.
