# Exercise 9. Area and the Determinant

## Given

The vectors are:

u = ( 3 )
    ( 1 )


v = ( 1 )
    ( 4 )


These two vectors span a parallelogram. We need to calculate its area using a determinant, then reverse the order of the vectors and explain what changes in the determinant and what remains unchanged in the area.

## 1. Form a matrix using the vectors

To calculate the area of a parallelogram formed by two vectors in the plane, we place the vectors as columns of a 2 × 2 matrix.

The first column is vector u, and the second column is vector v.

Therefore:

A = ( 3  1 )
    ( 1  4 )


The area of the parallelogram is the absolute value of the determinant of this matrix.

Area = |det(A)|


## 2. Calculate the determinant

For a 2 × 2 matrix, the determinant is calculated by multiplying the entries on the main diagonal and subtracting the product of the other diagonal.

The formula is:

det(A) = ad - bc


For our matrix:

A = ( 3  1 )
    ( 1  4 )


The entries are:

a = 3

b = 1

c = 1

d = 4


**Step 1: Multiply the main diagonal entries.**

3 × 4 = 12


**Step 2: Multiply the other diagonal entries.**

1 × 1 = 1


**Step 3: Subtract the second product from the first product.**

det(A) = 12 - 1

det(A) = 11


Therefore:

det(A) = 11


## 3. Calculate the area of the parallelogram

The determinant gives the signed area. The actual geometric area cannot be negative, so we take the absolute value of the determinant.

Area = |det(A)|


Substitute the determinant:

Area = |11|


Therefore:

Area = 11 square units


The area of the parallelogram formed by u and v is 11 square units.


## 4. Reverse the order of the vectors

Now, we reverse the order of the vectors and place v in the first column and u in the second column.

The new matrix is:

B = ( 1  3 )
    ( 4  1 )


We calculate its determinant.

det(B) = 1 × 1 - 3 × 4

det(B) = 1 - 12

det(B) = -11


Therefore:

det(B) = -11


## 5. Calculate the area after reversing the vectors

The area is the absolute value of the new determinant.

Area = |det(B)|


Substitute the result:

Area = |-11|


Therefore:

Area = 11 square units


The area remains unchanged even though the determinant has changed from 11 to -11.


## 6. Explain what changes and what does not change

Before reversing the vectors, we obtained:

det(A) = 11


After reversing the vectors, we obtained:

det(B) = -11


The sign of the determinant changes because exchanging the two columns of a matrix changes the sign of its determinant.

However, the area is calculated using the absolute value of the determinant.

Before reversing the vectors:

Area = |11| = 11


After reversing the vectors:

Area = |-11| = 11


Therefore, the determinant changes sign, but the area remains the same.

Geometrically, exchanging the order of the vectors reverses the orientation of the parallelogram, but it does not change its shape or size.


## Conclusion

The determinant of the matrix formed by u and v is:

det(A) = 11


The area of the parallelogram is:

Area = 11 square units


After reversing the vectors, the determinant becomes:

det(B) = -11


The area remains:

Area = 11 square units


This example demonstrates that the absolute value of a determinant gives the area of a parallelogram, while the sign of the determinant indicates its orientation.
