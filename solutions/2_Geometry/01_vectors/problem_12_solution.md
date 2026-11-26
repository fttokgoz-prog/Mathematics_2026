
# EXERCISE 12 – A NORMAL VECTOR TO A PLANE

## Given

The three points are:

$$
A=(1,0,2)
$$

$$
B=(2,1,0)
$$

$$
C=(0,3,1)
$$

Construct two vectors lying in the plane, find a vector perpendicular to both, and check the perpendicularity using dot products.

## Solution

### Step 1 – Construct the First Vector AB

To find the vector from A to B, subtract the coordinates of A from B.

$$
AB=B-A
$$

Substitute the coordinates:

$$
AB=(2-1,1-0,0-2)
$$

Therefore:

$$
AB=(1,1,-2)
$$

### Step 2 – Construct the Second Vector AC

Similarly, subtract the coordinates of A from C.

$$
AC=C-A
$$

Substitute the coordinates:

$$
AC=(0-1,3-0,1-2)
$$

Therefore:

$$
AC=(-1,3,-1)
$$

Both vectors lie in the plane because they connect points belonging to the given plane.

### Step 3 – Calculate the Cross Product

To find a vector perpendicular to both AB and AC, calculate their cross product.

The formula is:

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
(1(-1)-(-2)(3),
(-2)(-1)-1(-1),
1(3)-1(-1))
$$

Calculate each component:

$$
AB\times AC=
( -1+6,\;2+1,\;3+1)
$$

Therefore:

$$
n=(5,3,4)
$$

This is a normal vector to the plane.

### Step 4 – Verify Perpendicularity to AB

A vector is perpendicular to another vector if their dot product equals zero.

Calculate:

$$
n\cdot AB
$$

Substitute the vectors:

$$
(5,3,4)\cdot(1,1,-2)
$$

Multiply the corresponding components:

$$
=5(1)+3(1)+4(-2)
$$

Simplify:

$$
=5+3-8
$$

Therefore:

$$
n\cdot AB=0
$$

The normal vector is perpendicular to AB.

### Step 5 – Verify Perpendicularity to AC

Now calculate the dot product with AC:

$$
n\cdot AC
$$

Substitute the vectors:

$$
(5,3,4)\cdot(-1,3,-1)
$$

Multiply the corresponding components:

$$
=5(-1)+3(3)+4(-1)
$$

Simplify:

$$
=-5+9-4
$$

Therefore:

$$
n\cdot AC=0
$$

The normal vector is also perpendicular to AC.

### Step 6 – Explain the Geometrical Meaning

The points A, B, and C define a plane.

The vectors AB and AC lie in this plane and represent two different directions within it.

Their cross product produces a new vector perpendicular to both directions.

Therefore, the resulting vector is perpendicular to the entire plane.

This vector is called a normal vector.

The normal vector can point in either of two opposite directions, and both directions are perpendicular to the plane.

### Final Answer

The first vector is:

$$
AB=(1,1,-2)
$$

The second vector is:

$$
AC=(-1,3,-1)
$$

The normal vector is:

$$
n=AB\times AC=(5,3,4)
$$

First verification:

$$
n\cdot AB=0
$$

Second verification:

$$
n\cdot AC=0
$$

Both perpendicularity conditions are satisfied.

### Conclusion

A normal vector to a plane can be found by calculating the cross product of two non-parallel vectors lying in that plane.

The dot product confirms that the resulting vector is perpendicular to both original vectors.

Therefore, the vector (5,3,4) is a valid normal vector to the plane defined by A, B, and C.
