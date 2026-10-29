# Exercise 14. A System of Equations and the Determinant

## Given

Consider the system of equations:

Ax = b

where

A = ( 1  2 )
    ( k  4 )


We need to determine the values of k for which the system has exactly one solution for every right-hand side b.

For the remaining value of k, we must give an example of a right-hand side b for which the system has infinitely many solutions and an example for which it has no solution.

## 1. Calculate the determinant of A

The coefficient matrix is:

A = ( 1  2 )
    ( k  4 )


For a 2 × 2 matrix, the determinant is calculated using the formula:

det(A) = ad - bc


In this matrix:

a = 1

b = 2

c = k

d = 4


Substitute these values into the formula:

det(A) = 1 × 4 - 2 × k


Calculate the products:

det(A) = 4 - 2k


Therefore:

det(A) = 4 - 2k


## 2. Find the values of k for which the system has exactly one solution for every b

A square linear system Ax = b has exactly one solution for every right-hand side b if its coefficient matrix A is invertible.

A matrix is invertible if and only if its determinant is nonzero.

Therefore, we require:

det(A) ≠ 0


Substitute the determinant:

4 - 2k ≠ 0


Subtract 4 from both sides:

-2k ≠ -4


Divide both sides by -2:

k ≠ 2


Therefore, the system has exactly one solution for every b when:

k ≠ 2


For these values, the inverse matrix A⁻¹ exists, so the unique solution can be written as:

x = A⁻¹b


## 3. Examine the remaining value k = 2

The only remaining value is:

k = 2


Substitute this value into the coefficient matrix:

A = ( 1  2 )
    ( 2  4 )


The second row is twice the first row:

R₂ = 2R₁


The determinant is:

det(A) = 4 - 2(2)

det(A) = 4 - 4

det(A) = 0


Therefore, the matrix is not invertible.

For this value of k, the system does not have exactly one solution for every b. Depending on the right-hand side, it can have either infinitely many solutions or no solution.

## 4. Give an example with infinitely many solutions

Choose the right-hand side:

b = ( 3 )
    ( 6 )


When k = 2, the system Ax = b becomes:

x₁ + 2x₂ = 3

2x₁ + 4x₂ = 6


The second equation is exactly twice the first equation.

Multiply the first equation by 2:

2x₁ + 4x₂ = 6


This is identical to the second equation. Therefore, the two equations represent the same line and provide only one independent equation.

We can solve the first equation for x₁:

x₁ + 2x₂ = 3


Subtract 2x₂ from both sides:

x₁ = 3 - 2x₂


Let x₂ = t, where t can be any real number.

Then:

x₁ = 3 - 2t

x₂ = t


Therefore, the solutions are:

x = ( 3 - 2t )
    (     t   )


where t ∈ ℝ.

Since t can take infinitely many real values, the system has infinitely many solutions.

**Example of a right-hand side with infinitely many solutions:**

b = ( 3 )
    ( 6 )


## 5. Give an example with no solution

Now choose a different right-hand side:

b = ( 3 )
    ( 7 )


When k = 2, the system becomes:

x₁ + 2x₂ = 3

2x₁ + 4x₂ = 7


Multiply the first equation by 2:

2x₁ + 4x₂ = 6


However, the second equation requires:

2x₁ + 4x₂ = 7


The same expression cannot equal both 6 and 7.

Subtracting the doubled first equation from the second equation gives:

(2x₁ + 4x₂) - (2x₁ + 4x₂) = 7 - 6


Simplify:

0 = 1


This is a contradiction, so the system has no solution.

**Example of a right-hand side with no solution:**

b = ( 3 )
    ( 7 )


## 6. Explain the relationship between the determinant and the number of solutions

The determinant of the coefficient matrix is:

det(A) = 4 - 2k


There are two cases.

**Case 1: k ≠ 2**

The determinant is nonzero:

det(A) ≠ 0


The matrix is invertible, so the system has exactly one solution for every b.


**Case 2: k = 2**

The determinant is zero:

det(A) = 0


The matrix is not invertible, and its rows are linearly dependent.

In this case, the system can have infinitely many solutions if the equations are consistent, or no solution if the equations are inconsistent.

For example:

b = (3, 6) gives infinitely many solutions.

b = (3, 7) gives no solution.


## Conclusion

The determinant of the coefficient matrix is:

det(A) = 4 - 2k


The system has exactly one solution for every b when:

k ≠ 2


When k = 2, the determinant is zero and the matrix is not invertible.

For b = (3, 6), the system has infinitely many solutions because the two equations represent the same line.

For b = (3, 7), the system has no solution because the equations contradict each other.

This example demonstrates that a nonzero determinant guarantees a unique solution for every right-hand side, while a zero determinant allows either infinitely many solutions or no solution, depending on b.
