
# EXERCISE 10 – TRIANGLE AREA FROM VECTORS

## Given

The three points are:

$$
A=(0,0,0)
$$

$$
B=(2,1,0)
$$

$$
C=(1,3,2)
$$

Construct the vectors AB and AC, compute the area of the parallelogram using the cross product, and then find the area of the triangle. Explain the factor 1/2.

## Solution

### Step 1 – Construct the Vector AB

To find the vector from A to B, subtract the coordinates of A from B.

$$
AB=B-A
$$

Substitute the coordinates:

$$
AB=(2-0,1-0,0-0)
$$

Therefore:

$$
AB=(2,1,0)
$$

### Step 2 – Construct the Vector AC

Similarly, subtract the coordinates of A from C.

$$
AC=C-A
$$

Substitute the coordinates:

$$
AC=(1-0,3-0,2-0)
$$

Therefore:

$$
AC=(1,3,2)
$$

### Step 3 – Calculate the Cross Product

The cross product of two three-dimensional vectors is:

$$
AB\times AC=
$$

$$
(AB_2AC_3-AB_3AC_2,
AB_3AC_1-AB_1AC_3,
AB_1AC_2-AB_2AC_1)
$$

Substitute the components:

$$
AB\times AC=
$$

$$
(1(2)-0(3),
0(1)-2(2),
2(3)-1(1))
$$

Calculate each component:

$$
AB\times AC=(2,-4,5)
$$

Therefore:

$$
AB\times AC=(2,-4,5)
$$

### Step 4 – Calculate the Area of the Parallelogram

The area of a parallelogram formed by two vectors is equal to the magnitude of their cross product.

The magnitude formula is:

$$
|v|=\sqrt{x^2+y^2+z^2}
$$

Substitute the cross product:

$$
|AB\times AC|=
\sqrt{2^2+(-4)^2+5^2}
$$

Calculate the squares:

$$
=\sqrt{4+16+25}
$$

Simplify:

$$
=\sqrt{45}
$$

Therefore:

$$
Area_{\text{parallelogram}}=3\sqrt{5}
$$

### Step 5 – Calculate the Area of the Triangle

A triangle formed by two vectors has half the area of the parallelogram formed by the same vectors.

Therefore, the triangle area is:

$$
Area_{\text{triangle}}=
\frac{1}{2}|AB\times AC|
$$

Substitute the calculated value:

$$
Area_{\text{triangle}}=
\frac{1}{2}(3\sqrt{5})
$$

Therefore:

$$
Area_{\text{triangle}}=
\frac{3\sqrt{5}}{2}
$$

The approximate value is:

$$
Area_{\text{triangle}}\approx3.354
$$

### Step 6 – Explain the Factor 1/2

The cross product gives the area of the parallelogram formed by vectors AB and AC.

A diagonal divides a parallelogram into two equal triangles.

Therefore, the triangle occupies exactly half of the parallelogram's area.

This is why we multiply the parallelogram area by 1/2 to obtain the triangle area.

### Final Answer

The first vector is:

$$
AB=(2,1,0)
$$

The second vector is:

$$
AC=(1,3,2)
$$

Their cross product is:

$$
AB\times AC=(2,-4,5)
$$

The area of the parallelogram is:

$$
Area_{\text{parallelogram}}=3\sqrt{5}
$$

The area of the triangle is:

$$
Area_{\text{triangle}}=
\frac{3\sqrt{5}}{2}
$$

### Conclusion

The cross product provides a direct way to calculate the area of a parallelogram formed by two vectors.

Since a triangle occupies half of that parallelogram, its area is obtained by multiplying the magnitude of the cross product by 1/2.

In this exercise, the triangle area is 3√5/2 square units.
