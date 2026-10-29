# Exercise 15. Associativity of Multiplication and Different Calculation Paths

## Given

A = ( 1  2  0 )
    ( 0  1  1 )


B = (  1   0 )
    (  2   1 )
    ( -1   3 )


C = ( 2   1 )
    ( 0  -1 )


We need to compute (AB)C and A(BC), compare the results and the number of operations, and explain the associativity of matrix multiplication.

## 1. Compute (AB)C

First, we calculate AB. Then, we multiply the result by C.

### Step 1: Calculate AB

Matrix A has size 2 × 3, and matrix B has size 3 × 2.

Since the number of columns in A equals the number of rows in B, the multiplication is defined. The result has size 2 × 2.

AB = ( 1  2  0 ) (  1   0 )
     ( 0  1  1 ) (  2   1 )
                   ( -1   3 )


**First row, first column:**

1 × 1 + 2 × 2 + 0 × (-1)

= 1 + 4 + 0

= 5


**First row, second column:**

1 × 0 + 2 × 1 + 0 × 3

= 0 + 2 + 0

= 2


**Second row, first column:**

0 × 1 + 1 × 2 + 1 × (-1)

= 0 + 2 - 1

= 1


**Second row, second column:**

0 × 0 + 1 × 1 + 1 × 3

= 0 + 1 + 3

= 4


Therefore:

AB = ( 5  2 )
     ( 1  4 )


### Step 2: Calculate (AB)C

Now, we multiply the resulting matrix AB by C.

AB = ( 5  2 )
     ( 1  4 )


C = ( 2   1 )
    ( 0  -1 )


The multiplication is defined because both matrices have size 2 × 2. The result also has size 2 × 2.

(AB)C = ( 5  2 ) ( 2   1 )
        ( 1  4 ) ( 0  -1 )


**First row, first column:**

5 × 2 + 2 × 0

= 10 + 0

= 10


**First row, second column:**

5 × 1 + 2 × (-1)

= 5 - 2

= 3


**Second row, first column:**

1 × 2 + 4 × 0

= 2 + 0

= 2


**Second row, second column:**

1 × 1 + 4 × (-1)

= 1 - 4

= -3


Therefore, the final result is:

(AB)C = ( 10   3 )
        (  2  -3 )


## 2. Compute A(BC)

Now, we follow a different calculation path. First, we calculate BC. Then, we multiply A by the result.

### Step 1: Calculate BC

Matrix B has size 3 × 2, and matrix C has size 2 × 2.

Since the number of columns in B equals the number of rows in C, the multiplication is defined. The result has size 3 × 2.

BC = (  1   0 ) ( 2   1 )
     (  2   1 ) ( 0  -1 )
     ( -1   3 )


**First row, first column:**

1 × 2 + 0 × 0

= 2 + 0

= 2


**First row, second column:**

1 × 1 + 0 × (-1)

= 1 + 0

= 1


**Second row, first column:**

2 × 2 + 1 × 0

= 4 + 0

= 4


**Second row, second column:**

2 × 1 + 1 × (-1)

= 2 - 1

= 1


**Third row, first column:**

(-1) × 2 + 3 × 0

= -2 + 0

= -2


**Third row, second column:**

(-1) × 1 + 3 × (-1)

= -1 - 3

= -4


Therefore:

BC = (  2   1 )
     (  4   1 )
     ( -2  -4 )


### Step 2: Calculate A(BC)

Now, we multiply A by the resulting matrix BC.

A = ( 1  2  0 )
    ( 0  1  1 )


BC = (  2   1 )
     (  4   1 )
     ( -2  -4 )


The multiplication is defined because A has 3 columns and BC has 3 rows. The result has size 2 × 2.

A(BC) = ( 1  2  0 ) (  2   1 )
        ( 0  1  1 ) (  4   1 )
                      ( -2  -4 )


**First row, first column:**

1 × 2 + 2 × 4 + 0 × (-2)

= 2 + 8 + 0

= 10


**First row, second column:**

1 × 1 + 2 × 1 + 0 × (-4)

= 1 + 2 + 0

= 3


**Second row, first column:**

0 × 2 + 1 × 4 + 1 × (-2)

= 0 + 4 - 2

= 2


**Second row, second column:**

0 × 1 + 1 × 1 + 1 × (-4)

= 0 + 1 - 4

= -3


Therefore, the final result is:

A(BC) = ( 10   3 )
        (  2  -3 )


## 3. Compare the results

From the first calculation path, we obtained:

(AB)C = ( 10   3 )
        (  2  -3 )


From the second calculation path, we obtained:

A(BC) = ( 10   3 )
        (  2  -3 )


Both matrices have exactly the same entries in the same positions.

Therefore:

(AB)C = A(BC)


This demonstrates the associativity of matrix multiplication.

Associativity means that when multiplying three matrices, changing the grouping of the multiplication does not change the final result, provided the products are defined.


## 4. Compare the number of operations

Although both calculation paths produce the same result, the number of arithmetic operations can be different.

### Path 1: Calculate (AB)C

First, we calculate AB.

A has size 2 × 3, and B has size 3 × 2.

To calculate the four entries of AB, each entry requires 3 multiplications and 2 additions.

Multiplications:

4 × 3 = 12

Additions:

4 × 2 = 8


Next, we calculate (AB)C.

Both matrices have size 2 × 2. Each of the four entries requires 2 multiplications and 1 addition.

Multiplications:

4 × 2 = 8

Additions:

4 × 1 = 4


Total for Path 1:

Multiplications: 12 + 8 = 20

Additions: 8 + 4 = 12


### Path 2: Calculate A(BC)

First, we calculate BC.

B has size 3 × 2, and C has size 2 × 2.

To calculate the six entries of BC, each entry requires 2 multiplications and 1 addition.

Multiplications:

6 × 2 = 12

Additions:

6 × 1 = 6


Next, we calculate A(BC).

A has size 2 × 3, and BC has size 3 × 2.

To calculate the four entries of A(BC), each entry requires 3 multiplications and 2 additions.

Multiplications:

4 × 3 = 12

Additions:

4 × 2 = 8


Total for Path 2:

Multiplications: 12 + 12 = 24

Additions: 6 + 8 = 14


### Comparison

Path 1, (AB)C:

20 multiplications and 12 additions.


Path 2, A(BC):

24 multiplications and 14 additions.


The first path uses 4 fewer multiplications and 2 fewer additions.

Therefore, calculating (AB)C requires fewer arithmetic operations for these matrices.


## Conclusion

We calculated both (AB)C and A(BC) and obtained the same result:

(AB)C = A(BC) = ( 10   3 )
                     (  2  -3 )


This confirms that matrix multiplication is associative.

However, the two calculation paths require different numbers of arithmetic operations. In this example, calculating AB first is more efficient because it requires fewer multiplications and additions.

Therefore, associativity allows us to choose the grouping that reduces the amount of computation without changing the final result.
