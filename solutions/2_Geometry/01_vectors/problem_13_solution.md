
# EXERCISE 13 – DO FOUR POINTS LIE IN ONE PLANE?

## Given

The four points are:

$$
A=(0,0,0)
$$

$$
B=(1,2,0)
$$

$$
C=(0,1,1)
$$

$$
D=(2,5,1)
$$

We need to determine whether all four points lie in the same plane.

## Solution

### Step 1 – Construct the Vector AB

To construct the vector AB, subtract the coordinates of A from B.

$$
AB=B-A
$$

Substitute the coordinates:

$$
AB=(1-0,2-0,0-0)
$$

Therefore:

$$
AB=(1,2,0)
$$

### Step 2 – Construct the Vector AC

Similarly, subtract the coordinates of A from C.

$$
AC=C-A
$$

Substitute the coordinates:

$$
AC=(0-0,1-0,1-0)
$$

Therefore:

$$
AC=(0,1,1)
$$

### Step 3 – Calculate the Normal Vector

To find a vector perpendicular to both AB and AC, calculate their cross product.

$$
n=AB\times AC
$$

Using the cross product formula:

$$
n=
(2(1)-0(1),
0(0)-1(1),
1(1)-2(0))
$$

Calculate each component:

$$
n=(2,-1,1)
$$

Therefore, the normal vector is:

$$
n=(2,-1,1)
$$

Since this normal vector is not zero, the vectors AB and AC are not parallel and determine a unique plane through A, B, and C.

### Step 4 – Construct the Vector AD

Now construct the vector from A to D.

$$
AD=D-A
$$

Substitute the coordinates:

$$
AD=(2-0,5-0,1-0)
$$

Therefore:

$$
AD=(2,5,1)
$$

### Step 5 – Check the Dot Product

For D to lie in the plane determined by A, B, and C, the vector AD must be perpendicular to the normal vector n.

Therefore, calculate:

$$
AD\cdot n
$$

Substitute the vectors:

$$
(2,5,1)\cdot(2,-1,1)
$$

Multiply the corresponding components:

$$
=2(2)+5(-1)+1(1)
$$

Simplify:

$$
=4-5+1
$$

Therefore:

$$
AD\cdot n=0
$$

The dot product equals zero, so AD is perpendicular to the normal vector.

### Step 6 – Determine Whether the Four Points Are Coplanar

We have established that:

$$
AD\cdot n=0
$$

This means that AD lies in the plane determined by A, B, and C.

Therefore, point D also belongs to this plane.

All four points lie in the same plane.

### Step 7 – Explain the Geometrical Criterion

Three non-collinear points determine a unique plane.

In this exercise, points A, B, and C determine the plane.

The cross product of AB and AC produces a normal vector perpendicular to that plane.

For another point D to belong to the same plane, the vector AD must be perpendicular to the normal vector.

This condition is expressed as:

$$
AD\cdot n=0
$$

Since this condition is satisfied, D belongs to the plane.

### Final Answer

The constructed vectors are:

$$
AB=(1,2,0)
$$

$$
AC=(0,1,1)
$$

The normal vector is:

$$
n=(2,-1,1)
$$

The vector AD is:

$$
AD=(2,5,1)
$$

The perpendicularity check gives:

$$
AD\cdot n=0
$$

Therefore:

$$
\boxed{\text{All four points are coplanar.}}
$$

### Conclusion

Four points lie in the same plane if the fourth point satisfies the perpendicularity condition with the normal vector of the plane determined by the first three non-collinear points.

In this exercise, the dot product equals zero, confirming that all four points lie in one plane.
