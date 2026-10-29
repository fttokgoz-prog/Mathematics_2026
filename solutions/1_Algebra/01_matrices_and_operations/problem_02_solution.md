# Exercise 2. Addition and Scalar Multiplication

## Question

Given the matrices

A = (  1   2 )
    ( -1   3 )

B = ( 4  -2 )
    ( 0   5 )

Compute the following matrix expressions:

1. A + B
2. A - B
3. 3A - 2B

Explain why matrix addition is possible only for matrices of the same size.

## Solution

### Part 1. Calculate A + B

Matrix addition is performed by adding the corresponding entries of two matrices.

For matrix addition to be defined, both matrices must have the same number of rows and columns. This ensures that every entry in the first matrix has a corresponding entry in the second matrix.

The given matrices are:

A = (  1   2 )
    ( -1   3 )

B = ( 4  -2 )
    ( 0   5 )

Both A and B have 2 rows and 2 columns. Therefore, their addition is defined, and the result will also be a 2 × 2 matrix.

The general formula for matrix addition is:

(A + B)ᵢⱼ = aᵢⱼ + bᵢⱼ

This means that each entry of A is added to the entry in the same position in B.

**Step 1: Calculate the first row.**

The first row of A is (1, 2).

The first row of B is (4, -2).

Add the first entries:

1 + 4 = 5

Add the second entries:

2 + (-2) = 0

Therefore, the first row of A + B is:

(5, 0)

**Step 2: Calculate the second row.**

The second row of A is (-1, 3).

The second row of B is (0, 5).

Add the first entries:

-1 + 0 = -1

Add the second entries:

3 + 5 = 8

Therefore, the second row of A + B is:

(-1, 8)

**Step 3: Write the resulting matrix.**

Combining the two calculated rows gives:

A + B = (  5   0 )
        ( -1   8 )

Therefore, the result is:

**A + B = (5, 0; -1, 8)**

### Part 2. Calculate A - B

Matrix subtraction is performed by subtracting each entry of the second matrix from the corresponding entry of the first matrix.

The formula is:

(A - B)ᵢⱼ = aᵢⱼ - bᵢⱼ

Both matrices have size 2 × 2, so subtraction is defined.

We start with:

A = (  1   2 )
    ( -1   3 )

B = ( 4  -2 )
    ( 0   5 )

**Step 1: Calculate the first row.**

The first row of A is (1, 2).

The first row of B is (4, -2).

Subtract the first entries:

1 - 4 = -3

Subtract the second entries:

2 - (-2) = 2 + 2 = 4

Remember that subtracting a negative number is equivalent to adding a positive number.

Therefore, the first row of A - B is:

(-3, 4)

**Step 2: Calculate the second row.**

The second row of A is (-1, 3).

The second row of B is (0, 5).

Subtract the first entries:

-1 - 0 = -1

Subtract the second entries:

3 - 5 = -2

Therefore, the second row of A - B is:

(-1, -2)

**Step 3: Write the resulting matrix.**

Combining the two rows gives:

A - B = ( -3   4 )
        ( -1  -2 )

Therefore, the result is:

**A - B = (-3, 4; -1, -2)**

### Part 3. Calculate 3A - 2B

In this expression, we must first multiply matrix A by 3 and matrix B by 2. After calculating both matrices, we subtract the corresponding entries.

Multiplying a matrix by a scalar means multiplying every entry of the matrix by that number.

The scalar multiplication formula is:

(kA)ᵢⱼ = k × aᵢⱼ

Therefore, we calculate 3A and 2B separately before performing the subtraction.

#### Step 1: Calculate 3A

The original matrix is:

A = (  1   2 )
    ( -1   3 )

Multiply every entry by 3.

First row:

3 × 1 = 3

3 × 2 = 6

Second row:

3 × (-1) = -3

3 × 3 = 9

Therefore:

3A = (  3   6 )
     ( -3   9 )

#### Step 2: Calculate 2B

The original matrix is:

B = ( 4  -2 )
    ( 0   5 )

Multiply every entry by 2.

First row:

2 × 4 = 8

2 × (-2) = -4

Second row:

2 × 0 = 0

2 × 5 = 10

Therefore:

2B = ( 8  -4 )
     ( 0  10 )

#### Step 3: Subtract 2B from 3A

We have obtained:

3A = (  3   6 )
     ( -3   9 )

2B = ( 8  -4 )
     ( 0  10 )

Now calculate:

3A - 2B = ( 3 - 8       6 - (-4) )
          ( -3 - 0      9 - 10   )

Calculate each entry separately.

**First row, first column:**

3 - 8 = -5

**First row, second column:**

6 - (-4) = 6 + 4 = 10

**Second row, first column:**

-3 - 0 = -3

**Second row, second column:**

9 - 10 = -1

Therefore, the resulting matrix is:

3A - 2B = ( -5   10 )
          ( -3   -1 )

The final result is:

**3A - 2B = (-5, 10; -3, -1)**

### Part 4. Explain why matrix addition is possible only for matrices of the same size

Matrix addition requires both matrices to have the same dimensions.

Suppose matrix A has size m × n and matrix B has size p × q.

For A + B to be defined, the corresponding entries must exist in both matrices. Therefore, the number of rows and columns must match.

The condition is:

m = p

and

n = q

Consequently, the two matrices must have the same size:

m × n = p × q

**Step 1: Consider the dimensions of A and B.**

In this exercise:

A has size 2 × 2.

B has size 2 × 2.

Both matrices have two rows and two columns.

Therefore, every entry in A has a corresponding entry in B.

**Step 2: Apply the addition rule.**

The entries can be added position by position:

First row, first column: 1 + 4

First row, second column: 2 + (-2)

Second row, first column: -1 + 0

Second row, second column: 3 + 5

All four additions are defined because the corresponding entries exist in both matrices.

**Step 3: State the general rule.**

If two matrices have different dimensions, their entries cannot be paired at every corresponding position.

For this reason, matrix addition is defined only when both matrices have the same number of rows and columns.

Scalar multiplication, however, does not require two matrices to have the same size because it involves multiplying each entry of a single matrix by a number.

## Final Answers

**1. Matrix addition**

A + B = (  5   0 )
        ( -1   8 )

**2. Matrix subtraction**

A - B = ( -3   4 )
        ( -1  -2 )

**3. Scalar multiplication and subtraction**

3A - 2B = ( -5   10 )
          ( -3   -1 )

**4. Condition for matrix addition**

Two matrices can be added only if they have the same number of rows and the same number of columns.

In this exercise, both A and B are 2 × 2 matrices, so all three requested expressions are defined.

## Explanation of the Method

Matrix addition and subtraction operate on corresponding entries. Scalar multiplication multiplies every entry by the same number.

For the expression 3A - 2B, the scalar multiplications must be performed first, followed by entry-by-entry subtraction.

The dimensions determine whether the operations are defined. Since A and B have the same size, addition and subtraction are possible, and the resulting matrices retain the same 2 × 2 dimensions.
