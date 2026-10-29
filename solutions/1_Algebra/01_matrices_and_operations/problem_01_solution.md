# Exercise 1. Matrix Size and Entries

## Question

Given the matrices

A = ( 2  -1   3 )
    ( 0   4   5 )

B = (  1   0 )
    ( -2   3 )
    (  4   1 )

Answer the following questions:

1. State the sizes of matrices A and B.

2. Identify the entries a₁₂, a₂₃, b₂₁, and b₃₂.

3. Write the second row of A and the first column of B as vectors.

## Solution

### Part 1. Determine the sizes of matrices A and B

The size or dimension of a matrix is determined by counting its rows and columns.

The general notation for the size of a matrix is:

m × n

where:

- m represents the number of rows.
- n represents the number of columns.

The number of rows is counted horizontally, and the number of columns is counted vertically.

**Step 1: Determine the size of matrix A.**

The given matrix is:

A = ( 2  -1   3 )
    ( 0   4   5 )

First, count the rows.

The first row is (2, -1, 3).

The second row is (0, 4, 5).

Therefore, matrix A has 2 rows.

Next, count the columns.

The first column contains 2 and 0.

The second column contains -1 and 4.

The third column contains 3 and 5.

Therefore, matrix A has 3 columns.

Using the formula for matrix dimensions:

Size of A = number of rows × number of columns

Size of A = 2 × 3

Therefore, matrix A has size **2 × 3**.

**Step 2: Determine the size of matrix B.**

The given matrix is:

B = (  1   0 )
    ( -2   3 )
    (  4   1 )

First, count the rows.

The first row is (1, 0).

The second row is (-2, 3).

The third row is (4, 1).

Therefore, matrix B has 3 rows.

Next, count the columns.

The first column contains 1, -2, and 4.

The second column contains 0, 3, and 1.

Therefore, matrix B has 2 columns.

Using the formula:

Size of B = number of rows × number of columns

Size of B = 3 × 2

Therefore, matrix B has size **3 × 2**.

**Result of Part 1:**

A has size 2 × 3.

B has size 3 × 2.

The order is important because matrix dimensions are always written as rows first and columns second.

### Part 2. Identify the requested matrix entries

Matrix entries are identified using two indices.

The general notation is:

aᵢⱼ

where:

- The first index, i, indicates the row.
- The second index, j, indicates the column.

Therefore, aᵢⱼ means the entry located in row i and column j.

The same rule applies to the entries of matrix B, written as bᵢⱼ.

**Step 1: Find a₁₂.**

The notation a₁₂ means:

Row = 1

Column = 2

Matrix A is:

A = ( 2  -1   3 )
    ( 0   4   5 )

The first row contains:

2, -1, 3

The second entry in this row is -1.

Therefore:

a₁₂ = -1

**Step 2: Find a₂₃.**

The notation a₂₃ means:

Row = 2

Column = 3

The second row of A is:

(0, 4, 5)

The third entry in this row is 5.

Therefore:

a₂₃ = 5

**Step 3: Find b₂₁.**

The notation b₂₁ means:

Row = 2

Column = 1

Matrix B is:

B = (  1   0 )
    ( -2   3 )
    (  4   1 )

The second row is:

(-2, 3)

The first entry in this row is -2.

Therefore:

b₂₁ = -2

**Step 4: Find b₃₂.**

The notation b₃₂ means:

Row = 3

Column = 2

The third row of B is:

(4, 1)

The second entry in this row is 1.

Therefore:

b₃₂ = 1

**Result of Part 2:**

a₁₂ = -1

a₂₃ = 5

b₂₁ = -2

b₃₂ = 1

Each entry was identified by first locating the correct row and then selecting the required column.

### Part 3. Write the second row of A and the first column of B as vectors

A vector is an ordered list of numbers. Depending on how its entries are arranged, it can be written as a row vector or a column vector.

A row vector has one row and several columns.

A column vector has several rows and one column.

**Step 1: Write the second row of A as a vector.**

The matrix is:

A = ( 2  -1   3 )
    ( 0   4   5 )

The second row contains the entries:

0, 4, 5

Writing these entries in the same order gives the row vector:

r₂ = (0, 4, 5)

The order of the entries must remain unchanged because each number occupies a specific position in the original row.

Therefore, the second row of A is:

**(0, 4, 5)**

**Step 2: Write the first column of B as a vector.**

The matrix is:

B = (  1   0 )
    ( -2   3 )
    (  4   1 )

The first column contains the entries:

1, -2, 4

A column vector is written vertically, so these entries become:

c₁ = (  1 )
     ( -2 )
     (  4 )

The entries remain in the same top-to-bottom order as in matrix B.

Therefore, the first column of B is:

**(1, -2, 4)ᵀ**

The superscript T indicates that the entries are arranged as a column vector rather than a row vector.

## Final Answers

**1. Matrix dimensions**

A is a 2 × 3 matrix.

B is a 3 × 2 matrix.

**2. Requested entries**

a₁₂ = -1

a₂₃ = 5

b₂₁ = -2

b₃₂ = 1

**3. Requested vectors**

The second row of A is:

(0, 4, 5)

The first column of B is:

(1, -2, 4)ᵀ

## Explanation of the Method

Matrix dimensions are found by counting rows and columns, always writing the number of rows first.

Matrix entries are identified using two indices: the first specifies the row, and the second specifies the column.

Rows and columns can also be represented as vectors. A row is written horizontally, while a column is written vertically. In both cases, the original order of the entries must be preserved.
