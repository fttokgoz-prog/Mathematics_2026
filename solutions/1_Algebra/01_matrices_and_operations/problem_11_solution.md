# Exercise 11. When Do Matrices Commute?

## Given

A = ( 1  1 )
    ( 0  1 )


B = ( a  b )
    ( c  d )


We need to find the conditions on a, b, c, and d such that AB = BA, and describe the general form of all matrices B satisfying this condition.

## 1. Compute AB

To multiply two matrices, we multiply each row of the first matrix by each column of the second matrix and add the products.

AB = ( 1  1 ) ( a  b )
     ( 0  1 ) ( c  d )


**Step 1: Calculate the first row, first column.**

1 × a + 1 × c = a + c


**Step 2: Calculate the first row, second column.**

1 × b + 1 × d = b + d


**Step 3: Calculate the second row, first column.**

0 × a + 1 × c = 0 + c = c


**Step 4: Calculate the second row, second column.**

0 × b + 1 × d = 0 + d = d


Therefore:

AB = ( a + c  b + d )
     ( c       d     )


## 2. Compute BA

Now, we reverse the order and multiply B by A.

BA = ( a  b ) ( 1  1 )
     ( c  d ) ( 0  1 )


**Step 1: Calculate the first row, first column.**

a × 1 + b × 0 = a + 0 = a


**Step 2: Calculate the first row, second column.**

a × 1 + b × 1 = a + b


**Step 3: Calculate the second row, first column.**

c × 1 + d × 0 = c + 0 = c


**Step 4: Calculate the second row, second column.**

c × 1 + d × 1 = c + d


Therefore:

BA = ( a  a + b )
     ( c  c + d )


## 3. Find the conditions for AB = BA

For AB and BA to be equal, their corresponding entries must be equal.

We have:

AB = ( a + c  b + d )
     ( c       d     )


BA = ( a  a + b )
     ( c  c + d )


We compare the corresponding entries.

**First entry:**

a + c = a

Subtract a from both sides:

c = 0


**Second entry:**

b + d = a + b

Subtract b from both sides:

d = a


**Third entry:**

c = c

This equality is always true, so it gives no additional condition.


**Fourth entry:**

d = c + d

Subtract d from both sides:

c = 0

This is the same condition we obtained from the first entry.


Therefore, the required conditions are:

c = 0

d = a


There are no additional restrictions on a or b.


## 4. Describe the general form of all matrices B

We found that:

c = 0

d = a


The original matrix B is:

B = ( a  b )
    ( c  d )


Substituting c = 0 and d = a gives:

B = ( a  b )
    ( 0  a )


Therefore, the general form of all matrices B that commute with A is:

B = ( a  b )
    ( 0  a )

where a and b can be any real numbers.


## 5. Verify the result

Using the general form:

B = ( a  b )
    ( 0  a )


Calculate AB:

AB = ( 1  1 ) ( a  b )
     ( 0  1 ) ( 0  a )


AB = ( a + 0  b + a )
     ( 0 + 0  0 + a )


AB = ( a  a + b )
     ( 0  a     )


Now calculate BA:

BA = ( a  b ) ( 1  1 )
     ( 0  a ) ( 0  1 )


BA = ( a + 0  a + b )
     ( 0 + 0  0 + a )


BA = ( a  a + b )
     ( 0  a     )


Both products are equal:

AB = BA


This confirms that every matrix of the form

B = ( a  b )
    ( 0  a )

commutes with A.


## Conclusion

The matrices A and B commute when AB = BA.

Comparing the entries of the two products gives the conditions c = 0 and d = a. There are no restrictions on a and b.

Therefore, all matrices B that commute with A have the form:

B = ( a  b )
    ( 0  a )

where a and b are arbitrary real numbers.
