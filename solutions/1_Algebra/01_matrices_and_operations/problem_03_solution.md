# Exercise 3. When Can Matrices Be Multiplied?

Given:

A has size 2 × 3.

B has size 3 × 4.

C has size 4 × 2.

D has size 2 × 2.

The rule for matrix multiplication is that the number of columns in the first matrix must be equal to the number of rows in the second matrix.

If the sizes are (m × n) and (n × p), multiplication is possible and the result has size (m × p).

## 1. AB

A has size 2 × 3.

B has size 3 × 4.

The number of columns in A is 3, and the number of rows in B is 3.

Since 3 = 3, multiplication is possible.

Result size: 2 × 4.

Answer: AB is defined, and its size is 2 × 4.

## 2. BA

B has size 3 × 4.

A has size 2 × 3.

The number of columns in B is 4, and the number of rows in A is 2.

Since 4 ≠ 2, multiplication is not possible.

Answer: BA is not defined.

## 3. BC

B has size 3 × 4.

C has size 4 × 2.

The number of columns in B is 4, and the number of rows in C is 4.

Since 4 = 4, multiplication is possible.

Result size: 3 × 2.

Answer: BC is defined, and its size is 3 × 2.

## 4. CB

C has size 4 × 2.

B has size 3 × 4.

The number of columns in C is 2, and the number of rows in B is 3.

Since 2 ≠ 3, multiplication is not possible.

Answer: CB is not defined.

## 5. AC

A has size 2 × 3.

C has size 4 × 2.

The number of columns in A is 3, and the number of rows in C is 4.

Since 3 ≠ 4, multiplication is not possible.

Answer: AC is not defined.

## 6. CA

C has size 4 × 2.

A has size 2 × 3.

The number of columns in C is 2, and the number of rows in A is 2.

Since 2 = 2, multiplication is possible.

Result size: 4 × 3.

Answer: CA is defined, and its size is 4 × 3.

## 7. AD

A has size 2 × 3.

D has size 2 × 2.

The number of columns in A is 3, and the number of rows in D is 2.

Since 3 ≠ 2, multiplication is not possible.

Answer: AD is not defined.

## 8. DA

D has size 2 × 2.

A has size 2 × 3.

The number of columns in D is 2, and the number of rows in A is 2.

Since 2 = 2, multiplication is possible.

Result size: 2 × 3.

Answer: DA is defined, and its size is 2 × 3.

## Conclusion

Matrix multiplication is defined only when the number of columns in the first matrix equals the number of rows in the second matrix. The size of the result is determined by the number of rows in the first matrix and the number of columns in the second matrix.
