# Exercise 3. Matrix Multiplication and Dimensions

## Question

Given the matrices

A = ( 1  2  0 )
    ( 0  1  1 )

B = (  1   0 )
    (  2   1 )
    ( -1   3 )

C = ( 2  1 )
    ( 0  1 )

Determine which of the following matrix products are defined. For each product that is defined, calculate the result.

1. AB
2. BA
3. AC
4. CA
5. AᵀB
6. ABᵀ
7. BC
8. CB

Explain the dimension rule for matrix multiplication.

## Solution

### Part 1. Understand the matrix multiplication rule

Before calculating the products, we must determine whether each multiplication is defined.

If matrix X has dimensions m × n and matrix Y has dimensions p × q, the product XY is defined only when:

n = p

In other words, the number of columns in the first matrix must equal the number of rows in the second matrix.

When the multiplication is defined, the resulting matrix has dimensions:

(m × n)(n × q) = m × q

The inner dimensions must match, while the outer dimensions determine the size of the result.

For the matrices in this exercise:

A has dimensions 2 × 3.

B has dimensions 3 × 2.

C has dimensions 2 × 2.

The transpose of a matrix exchanges its rows and columns. Therefore:

Aᵀ has dimensions 3 × 2.

Bᵀ has dimensions 2 × 3.

We will use these dimensions to check all eight products.

### Part 2. Calculate AB

**Step 1: Check the dimensions.**

A has dimensions 2 × 3.

B has dimensions 3 × 2.

The number of columns in A is 3, and the number of rows in B is also 3.

Therefore, AB is defined.

The resulting matrix has dimensions:

(2 × 3)(3 × 2) = 2 × 2

**Step 2: Write the multiplication.**

AB = ( 1  2  0 ) (  1   0 )
     ( 0  1  1 ) (  2   1 )
                   ( -1   3 )

**Step 3: Calculate the first row, first column.**

Multiply the first row of A by the first column of B:

1 × 1 + 2 × 2 + 0 × (-1)

= 1 + 4 + 0

= 5

**Step 4: Calculate the first row, second column.**

Multiply the first row of A by the second column of B:

1 × 0 + 2 × 1 + 0 × 3

= 0 + 2 + 0

= 2

**Step 5: Calculate the second row, first column.**

Multiply the second row of A by the first column of B:

0 × 1 + 1 × 2 + 1 × (-1)

= 0 + 2 - 1

= 1

**Step 6: Calculate the second row, second column.**

Multiply the second row of A by the second column of B:

0 × 0 + 1 × 1 + 1 × 3

= 0 + 1 + 3

= 4

**Final result:**

AB = ( 5  2 )
     ( 1  4 )

### Part 3. Calculate BA

**Step 1: Check the dimensions.**

B has dimensions 3 × 2.

A has dimensions 2 × 3.

The number of columns in B is 2, and the number of rows in A is also 2.

Therefore, BA is defined.

The resulting matrix has dimensions:

(3 × 2)(2 × 3) = 3 × 3

**Step 2: Write the multiplication.**

BA = (  1   0 ) ( 1  2  0 )
     (  2   1 ) ( 0  1  1 )
     ( -1   3 )

**Step 3: Calculate the first row.**

First entry:

1 × 1 + 0 × 0 = 1

Second entry:

1 × 2 + 0 × 1 = 2

Third entry:

1 × 0 + 0 × 1 = 0

The first row is:

(1, 2, 0)

**Step 4: Calculate the second row.**

First entry:

2 × 1 + 1 × 0 = 2

Second entry:

2 × 2 + 1 × 1 = 4 + 1 = 5

Third entry:

2 × 0 + 1 × 1 = 1

The second row is:

(2, 5, 1)

**Step 5: Calculate the third row.**

First entry:

(-1) × 1 + 3 × 0 = -1

Second entry:

(-1) × 2 + 3 × 1 = -2 + 3 = 1

Third entry:

(-1) × 0 + 3 × 1 = 3

The third row is:

(-1, 1, 3)

**Final result:**

BA = (  1   2   0 )
     (  2   5   1 )
     ( -1   1   3 )

Notice that AB is 2 × 2, while BA is 3 × 3. Both products are defined, but they have different dimensions.

### Part 4. Calculate AC

**Step 1: Check the dimensions.**

A has dimensions 2 × 3.

C has dimensions 2 × 2.

The number of columns in A is 3, but the number of rows in C is 2.

Since 3 ≠ 2, the inner dimensions do not match.

Therefore:

**AC is not defined.**

No multiplication can be performed because each row of A would need to be multiplied by a column of C, but the numbers of corresponding entries would not match.

### Part 5. Calculate CA

**Step 1: Check the dimensions.**

C has dimensions 2 × 2.

A has dimensions 2 × 3.

The number of columns in C is 2, and the number of rows in A is also 2.

Therefore, CA is defined.

The resulting matrix has dimensions:

(2 × 2)(2 × 3) = 2 × 3

**Step 2: Write the multiplication.**

CA = ( 2  1 ) ( 1  2  0 )
     ( 0  1 ) ( 0  1  1 )

**Step 3: Calculate the first row.**

First entry:

2 × 1 + 1 × 0 = 2

Second entry:

2 × 2 + 1 × 1 = 4 + 1 = 5

Third entry:

2 × 0 + 1 × 1 = 1

The first row is:

(2, 5, 1)

**Step 4: Calculate the second row.**

First entry:

0 × 1 + 1 × 0 = 0

Second entry:

0 × 2 + 1 × 1 = 1

Third entry:

0 × 0 + 1 × 1 = 1

The second row is:

(0, 1, 1)

**Final result:**

CA = ( 2  5  1 )
     ( 0  1  1 )

### Part 6. Calculate AᵀB

**Step 1: Determine the dimensions of Aᵀ.**

The original matrix A has dimensions 2 × 3.

Transposing a matrix exchanges its rows and columns.

Therefore:

Aᵀ has dimensions 3 × 2.

The transpose is:

Aᵀ = ( 1  0 )
     ( 2  1 )
     ( 0  1 )

**Step 2: Check the dimensions of AᵀB.**

Aᵀ has dimensions 3 × 2.

B has dimensions 3 × 2.

The number of columns in Aᵀ is 2, but the number of rows in B is 3.

Since 2 ≠ 3, the multiplication is not defined.

Therefore:

**AᵀB is not defined.**

### Part 7. Calculate ABᵀ

**Step 1: Determine the dimensions of Bᵀ.**

The original matrix B has dimensions 3 × 2.

After transposing, its dimensions become 2 × 3.

The transpose is:

Bᵀ = ( 1   2  -1 )
     ( 0   1   3 )

**Step 2: Check the dimensions.**

A has dimensions 2 × 3.

Bᵀ has dimensions 2 × 3.

The number of columns in A is 3, but the number of rows in Bᵀ is 2.

Since 3 ≠ 2, the multiplication is not defined.

Therefore:

**ABᵀ is not defined.**

### Part 8. Calculate BC

**Step 1: Check the dimensions.**

B has dimensions 3 × 2.

C has dimensions 2 × 2.

The number of columns in B is 2, and the number of rows in C is also 2.

Therefore, BC is defined.

The resulting matrix has dimensions:

(3 × 2)(2 × 2) = 3 × 2

**Step 2: Write the multiplication.**

BC = (  1   0 ) ( 2  1 )
     (  2   1 ) ( 0  1 )
     ( -1   3 )

**Step 3: Calculate the first row.**

First entry:

1 × 2 + 0 × 0 = 2

Second entry:

1 × 1 + 0 × 1 = 1

The first row is:

(2, 1)

**Step 4: Calculate the second row.**

First entry:

2 × 2 + 1 × 0 = 4

Second entry:

2 × 1 + 1 × 1 = 2 + 1 = 3

The second row is:

(4, 3)

**Step 5: Calculate the third row.**

First entry:

(-1) × 2 + 3 × 0 = -2

Second entry:

(-1) × 1 + 3 × 1 = -1 + 3 = 2

The third row is:

(-2, 2)

**Final result:**

BC = (  2   1 )
     (  4   3 )
     ( -2   2 )

### Part 9. Calculate CB

**Step 1: Check the dimensions.**

C has dimensions 2 × 2.

B has dimensions 3 × 2.

The number of columns in C is 2, but the number of rows in B is 3.

Since 2 ≠ 3, the multiplication is not defined.

Therefore:

**CB is not defined.**

## Final Answers

1. AB is defined.

   AB = ( 5  2 )
        ( 1  4 )

2. BA is defined.

   BA = (  1   2   0 )
        (  2   5   1 )
        ( -1   1   3 )

3. AC is not defined because the inner dimensions are 3 and 2.

4. CA is defined.

   CA = ( 2  5  1 )
        ( 0  1  1 )

5. AᵀB is not defined because the inner dimensions are 2 and 3.

6. ABᵀ is not defined because the inner dimensions are 3 and 2.

7. BC is defined.

   BC = (  2   1 )
        (  4   3 )
        ( -2   2 )

8. CB is not defined because the inner dimensions are 2 and 3.

## Explanation of the Method

Matrix multiplication is possible only when the number of columns in the first matrix equals the number of rows in the second matrix.

If the product is defined, the result has the number of rows of the first matrix and the number of columns of the second matrix.

For every defined product, each entry is calculated by multiplying a row of the first matrix by a column of the second matrix and adding the products.

The order of multiplication matters. For example, AB is a 2 × 2 matrix, whereas BA is a 3 × 3 matrix. Both are defined, but they are not the same product and do not even have the same dimensions.
