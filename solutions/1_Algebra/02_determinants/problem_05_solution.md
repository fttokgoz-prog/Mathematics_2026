# Exercise 5. Matrix Times Vector

## Given

A = ( 2  -1 )
    ( 1   3 )


x = ( 4 )
    ( 2 )


We need to compute Ax and express the result as a linear combination of the columns of A, using the entries of vector x as coefficients.

## 1. Compute Ax

To multiply a matrix by a vector, we multiply each row of the matrix by the vector and add the products.

Matrix A has 2 rows, and vector x has 2 entries. Therefore, the multiplication is defined, and the result will be a vector with 2 entries.

Ax = ( 2  -1 ) ( 4 )
     ( 1   3 ) ( 2 )


**Step 1: Calculate the first entry.**

The first row of A is (2, -1), and the vector x is (4, 2).

Multiply the corresponding entries and add the results:

2 × 4 + (-1) × 2

= 8 - 2

= 6


Therefore, the first entry of Ax is 6.


**Step 2: Calculate the second entry.**

The second row of A is (1, 3).

Multiply the corresponding entries and add the results:

1 × 4 + 3 × 2

= 4 + 6

= 10


Therefore, the second entry of Ax is 10.


**Step 3: Write the final result.**

The first entry is 6, and the second entry is 10.

Therefore:

Ax = (  6 )
     ( 10 )


## 2. Express Ax as a linear combination of the columns of A

A linear combination means multiplying each column of a matrix by a number and then adding the resulting vectors.

The entries of vector x provide the coefficients for the columns of A.

### Step 1: Identify the columns of A

The first column of A is:

c₁ = ( 2 )
     ( 1 )


The second column of A is:

c₂ = ( -1 )
     (  3 )


### Step 2: Identify the coefficients

The vector x is:

x = ( 4 )
    ( 2 )


The first entry is 4, so the first column is multiplied by 4.

The second entry is 2, so the second column is multiplied by 2.

Therefore, the linear combination is:

Ax = 4c₁ + 2c₂


### Step 3: Multiply each column by its coefficient

First column:

4c₁ = 4 × ( 2 )
             ( 1 )

4c₁ = ( 8 )
      ( 4 )


Second column:

2c₂ = 2 × ( -1 )
             (  3 )

2c₂ = ( -2 )
      (  6 )


### Step 4: Add the resulting vectors

Ax = (  8 ) + ( -2 )
     (  4 )   (  6 )


Add the first entries:

8 + (-2) = 6


Add the second entries:

4 + 6 = 10


Therefore:

Ax = (  6 )
     ( 10 )


## 3. Compare the two methods

Using direct matrix-vector multiplication, we obtained:

Ax = (  6 )
     ( 10 )


Using a linear combination of the columns of A, we obtained:

Ax = 4c₁ + 2c₂

Ax = (  6 )
     ( 10 )


Both methods give the same result.

This confirms that multiplying a matrix by a vector is equivalent to taking a linear combination of the matrix's columns, using the entries of the vector as coefficients.


## Conclusion

The final result is:

Ax = (  6 )
     ( 10 )


The linear combination is:

Ax = 4c₁ + 2c₂


The first column of A is multiplied by 4, and the second column is multiplied by 2. Adding these vectors produces the same result as direct matrix-vector multiplication.
