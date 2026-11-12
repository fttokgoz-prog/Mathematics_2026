# Exercise 3. When Can Matrices Be Multiplied?

## Given

The dimensions of the matrices are:

- Matrix A: \(2 \times 3\)
- Matrix B: \(3 \times 4\)
- Matrix C: \(4 \times 2\)
- Matrix D: \(2 \times 2\)

## Questions

Determine whether the following matrix products are defined:

1. \(AB\)
2. \(BA\)
3. \(BC\)
4. \(CB\)
5. \(AC\)
6. \(CA\)
7. \(AD\)
8. \(DA\)

If a product is defined, state the size of the resulting matrix. Justify each answer using the dimension compatibility condition.

## Solution

### Multiplication Rule

Two matrices can be multiplied if the number of columns in the first matrix equals the number of rows in the second matrix.

For example:

$$
(m \times n)(n \times p) = m \times p
$$

The inner dimensions must be equal. The result has the outer dimensions.

### 1. Product AB

$$
A_{2 \times 3} \cdot B_{3 \times 4}
$$

The inner dimensions are equal (3 = 3).

**Defined.** The result has size:

$$
\boxed{AB: 2 \times 4}
$$

### 2. Product BA

$$
B_{3 \times 4} \cdot A_{2 \times 3}
$$

The inner dimensions are not equal (4 ≠ 2).

**Not defined.**

### 3. Product BC

$$
B_{3 \times 4} \cdot C_{4 \times 2}
$$

The inner dimensions are equal (4 = 4).

**Defined.** The result has size:

$$
\boxed{BC: 3 \times 2}
$$

### 4. Product CB

$$
C_{4 \times 2} \cdot B_{3 \times 4}
$$

The inner dimensions are not equal (2 ≠ 3).

**Not defined.**

### 5. Product AC

$$
A_{2 \times 3} \cdot C_{4 \times 2}
$$

The inner dimensions are not equal (3 ≠ 4).

**Not defined.**

### 6. Product CA

$$
C_{4 \times 2} \cdot A_{2 \times 3}
$$

The inner dimensions are equal (2 = 2).

**Defined.** The result has size:

$$
\boxed{CA: 4 \times 3}
$$

### 7. Product AD

$$
A_{2 \times 3} \cdot D_{2 \times 2}
$$

The inner dimensions are not equal (3 ≠ 2).

**Not defined.**

### 8. Product DA

$$
D_{2 \times 2} \cdot A_{2 \times 3}
$$

The inner dimensions are equal (2 = 2).

**Defined.** The result has size:

$$
\boxed{DA: 2 \times 3}
$$

## Final Summary

| Product | Defined? | Result Size |
|---|---|---|
| AB | Yes | \(2 \times 4\) |
| BA | No | Not defined |
| BC | Yes | \(3 \times 2\) |
| CB | No | Not defined |
| AC | No | Not defined |
| CA | Yes | \(4 \times 3\) |
| AD | No | Not defined |
| DA | Yes | \(2 \times 3\) |

## Conclusion

Matrix multiplication is possible only when the number of columns in the first matrix equals the number of rows in the second matrix.

The order of multiplication matters because changing the order can make a product undefined or produce a different result size.
