
# EXERCISE 3
# WHEN CAN MATRICES BE MULTIPLIED?

---

## 1. GIVEN

The dimensions of the four matrices are:

```math
A \in \mathbb{R}^{2\times3}
```

```math
B \in \mathbb{R}^{3\times4}
```

```math
C \in \mathbb{R}^{4\times2}
```

```math
D \in \mathbb{R}^{2\times2}
```

---

## 2. COMPLETE QUESTION

Consider the following eight matrix products:

1. AB
2. BA
3. BC
4. CB
5. AC
6. CA
7. AD
8. DA

For each of these eight products:

- Determine whether the multiplication is defined.
- If the product is defined, state the dimensions of the resulting matrix.
- If the product is not defined, explain why the multiplication is impossible.
- Justify every decision using the dimension compatibility condition.

Remember that two matrices can be multiplied only when the number of columns in the first matrix equals the number of rows in the second matrix.

---

## 3. MATRIX MULTIPLICATION RULE

The general dimension compatibility condition is:

```math
(m\times n)(n\times p)=m\times p
```

The inner dimensions must be equal.

The outer dimensions determine the size of the resulting matrix.

---

## 4. SOLUTIONS

### 4.1. Product AB

The dimensions are:

```math
(2\times3)(3\times4)
```

The inner dimensions are both 3.

Therefore, the multiplication is defined.

The resulting matrix has dimensions:

```math
AB: 2\times4
```

### 4.2. Product BA

The dimensions are:

```math
(3\times4)(2\times3)
```

The inner dimensions are 4 and 2.

Since they are different, the multiplication is not defined.

```math
BA:\text{ Not defined}
```

### 4.3. Product BC

The dimensions are:

```math
(3\times4)(4\times2)
```

The inner dimensions are both 4.

Therefore, the multiplication is defined.

The resulting matrix has dimensions:

```math
BC: 3\times2
```

### 4.4. Product CB

The dimensions are:

```math
(4\times2)(3\times4)
```

The inner dimensions are 2 and 3.

Since they are different, the multiplication is not defined.

```math
CB:\text{ Not defined}
```

### 4.5. Product AC

The dimensions are:

```math
(2\times3)(4\times2)
```

The inner dimensions are 3 and 4.

Since they are different, the multiplication is not defined.

```math
AC:\text{ Not defined}
```

### 4.6. Product CA

The dimensions are:

```math
(4\times2)(2\times3)
```

The inner dimensions are both 2.

Therefore, the multiplication is defined.

The resulting matrix has dimensions:

```math
CA: 4\times3
```

### 4.7. Product AD

The dimensions are:

```math
(2\times3)(2\times2)
```

The inner dimensions are 3 and 2.

Since they are different, the multiplication is not defined.

```math
AD:\text{ Not defined}
```

### 4.8. Product DA

The dimensions are:

```math
(2\times2)(2\times3)
```

The inner dimensions are both 2.

Therefore, the multiplication is defined.

The resulting matrix has dimensions:

```math
DA: 2\times3
```

---

## 5. SUMMARY TABLE

| Product | Dimensions | Result |
|---|---|---|
| AB | (2×3)(3×4) | Defined: 2×4 |
| BA | (3×4)(2×3) | Not defined |
| BC | (3×4)(4×2) | Defined: 3×2 |
| CB | (4×2)(3×4) | Not defined |
| AC | (2×3)(4×2) | Not defined |
| CA | (4×2)(2×3) | Defined: 4×3 |
| AD | (2×3)(2×2) | Not defined |
| DA | (2×2)(2×3) | Defined: 2×3 |

---

## 6. CONCLUSION

Out of the eight matrix products:

Four products are defined:

- AB: 2×4
- BC: 3×2
- CA: 4×3
- DA: 2×3

Four products are not defined:

- BA
- CB
- AC
- AD

The reason is that matrix multiplication requires the number of columns in the first matrix to equal the number of rows in the second matrix.

This condition must always be checked before multiplying matrices.
