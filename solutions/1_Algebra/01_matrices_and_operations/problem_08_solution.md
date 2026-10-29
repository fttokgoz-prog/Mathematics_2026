# Exercise 8. Row Operations and Their Reversibility

## Given

A = (  1   2  -1 )
    (  2   4   1 )
    ( -1   1   3 )


We must perform the following row operations in order:

1. R₂ ← R₂ − 2R₁
2. R₃ ← R₃ + R₁
3. Interchange R₂ and R₃

After each operation, we write the resulting matrix and explain how to reverse the operation.

## 1. Perform R₂ ← R₂ − 2R₁

This operation means that we multiply the first row by 2 and subtract the result from the second row. The first and third rows remain unchanged.

The original matrix is:

A = (  1   2  -1 )
    (  2   4   1 )
    ( -1   1   3 )


Step 1: Multiply the first row by 2.

R₁ = (1, 2, -1)

2R₁ = (2, 4, -2)


Step 2: Subtract 2R₁ from the second row.

The original second row is:

R₂ = (2, 4, 1)

Calculate each entry:

2 − 2 = 0

4 − 4 = 0

1 − (-2) = 3


Therefore, the new second row is:

R₂ = (0, 0, 3)


Step 3: Write the resulting matrix.

A₁ = (  1   2  -1 )
     (  0   0   3 )
     ( -1   1   3 )


**Reverse operation:**

To reverse R₂ ← R₂ − 2R₁, we add 2R₁ back to R₂.

The reverse operation is:

R₂ ← R₂ + 2R₁

This restores the original second row.


## 2. Perform R₃ ← R₃ + R₁

We now use the matrix obtained after Step 1.

A₁ = (  1   2  -1 )
     (  0   0   3 )
     ( -1   1   3 )


This operation means that we add the first row to the third row. The first and second rows remain unchanged.


Step 1: Identify the rows.

First row:

R₁ = (1, 2, -1)

Third row:

R₃ = (-1, 1, 3)


Step 2: Add the corresponding entries.

First entry:

-1 + 1 = 0

Second entry:

1 + 2 = 3

Third entry:

3 + (-1) = 2


Therefore, the new third row is:

R₃ = (0, 3, 2)


Step 3: Write the resulting matrix.

A₂ = (  1   2  -1 )
     (  0   0   3 )
     (  0   3   2 )


**Reverse operation:**

To reverse R₃ ← R₃ + R₁, we subtract the first row from the third row.

The reverse operation is:

R₃ ← R₃ − R₁

This restores the previous third row.


## 3. Interchange R₂ and R₃

We now use the matrix obtained after Step 2.

A₂ = (  1   2  -1 )
     (  0   0   3 )
     (  0   3   2 )


Interchanging R₂ and R₃ means swapping the second and third rows. The first row remains unchanged.


Step 1: Identify the rows to interchange.

Second row:

R₂ = (0, 0, 3)

Third row:

R₃ = (0, 3, 2)


Step 2: Swap the two rows.

The second row becomes (0, 3, 2).

The third row becomes (0, 0, 3).


Step 3: Write the resulting matrix.

A₃ = (  1   2  -1 )
     (  0   3   2 )
     (  0   0   3 )


**Reverse operation:**

To reverse the interchange, we swap the second and third rows again.

The reverse operation is:

Interchange R₂ and R₃

Swapping the same two rows a second time restores the previous matrix.


## Conclusion

Elementary row operations are reversible because each operation has an inverse operation that restores the previous matrix.

1. R₂ ← R₂ − 2R₁ is reversed by R₂ ← R₂ + 2R₁.

2. R₃ ← R₃ + R₁ is reversed by R₃ ← R₃ − R₁.

3. Interchanging R₂ and R₃ is reversed by interchanging R₂ and R₃ again.

The final matrix after all three operations is:

A₃ = (  1   2  -1 )
     (  0   3   2 )
     (  0   0   3 )

These operations demonstrate how rows can be transformed in a controlled way while preserving the ability to return to the previous matrix.
