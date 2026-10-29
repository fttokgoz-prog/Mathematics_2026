# Exercise 5. Matrix Times Vector

**Given:**

A = ( 2  -1 )
    ( 1   3 )

x = ( 4 )
    ( 2 )


## 1. Compute Ax

To multiply a matrix by a vector, we multiply each row of the matrix by the entries of the vector. Then, we add the products to obtain each entry of the result.

The matrix A has 2 rows, and the vector x has 2 entries. Therefore, the multiplication Ax is defined, and the result will be a vector with 2 entries.

**Step 1: Calculate the first entry.**

The first row of A contains the numbers 2 and -1. The vector x contains the numbers 4 and 2.

We multiply the corresponding entries and add the results:

2 × 4 + (-1) × 2 = 8 - 2 = 6

Therefore, the first entry of Ax is 6.

**Step 2: Calculate the second entry.**

The second row of A contains the numbers 1 and 3.

We multiply the corresponding entries of this row by the entries of x and add the results:

1 × 4 + 3 × 2 = 4 + 6 = 10

Therefore, the second entry of Ax is 10.

**Step 3: Write the final result.**

The first entry is 6, and the second entry is 10.

Ax = (  6 )
     ( 10 )


## 2. Express Ax as a linear combination of the columns of A

A linear combination means multiplying each column of a matrix by a number and then adding the resulting vectors.

**Step 1: Identify the columns of A.**

The first column of A is:

c₁ = ( 2 )
     ( 1 )

The second column of A is:

c₂ = ( -1 )
     (  3 )

**Step 2: Identify the coefficients.**

The vector x is:

x = ( 4 )
    ( 2 )

The first entry of x is 4, and the second entry is 2. These numbers are the coefficients of the corresponding columns of A.

Therefore, the first column is multiplied by 4, and the second column is multiplied by 2.

This gives:

Ax = 4c₁ + 2c₂

**Step 3: Multiply each column by its coefficient.**

First column:

4c₁ = 4 × ( 2 ) = ( 8 )
             ( 1 )   ( 4 )

Second column:

2c₂ = 2 × ( -1 ) = ( -2 )
             (  3 )   (  6 )

**Step 4: Add the resulting vectors.**

Ax = (  8 ) + ( -2 )
     (  4 )   (  6 )

We add the corresponding entries:

First entry: 8 + (-2) = 6

Second entry: 4 + 6 = 10

Therefore:

Ax = (  6 )
     ( 10 )


## Conclusion

The result of multiplying a matrix by a vector can be expressed as a linear combination of the columns of the matrix.

The entries of the vector determine the coefficients used to multiply each column. In this exercise, the first column is multiplied by 4, and the second column is multiplied by 2. Adding these vectors gives the same result as calculating Ax directly.
