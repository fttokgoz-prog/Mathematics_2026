# Exercise 10. Columns of a Matrix Product

## Given

A = ( 1  2  0 )
    ( 0  1  1 )


B = (  1   2 )
    ( -1   0 )
    (  3   1 )


Let b₁ and b₂ denote the first and second columns of matrix B.

The first column is:

b₁ = (  1 )
     ( -1 )
     (  3 )


The second column is:

b₂ = ( 2 )
     ( 0 )
     ( 1 )


## 1. Compute Ab₁ and Ab₂

### Step 1: Compute Ab₁

We multiply matrix A by the first column of B.

Ab₁ = ( 1  2  0 ) (  1 )
      ( 0  1  1 ) ( -1 )
                    (  3 )


To calculate the first entry, multiply the first row of A by b₁ and add the products:

1 × 1 + 2 × (-1) + 0 × 3

= 1 - 2 + 0

= -1


To calculate the second entry, multiply the second row of A by b₁ and add the products:

0 × 1 + 1 × (-1) + 1 × 3

= 0 - 1 + 3

= 2


Therefore:

Ab₁ = ( -1 )
      (  2 )


### Step 2: Compute Ab₂

We multiply matrix A by the second column of B.

Ab₂ = ( 1  2  0 ) ( 2 )
      ( 0  1  1 ) ( 0 )
                    ( 1 )


To calculate the first entry:

1 × 2 + 2 × 0 + 0 × 1

= 2 + 0 + 0

= 2


To calculate the second entry:

0 × 2 + 1 × 0 + 1 × 1

= 0 + 0 + 1

= 1


Therefore:

Ab₂ = ( 2 )
      ( 1 )


## 2. Compute the matrix AB

To multiply matrices A and B, we multiply each row of A by each column of B.

Matrix A has size 2 × 3, and matrix B has size 3 × 2. Since the number of columns in A equals the number of rows in B, the multiplication is defined.

The result will have size 2 × 2.

AB = ( 1  2  0 ) (  1   2 )
     ( 0  1  1 ) ( -1   0 )
                   (  3   1 )


### Step 1: Calculate the first row, first column

1 × 1 + 2 × (-1) + 0 × 3

= 1 - 2 + 0

= -1


### Step 2: Calculate the first row, second column

1 × 2 + 2 × 0 + 0 × 1

= 2 + 0 + 0

= 2


### Step 3: Calculate the second row, first column

0 × 1 + 1 × (-1) + 1 × 3

= 0 - 1 + 3

= 2


### Step 4: Calculate the second row, second column

0 × 2 + 1 × 0 + 1 × 1

= 0 + 0 + 1

= 1


Therefore, the final matrix is:

AB = ( -1   2 )
     (  2   1 )


## 3. Compare the results and explain why the columns of AB are Ab₁ and Ab₂

From the first part, we calculated:

Ab₁ = ( -1 )
      (  2 )


Ab₂ = ( 2 )
      ( 1 )


From the second part, we calculated:

AB = ( -1   2 )
     (  2   1 )


The first column of AB is (-1, 2), which is exactly Ab₁.

The second column of AB is (2, 1), which is exactly Ab₂.

Therefore, the columns of AB are:

First column = Ab₁

Second column = Ab₂


**Explanation:**

When multiplying A by B, each column of B is multiplied by A separately. The result of multiplying A by a column of B becomes the corresponding column of the product AB.

Since b₁ is the first column of B, Ab₁ becomes the first column of AB.

Since b₂ is the second column of B, Ab₂ becomes the second column of AB.

This explains why the columns of AB are exactly Ab₁ and Ab₂.


## Conclusion

We obtained:

Ab₁ = (-1, 2)

Ab₂ = (2, 1)

AB = ( -1   2 )
     (  2   1 )

The results confirm that each column of the matrix product AB is obtained by multiplying A by the corresponding column of B.
