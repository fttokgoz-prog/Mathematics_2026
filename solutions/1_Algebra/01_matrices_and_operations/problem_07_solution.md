# Exercise 7. Identity Matrix, Zero Matrix, and Powers

## Given

A = ( 2  1 )
    ( 0  2 )


We will compute AI, IA, A + 0, A², and A³.

The identity matrix I and the zero matrix 0 are both 2 × 2 matrices in this exercise.

The identity matrix is:

I = ( 1  0 )
    ( 0  1 )


The zero matrix is:

0 = ( 0  0 )
    ( 0  0 )


## 1. Compute AI

Matrix multiplication is performed by multiplying the rows of the first matrix by the columns of the second matrix and adding the products.

First, we multiply A by the identity matrix I:

AI = ( 2  1 ) ( 1  0 )
     ( 0  2 ) ( 0  1 )


**Step 1: Calculate the first row, first column.**

2 × 1 + 1 × 0 = 2 + 0 = 2


**Step 2: Calculate the first row, second column.**

2 × 0 + 1 × 1 = 0 + 1 = 1


**Step 3: Calculate the second row, first column.**

0 × 1 + 2 × 0 = 0 + 0 = 0


**Step 4: Calculate the second row, second column.**

0 × 0 + 2 × 1 = 0 + 2 = 2


Therefore:

AI = ( 2  1 )
     ( 0  2 )


We can see that AI = A. Multiplying a matrix by the identity matrix does not change the matrix.


## 2. Compute IA

Now, we multiply the identity matrix I by A. The order of multiplication is reversed.

IA = ( 1  0 ) ( 2  1 )
     ( 0  1 ) ( 0  2 )


**Step 1: Calculate the first row, first column.**

1 × 2 + 0 × 0 = 2 + 0 = 2


**Step 2: Calculate the first row, second column.**

1 × 1 + 0 × 2 = 1 + 0 = 1


**Step 3: Calculate the second row, first column.**

0 × 2 + 1 × 0 = 0 + 0 = 0


**Step 4: Calculate the second row, second column.**

0 × 1 + 1 × 2 = 0 + 2 = 2


Therefore:

IA = ( 2  1 )
     ( 0  2 )


We can see that IA = A as well. The identity matrix leaves A unchanged whether it is multiplied from the left or from the right.


## 3. Compute A + 0

Matrix addition means adding the corresponding entries in the same positions.

A = ( 2  1 )
    ( 0  2 )


0 = ( 0  0 )
    ( 0  0 )


We add the two matrices entry by entry:

A + 0 = ( 2 + 0    1 + 0 )
        ( 0 + 0    2 + 0 )


Now, calculate each entry:

2 + 0 = 2

1 + 0 = 1

0 + 0 = 0

2 + 0 = 2


Therefore:

A + 0 = ( 2  1 )
        ( 0  2 )


We can see that A + 0 = A. Adding a zero matrix does not change the original matrix because adding zero to any number leaves that number unchanged.


## 4. Compute A²

The notation A² means multiplying A by itself.

A² = A × A


A² = ( 2  1 ) ( 2  1 )
     ( 0  2 ) ( 0  2 )


**Step 1: Calculate the first row, first column.**

Multiply the first row of the first matrix by the first column of the second matrix.

2 × 2 + 1 × 0 = 4 + 0 = 4


**Step 2: Calculate the first row, second column.**

2 × 1 + 1 × 2 = 2 + 2 = 4


**Step 3: Calculate the second row, first column.**

0 × 2 + 2 × 0 = 0 + 0 = 0


**Step 4: Calculate the second row, second column.**

0 × 1 + 2 × 2 = 0 + 4 = 4


Therefore:

A² = ( 4  4 )
     ( 0  4 )


The matrix A² is obtained by multiplying A by itself once.


## 5. Compute A³

The notation A³ means multiplying A by itself three times.

A³ = A² × A


From the previous calculation:

A² = ( 4  4 )
     ( 0  4 )


Now, multiply A² by A:

A³ = ( 4  4 ) ( 2  1 )
     ( 0  4 ) ( 0  2 )


**Step 1: Calculate the first row, first column.**

4 × 2 + 4 × 0 = 8 + 0 = 8


**Step 2: Calculate the first row, second column.**

4 × 1 + 4 × 2 = 4 + 8 = 12


**Step 3: Calculate the second row, first column.**

0 × 2 + 4 × 0 = 0 + 0 = 0


**Step 4: Calculate the second row, second column.**

0 × 1 + 4 × 2 = 0 + 8 = 8


Therefore:

A³ = (  8  12 )
     (  0   8 )


The matrix A³ is obtained by multiplying A² by A.


## 6. Explain the roles of the matrices I and 0

The identity matrix I acts as a multiplicative identity. This means that multiplying a matrix by I does not change the original matrix.

In this exercise:

AI = A

IA = A

The zero matrix 0 acts as an additive identity. This means that adding the zero matrix to a matrix does not change the original matrix.

In this exercise:

A + 0 = A

Therefore, the identity matrix is used in matrix multiplication, while the zero matrix is used in matrix addition.


## 7. Describe the pattern in successive powers of A

The successive powers of A are:

A = ( 2  1 )
    ( 0  2 )


A² = ( 4  4 )
     ( 0  4 )


A³ = (  8  12 )
     (  0   8 )


Looking at the results, we can observe the following pattern:

- The diagonal entries double with each successive power: 2, 4, 8.
- The bottom-left entry remains 0 in every power.
- The top-right entry changes from 1 to 4 and then to 12.

The pattern can be expressed more generally as:

Aⁿ = ( 2ⁿ    n × 2ⁿ⁻¹ )
     (  0        2ⁿ   )

For example, when n = 2, the top-right entry is 2 × 2¹ = 4.

When n = 3, the top-right entry is 3 × 2² = 12.

Therefore, the diagonal entries follow powers of 2, while the top-right entry follows the pattern n × 2ⁿ⁻¹.


## Conclusion

The identity matrix I does not change a matrix when multiplied by it, and the zero matrix 0 does not change a matrix when added to it.

The successive powers A² and A³ show a clear pattern: the diagonal entries are powers of 2, the bottom-left entry remains zero, and the top-right entry follows the formula n × 2ⁿ⁻¹.

These results demonstrate the roles of identity and zero matrices and show how patterns can appear in successive powers of a matrix.
