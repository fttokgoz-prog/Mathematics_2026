# Exercise 12. Formula for a Matrix Power

## Given

A = ( 1  1 )
    ( 0  1 )


We need to compute A², A³, and A⁴, find a general formula for Aⁿ, and prove the formula using mathematical induction.

## 1. Compute A²

The notation A² means multiplying A by itself.

A² = A × A

A² = ( 1  1 ) ( 1  1 )
     ( 0  1 ) ( 0  1 )


**Step 1: Calculate the first row, first column.**

1 × 1 + 1 × 0 = 1 + 0 = 1


**Step 2: Calculate the first row, second column.**

1 × 1 + 1 × 1 = 1 + 1 = 2


**Step 3: Calculate the second row, first column.**

0 × 1 + 1 × 0 = 0 + 0 = 0


**Step 4: Calculate the second row, second column.**

0 × 1 + 1 × 1 = 0 + 1 = 1


Therefore:

A² = ( 1  2 )
     ( 0  1 )


## 2. Compute A³

The notation A³ means multiplying A² by A.

A³ = A² × A

A³ = ( 1  2 ) ( 1  1 )
     ( 0  1 ) ( 0  1 )


**Step 1: Calculate the first row, first column.**

1 × 1 + 2 × 0 = 1 + 0 = 1


**Step 2: Calculate the first row, second column.**

1 × 1 + 2 × 1 = 1 + 2 = 3


**Step 3: Calculate the second row, first column.**

0 × 1 + 1 × 0 = 0 + 0 = 0


**Step 4: Calculate the second row, second column.**

0 × 1 + 1 × 1 = 0 + 1 = 1


Therefore:

A³ = ( 1  3 )
     ( 0  1 )


## 3. Compute A⁴

The notation A⁴ means multiplying A³ by A.

A⁴ = A³ × A

A⁴ = ( 1  3 ) ( 1  1 )
     ( 0  1 ) ( 0  1 )


**Step 1: Calculate the first row, first column.**

1 × 1 + 3 × 0 = 1 + 0 = 1


**Step 2: Calculate the first row, second column.**

1 × 1 + 3 × 1 = 1 + 3 = 4


**Step 3: Calculate the second row, first column.**

0 × 1 + 1 × 0 = 0 + 0 = 0


**Step 4: Calculate the second row, second column.**

0 × 1 + 1 × 1 = 0 + 1 = 1


Therefore:

A⁴ = ( 1  4 )
     ( 0  1 )


## 4. Formulate a conjecture for Aⁿ

We have calculated the following powers:

A² = ( 1  2 )
     ( 0  1 )


A³ = ( 1  3 )
     ( 0  1 )


A⁴ = ( 1  4 )
     ( 0  1 )


We can observe a pattern:

- The top-left entry is always 1.
- The bottom-left entry is always 0.
- The bottom-right entry is always 1.
- The top-right entry is equal to the exponent n.

For A², the top-right entry is 2.

For A³, the top-right entry is 3.

For A⁴, the top-right entry is 4.

Therefore, we conjecture that for every positive integer n:

Aⁿ = ( 1  n )
     ( 0  1 )


## 5. Prove the formula using mathematical induction

We want to prove that:

Aⁿ = ( 1  n )
     ( 0  1 )

for every positive integer n.

**Step 1: Base case**

For n = 1, the formula gives:

A¹ = ( 1  1 )
     ( 0  1 )

This is exactly the original matrix A.

Therefore, the formula is true for n = 1.


**Step 2: Inductive hypothesis**

Assume that the formula is true for some positive integer n.

This means we assume:

Aⁿ = ( 1  n )
     ( 0  1 )

We must show that the formula is also true for n + 1.


**Step 3: Multiply Aⁿ by A**

By the definition of matrix powers:

Aⁿ⁺¹ = Aⁿ × A

Using the inductive hypothesis:

Aⁿ⁺¹ = ( 1  n ) ( 1  1 )
       ( 0  1 ) ( 0  1 )


**Step 4: Calculate each entry**

First row, first column:

1 × 1 + n × 0 = 1 + 0 = 1


First row, second column:

1 × 1 + n × 1 = 1 + n = n + 1


Second row, first column:

0 × 1 + 1 × 0 = 0 + 0 = 0


Second row, second column:

0 × 1 + 1 × 1 = 0 + 1 = 1


Therefore:

Aⁿ⁺¹ = ( 1  n + 1 )
       ( 0    1   )


This is exactly the same formula with n replaced by n + 1.


**Step 5: Complete the proof**

We have shown that the formula is true for n = 1.

We have also shown that if the formula is true for n, then it is true for n + 1.

Therefore, by mathematical induction, the formula holds for every positive integer n:

Aⁿ = ( 1  n )
     ( 0  1 )


## Conclusion

The calculations of A², A³, and A⁴ reveal a clear pattern in which the top-right entry equals the exponent n.

Using mathematical induction, we proved that this pattern continues for every positive integer n.

The general formula is:

Aⁿ = ( 1  n )
     ( 0  1 )
