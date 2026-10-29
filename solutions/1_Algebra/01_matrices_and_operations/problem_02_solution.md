# Exercise 2. Addition and Scalar Multiplication

Given:

A = ( 1   2 )
    ( -1  3 )

B = ( 4  -2 )
    ( 0   5 )

## 1. Compute A + B

Matrix addition means adding the numbers in the same positions.

Step 1: Add the corresponding entries.

A + B = ( 1 + 4       2 + (-2) )
        ( -1 + 0      3 + 5    )

Step 2: Calculate each entry.

1 + 4 = 5

2 + (-2) = 0

-1 + 0 = -1

3 + 5 = 8

Final answer:

A + B = ( 5   0 )
        ( -1  8 )


## 2. Compute A - B

Matrix subtraction means subtracting the numbers in the same positions.

Step 1: Subtract the corresponding entries.

A - B = ( 1 - 4       2 - (-2) )
        ( -1 - 0      3 - 5    )

Step 2: Calculate each entry.

1 - 4 = -3

2 - (-2) = 4

-1 - 0 = -1

3 - 5 = -2

Final answer:

A - B = ( -3   4  )
        ( -1  -2  )


## 3. Compute 3A - 2B

First, multiply every entry of A by 3 and every entry of B by 2. Then subtract the resulting matrices.

Step 1: Calculate 3A.

3A = ( 3 × 1       3 × 2 )
     ( 3 × (-1)    3 × 3 )

3A = (  3   6 )
     ( -3   9 )


Step 2: Calculate 2B.

2B = ( 2 × 4       2 × (-2) )
     ( 2 × 0       2 × 5    )

2B = ( 8  -4 )
     ( 0  10 )


Step 3: Subtract 2B from 3A.

3A - 2B = ( 3 - 8       6 - (-4) )
          ( -3 - 0      9 - 10   )

Step 4: Calculate each entry.

3 - 8 = -5

6 - (-4) = 10

-3 - 0 = -3

9 - 10 = -1

Final answer:

3A - 2B = ( -5   10 )
          ( -3   -1 )


## 4. Explain why matrix addition is possible only for matrices of the same size.

Matrix addition is possible only when both matrices have the same number of rows and columns. This is because we add corresponding entries in the same positions. If the matrices have different sizes, some entries will not have matching positions, so the addition cannot be performed.
