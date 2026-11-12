
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

## 2. QUESTIONS

Determine whether each of the following matrix products is defined:

1. AB
2. BA
3. BC
4. CB
5. AC
6. CA
7. AD
8. DA

For every product:

- Determine whether the multiplication is defined.
- If it is defined, state the dimensions of the resulting matrix.
- If it is not defined, explain why.
- Justify each decision using the dimension compatibility condition.

---

## 3. MATRIX MULTIPLICATION RULE

Two matrices can be multiplied if the number of columns in the first matrix equals the number of rows in the second matrix.

The general rule is:

```math
(m\times n)(n\times p)=m\times p
```

The inner dimensions must be equal.

The outer dimensions determine the size of the resulting matrix.

---

## 4. SOLUTIONS

### 4.1. Product AB

Dimensions:

```math
(2\times3)(3\times4)
```

The inner dimensions are both 3, so the multiplication is defined.

The resulting matrix has dimensions:

```math
\boxed{AB: 2\times4}
```

### 4.2. Product BA

Dimensions:

```math
(3\times4)(2\times3)
```

The inner dimensions are 4 and 2.

Since they are different, the multiplication is not defined.

```math
\boxed{BA:\text{ Not defined}}
```

### 4.3. Product BC

Dimensions:

```math
(3\times4)(4\times2)
```

The inner dimensions are both 4, so the multiplication is defined.

The resulting matrix has dimensions:

```math
\boxed{BC: 3\times2}
```

### 4.4. Product CB

Dimensions:

```math
(4\times2)(3\times4)
```

The inner dimensions are 2 and 3.

Since they are different, the multiplication is not defined.

```math
\boxed{CB:\text{ Not defined}}
```

### 4.5. Product AC

Dimensions:

```math
(2\times3)(4\times2)
```

The inner dimensions are 3 and 4.

Since they are different, the multiplication is not defined.

```math
\boxed{AC:\text{ Not defined}}
```

### 4.6. Product CA

Dimensions:

```math
(4\times2)(2\times3)
```

The inner dimensions are both 2, so the multiplication is defined.

The resulting matrix has dimensions:

```math
\boxed{CA: 4\times3}
```

### 4.7. Product AD

Dimensions:

```math
(2\times3)(2\times2)
```

The inner dimensions are 3 and 2.

Since they are different, the multiplication is not defined.

```math
\boxed{AD:\text{ Not defined}}
```

### 4.8. Product DA

Dimensions:

```math
(2\times2)(2\times3)
```

The inner dimensions are both 2, so the multiplication is defined.

The resulting matrix has dimensions:

```math
\boxed{DA: 2\times3}
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

Matrix multiplication is possible only when the number of columns in the first matrix equals the number of rows in the second matrix.

Out of the eight products:

- Four products are defined: AB, BC, CA and DA.
- Four products are not defined: BA, CB, AC and AD.

The resulting matrix dimensions depend on the outer dimensions of the two matrices.

This exercise demonstrates the importance of checking dimension compatibility before performing matrix multiplication.
