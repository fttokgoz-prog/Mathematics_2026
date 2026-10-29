# Exercise 13. A Recurrence Written in Matrix Form

## Given

F = ( 1  1 )
    ( 1  0 )


We need to compute F², F³, F⁴, and F⁵, compare the results with the sequence 0, 1, 1, 2, 3, 5, 8, ..., and explain how multiplying F by a vector performs one recurrence step.

## 1. Compute F²

The notation F² means multiplying F by itself.

F² = F × F

F² = ( 1  1 ) ( 1  1 )
     ( 1  0 ) ( 1  0 )


**First row, first column:**

1 × 1 + 1 × 1 = 1 + 1 = 2


**First row, second column:**

1 × 1 + 1 × 0 = 1 + 0 = 1


**Second row, first column:**

1 × 1 + 0 × 1 = 1 + 0 = 1


**Second row, second column:**

1 × 1 + 0 × 0 = 1 + 0 = 1


Therefore:

F² = ( 2  1 )
     ( 1  1 )


## 2. Compute F³

We multiply F² by F.

F³ = F² × F

F³ = ( 2  1 ) ( 1  1 )
     ( 1  1 ) ( 1  0 )


**First row, first column:**

2 × 1 + 1 × 1 = 2 + 1 = 3


**First row, second column:**

2 × 1 + 1 × 0 = 2 + 0 = 2


**Second row, first column:**

1 × 1 + 1 × 1 = 1 + 1 = 2


**Second row, second column:**

1 × 1 + 1 × 0 = 1 + 0 = 1


Therefore:

F³ = ( 3  2 )
     ( 2  1 )


## 3. Compute F⁴

We multiply F³ by F.

F⁴ = F³ × F

F⁴ = ( 3  2 ) ( 1  1 )
     ( 2  1 ) ( 1  0 )


**First row, first column:**

3 × 1 + 2 × 1 = 3 + 2 = 5


**First row, second column:**

3 × 1 + 2 × 0 = 3 + 0 = 3


**Second row, first column:**

2 × 1 + 1 × 1 = 2 + 1 = 3


**Second row, second column:**

2 × 1 + 1 × 0 = 2 + 0 = 2


Therefore:

F⁴ = ( 5  3 )
     ( 3  2 )


## 4. Compute F⁵

We multiply F⁴ by F.

F⁵ = F⁴ × F

F⁵ = ( 5  3 ) ( 1  1 )
     ( 3  2 ) ( 1  0 )


**First row, first column:**

5 × 1 + 3 × 1 = 5 + 3 = 8


**First row, second column:**

5 × 1 + 3 × 0 = 5 + 0 = 5


**Second row, first column:**

3 × 1 + 2 × 1 = 3 + 2 = 5


**Second row, second column:**

3 × 1 + 2 × 0 = 3 + 0 = 3


Therefore:

F⁵ = ( 8  5 )
     ( 5  3 )


## 5. Compare the results with the sequence 0, 1, 1, 2, 3, 5, 8, ...

The given sequence is:

0, 1, 1, 2, 3, 5, 8, ...

This is the Fibonacci sequence. Each term is obtained by adding the two previous terms.

For example:

0 + 1 = 1

1 + 1 = 2

1 + 2 = 3

2 + 3 = 5

3 + 5 = 8


Now, compare the matrix powers:

F² = ( 2  1 )
     ( 1  1 )


F³ = ( 3  2 )
     ( 2  1 )


F⁴ = ( 5  3 )
     ( 3  2 )


F⁵ = ( 8  5 )
     ( 5  3 )


The entries of these matrices are consecutive Fibonacci numbers.

The top-left entries are:

2, 3, 5, 8

The top-right entries are:

1, 2, 3, 5

The bottom-left entries are:

1, 2, 3, 5

The bottom-right entries are:

1, 1, 2, 3


Therefore, the powers of F contain consecutive Fibonacci numbers, and the entries follow the same addition pattern as the sequence.

In general, for n ≥ 1:

Fⁿ = ( Fₙ₊₁  Fₙ   )
     ( Fₙ     Fₙ₋₁ )

Here, Fₙ denotes the nth Fibonacci number, using F₀ = 0 and F₁ = 1.


## 6. Compute F multiplied by the vector (a, b)

We are given the vector:

v = ( a )
    ( b )


We multiply F by this vector:

Fv = ( 1  1 ) ( a )
     ( 1  0 ) ( b )


**First entry:**

1 × a + 1 × b = a + b


**Second entry:**

1 × a + 0 × b = a + 0 = a


Therefore:

Fv = ( a + b )
     (   a   )


## 7. Explain how this multiplication performs one recurrence step

The original vector is:

v = ( a )
    ( b )


After multiplying by F, we obtain:

Fv = ( a + b )
     (   a   )


The first entry becomes a + b, which is the sum of the two original entries.

The second entry becomes a, which is the previous first entry.

Therefore, the transformation changes the pair (a, b) into (a + b, a).

This is exactly one recurrence step: the next term is calculated by adding the two current terms, while the previous first term is retained as the second entry.

For example, if the vector is:

v = ( 3 )
    ( 2 )


Then:

Fv = ( 3 + 2 )
     (   3   )


Fv = ( 5 )
     ( 3 )


The pair (3, 2) becomes (5, 3), following the Fibonacci recurrence.


## Conclusion

The matrix F generates consecutive Fibonacci numbers through its powers.

We obtained:

F² = ( 2  1 )
     ( 1  1 )


F³ = ( 3  2 )
     ( 2  1 )


F⁴ = ( 5  3 )
     ( 3  2 )


F⁵ = ( 8  5 )
     ( 5  3 )


We also showed that multiplying F by a vector (a, b) produces (a + b, a). This adds the two current terms and carries one term forward, performing exactly one step of the Fibonacci recurrence.
