
# EXERCISE 7 – CHOOSING A METHOD DELIBERATELY

## Given

Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice.

### Case 1 – Triangular Coefficient Matrix

Given the system:

$$
\begin{cases}
2x-y=3\\
4y=8
\end{cases}
$$

### Case 2 – Three Systems with the Same Invertible Matrix

Consider three systems:

$$
Ax=b_1,\qquad Ax=b_2,\qquad Ax=b_3
$$

The matrix A is invertible, and its inverse A^(-1) is already known.

### Case 3 – One 3x3 System

Consider one 3x3 system where the inverse matrix is not given and the goal is only to find one solution vector.

For Case 1, carry out the chosen method completely. For Cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary.

Do not judge a method by its name alone. Refer to the number of right-hand sides and the structure of the matrix.

## Solution

### Case 1 – Triangular Coefficient Matrix

**Chosen method: Back Substitution**

The coefficient matrix is triangular because the second equation contains only y.

Therefore, back substitution is the most suitable method.

Start with the second equation:

$$
4y=8
$$

Divide both sides by 4:

$$
y=2
$$

Now substitute y = 2 into the first equation:

$$
2x-y=3
$$

$$
2x-2=3
$$

Add 2 to both sides:

$$
2x=5
$$

Divide both sides by 2:

$$
x=\frac{5}{2}
$$

**Final Answer:**

$$
x=\frac{5}{2},\qquad y=2
$$

Back substitution is efficient here because the value of y can be found directly from the last equation, and then used to calculate x.

### Case 2 – Three Systems with the Same Invertible Matrix

**Chosen method: Using the Known Inverse Matrix**

We are given three systems:

$$
Ax=b_1
$$

$$
Ax=b_2
$$

$$
Ax=b_3
$$

Since A is invertible and A^(-1) is already known, we can multiply each equation by A^(-1) from the left.

For the first system:

$$
A^{-1}Ax=A^{-1}b_1
$$

Therefore:

$$
x_1=A^{-1}b_1
$$

Similarly, for the other two systems:

$$
x_2=A^{-1}b_2
$$

$$
x_3=A^{-1}b_3
$$

**What can be reused?**

The inverse matrix A^(-1) is the same for all three systems, so it only needs to be calculated once.

The only new calculation for each system is multiplying A^(-1) by its corresponding right-hand side vector.

There is no need to calculate the inverse again or repeat Gaussian elimination for each system.

### Case 3 – One 3x3 System

**Chosen method: Gaussian Elimination**

For one 3x3 system where the inverse matrix is not given and only one solution is required, Gaussian elimination is a suitable method.

The plan is:

1. Write the augmented matrix [A | b].
2. Use elementary row operations to transform the matrix into row echelon form.
3. Use back substitution to find the unknown variables.

**Why is this method suitable?**

We only need one solution vector, so calculating the entire inverse matrix would be unnecessary extra work.

Gaussian elimination works directly with the given equations and finds the required solution without calculating A^(-1).

There is no need to calculate the inverse matrix or solve additional systems with the same coefficient matrix.

### Final Comparison

| Case | Chosen method | Reason |
|---|---|---|
| Case 1 | Back substitution | The coefficient matrix is triangular. |
| Case 2 | Known inverse matrix | The same inverse can be reused for three right-hand sides. |
| Case 3 | Gaussian elimination | Only one solution is required, so calculating the inverse is unnecessary. |

### Conclusion

The best method depends on the structure of the matrix and the number of right-hand sides.

For a triangular system, back substitution is efficient.

When several systems share the same invertible coefficient matrix, the known inverse can be reused.

For a single system where only one solution is needed, Gaussian elimination avoids the unnecessary calculation of the inverse matrix.
