# Exercise 4. Matrix Multiplication and Noncommutativity

**Given:**

A = (1  2)
    (0  1)

B = (2  0)
    (3  1)

## 1. Compute AB

To multiply two matrices, we multiply each row of the first matrix by each column of the second matrix and add the products.

AB = (1  2) (2  0)
     (0  1) (3  1)

First row, first column:

1 × 2 + 2 × 3 = 2 + 6 = 8

First row, second column:

1 × 0 + 2 × 1 = 0 + 2 = 2

Second row, first column:

0 × 2 + 1 × 3 = 0 + 3 = 3

Second row, second column:

0 × 0 + 1 × 1 = 0 + 1 = 1

Therefore,

AB = (8  2)
     (3  1)

## 2. Compute BA

Now we reverse the order of the matrices.

BA = (2  0) (1  2)
     (3  1) (0  1)

First row, first column:

2 × 1 + 0 × 0 = 2 + 0 = 2

First row, second column:

2 × 2 + 0 × 1 = 4 + 0 = 4

Second row, first column:

3 × 1 + 1 × 0 = 3 + 0 = 3

Second row, second column:

3 × 2 + 1 × 1 = 6 + 1 = 7

Therefore,

BA = (2  4)
     (3  7)

## 3. Is AB = BA? Explain noncommutativity.

The results are:

AB = (8  2)
     (3  1)

BA = (2  4)
     (3  7)

The matrices are different because their corresponding entries are not all equal. For example, the top-left entries are 8 and 2.

Therefore, AB ≠ BA.

Matrix multiplication is generally not commutative. This means that changing the order of the matrices can produce a different result. In this example, multiplying A by B gives a different matrix from multiplying B by A. Therefore, matrix multiplication does not follow the commutative property of ordinary number multiplication.
