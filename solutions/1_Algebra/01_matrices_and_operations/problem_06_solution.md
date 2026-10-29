# Exercise 6. Transpose

## Given

A = ( 1  2  3 )
    ( 4  5  6 )


B = (  1  0 )
    (  2  1 )
    ( -1  3 )


## 1. Compute Aᵀ

The transpose of a matrix is obtained by changing its rows into columns. The first row becomes the first column, and the second row becomes the second column.

The first row of A is (1, 2, 3).

The second row of A is (4, 5, 6).

After changing the rows into columns, we get:

Aᵀ = ( 1  4 )
     ( 2  5 )
     ( 3  6 )

The original matrix A has size 2 × 3, so its transpose has size 3 × 2.


## 2. Compute Bᵀ

To find the transpose of B, we change every row into a column.

The first row of B is (1, 0).

The second row of B is (2, 1).

The third row of B is (-1, 3).

After changing the rows into columns, we get:

Bᵀ = (  1   2  -1 )
     (  0   1   3 )

The original matrix B has size 3 × 2, so its transpose has size 2 × 3.


## 3. Compute AB

Matrix A has size 2 × 3, and matrix B has size 3 × 2.

The number of columns in A is 3, and the number of rows in B is also 3. Therefore, the multiplication AB is defined.

The result has size 2 × 2.

AB = ( 1  2  3 ) (  1  0 )
     ( 4  5  6 ) (  2  1 )
                   ( -1  3 )


**Step 1: Calculate the first row, first column.**

Multiply the first row of A by the first column of B.

1 × 1 = 1

2 × 2 = 4

3 × (-1) = -3

Add the results:

1 + 4 + (-3) = 5 - 3 = 2

The first entry is 2.


**Step 2: Calculate the first row, second column.**

Multiply the first row of A by the second column of B.

1 × 0 = 0

2 × 1 = 2

3 × 3 = 9

Add the results:

0 + 2 + 9 = 11

The second entry is 11.


**Step 3: Calculate the second row, first column.**

Multiply the second row of A by the first column of B.

4 × 1 = 4

5 × 2 = 10

6 × (-1) = -6

Add the results:

4 + 10 + (-6) = 14 - 6 = 8

The third entry is 8.


**Step 4: Calculate the second row, second column.**

Multiply the second row of A by the second column of B.

4 × 0 = 0

5 × 1 = 5

6 × 3 = 18

Add the results:

0 + 5 + 18 = 23

The fourth entry is 23.


**Final result:**

AB = (  2  11 )
     (  8  23 )


## 4. Verify that (AB)ᵀ = BᵀAᵀ

We need to calculate both sides and check whether they are equal.

### Step 1: Calculate (AB)ᵀ

From the previous calculation, we know that:

AB = (  2  11 )
     (  8  23 )

To find the transpose, we change the rows into columns.

The first row (2, 11) becomes the first column.

The second row (8, 23) becomes the second column.

Therefore:

(AB)ᵀ = (  2   8 )
        ( 11  23 )


### Step 2: Calculate BᵀAᵀ

From the previous calculations:

Bᵀ = (  1   2  -1 )
     (  0   1   3 )


Aᵀ = ( 1  4 )
     ( 2  5 )
     ( 3  6 )

The number of columns in Bᵀ is 3, and the number of rows in Aᵀ is also 3. Therefore, the multiplication BᵀAᵀ is defined.

The result has size 2 × 2.

BᵀAᵀ = (  1   2  -1 ) ( 1  4 )
       (  0   1   3 ) ( 2  5 )
                         ( 3  6 )


**First row, first column:**

Multiply the first row of Bᵀ by the first column of Aᵀ.

1 × 1 = 1

2 × 2 = 4

(-1) × 3 = -3

Add the results:

1 + 4 + (-3) = 2


**First row, second column:**

Multiply the first row of Bᵀ by the second column of Aᵀ.

1 × 4 = 4

2 × 5 = 10

(-1) × 6 = -6

Add the results:

4 + 10 + (-6) = 14 - 6 = 8


**Second row, first column:**

Multiply the second row of Bᵀ by the first column of Aᵀ.

0 × 1 = 0

1 × 2 = 2

3 × 3 = 9

Add the results:

0 + 2 + 9 = 11


**Second row, second column:**

Multiply the second row of Bᵀ by the second column of Aᵀ.

0 × 4 = 0

1 × 5 = 5

3 × 6 = 18

Add the results:

0 + 5 + 18 = 23


Therefore:

BᵀAᵀ = (  2   8 )
       ( 11  23 )


### Step 3: Compare both results

We calculated:

(AB)ᵀ = (  2   8 )
        ( 11  23 )


BᵀAᵀ = (  2   8 )
       ( 11  23 )

Both matrices have exactly the same entries in the same positions.

Therefore:

(AB)ᵀ = BᵀAᵀ


## Conclusion

The transpose of a matrix changes its rows into columns and its columns into rows.

When we take the transpose of a product of two matrices, we must also reverse the order of the matrices.

Therefore, the general rule is:

(AB)ᵀ = BᵀAᵀ

This example verifies the rule because both sides produce the same matrix.
