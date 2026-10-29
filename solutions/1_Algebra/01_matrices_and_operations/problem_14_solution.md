# Exercise 14. Rotation Matrices

## Given

The matrix for a rotation through an angle θ is:

R(θ) = ( cos θ   -sin θ )
       ( sin θ    cos θ )


We need to compute R(α)R(β) and use the angle-sum formulas for sine and cosine to show that:

R(α)R(β) = R(α + β)

We will also explain the geometrical meaning of this result.

## 1. Write the rotation matrices

For an angle α:

R(α) = ( cos α   -sin α )
       ( sin α    cos α )


For an angle β:

R(β) = ( cos β   -sin β )
       ( sin β    cos β )


## 2. Compute R(α)R(β)

We multiply the two matrices using the row-by-column method.

R(α)R(β) = ( cos α   -sin α ) ( cos β   -sin β )
           ( sin α    cos α ) ( sin β    cos β )


**Step 1: Calculate the first row, first column.**

Multiply the first row of R(α) by the first column of R(β).

cos α × cos β + (-sin α) × sin β

= cos α cos β - sin α sin β


**Step 2: Calculate the first row, second column.**

Multiply the first row of R(α) by the second column of R(β).

cos α × (-sin β) + (-sin α) × cos β

= -cos α sin β - sin α cos β

= -(cos α sin β + sin α cos β)


**Step 3: Calculate the second row, first column.**

Multiply the second row of R(α) by the first column of R(β).

sin α × cos β + cos α × sin β

= sin α cos β + cos α sin β


**Step 4: Calculate the second row, second column.**

Multiply the second row of R(α) by the second column of R(β).

sin α × (-sin β) + cos α × cos β

= -sin α sin β + cos α cos β

= cos α cos β - sin α sin β


Therefore, the product is:

R(α)R(β) = ( cos α cos β - sin α sin β        -(cos α sin β + sin α cos β) )
           ( sin α cos β + cos α sin β          cos α cos β - sin α sin β    )


## 3. Use the angle-sum formulas

To simplify the result, we use the standard trigonometric identities.

The cosine angle-sum formula is:

cos(α + β) = cos α cos β - sin α sin β


The sine angle-sum formula is:

sin(α + β) = sin α cos β + cos α sin β


Now, we substitute these identities into the matrix obtained above.

**First row, first column:**

cos α cos β - sin α sin β = cos(α + β)


**First row, second column:**

-(cos α sin β + sin α cos β) = -sin(α + β)


**Second row, first column:**

sin α cos β + cos α sin β = sin(α + β)


**Second row, second column:**

cos α cos β - sin α sin β = cos(α + β)


After substitution, the matrix becomes:

R(α)R(β) = ( cos(α + β)   -sin(α + β) )
           ( sin(α + β)    cos(α + β) )


This is exactly the definition of the rotation matrix R(α + β).

Therefore:

R(α)R(β) = R(α + β)


## 4. Explain the result geometrically

A rotation matrix rotates a vector around the origin by a specified angle.

First, applying R(β) rotates a vector by angle β.

Then, applying R(α) rotates the resulting vector by angle α.

The total rotation is the sum of the two angles:

β + α = α + β


Therefore, performing two consecutive rotations is equivalent to performing one rotation through the combined angle α + β.

The matrix product represents these two consecutive transformations, which explains why:

R(α)R(β) = R(α + β)


## Conclusion

By multiplying the two rotation matrices and applying the angle-sum formulas for sine and cosine, we obtain:

R(α)R(β) = R(α + β)

This shows that the product of two rotation matrices represents a rotation through the sum of their angles.

Geometrically, two consecutive rotations around the same origin are equivalent to a single rotation by the combined angle.
