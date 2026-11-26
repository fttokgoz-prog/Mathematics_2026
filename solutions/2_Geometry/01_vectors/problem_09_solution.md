
# EXERCISE 9 – CROSS PRODUCT AS A PERPENDICULAR DIRECTION

## Given

The vectors are:

$$
u=(1,2,0)
$$

$$
v=(0,1,3)
$$

Compute the cross product u × v.

Use dot products to check perpendicularity to both vectors, compute v × u, and compare the results.

## Solution

### Step 1 – Calculate the Cross Product

The cross product of two vectors in three-dimensional space is calculated using:

$$
u\times v=
(u_2v_3-u_3v_2,\;
u_3v_1-u_1v_3,\;
u_1v_2-u_2v_1)
$$

Given:

$$
u=(1,2,0)
$$

$$
v=(0,1,3)
$$

Substitute the components:

$$
u\times v=
(2(3)-0(1),\;
0(0)-1(3),\;
1(1)-2(0))
$$

Calculate each component:

$$
u\times v=(6,-3,1)
$$

Therefore, the cross product is:

$$
\boxed{u\times v=(6,-3,1)}
$$

### Step 2 – Check Perpendicularity to u

A vector is perpendicular to another vector if their dot product equals zero.

Calculate the dot product:

$$
(u\times v)\cdot u
$$

Substitute the vectors:

$$
(6,-3,1)\cdot(1,2,0)
$$

Multiply the corresponding components:

$$
=6(1)+(-3)(2)+1(0)
$$

Simplify:

$$
=6-6+0
$$

Therefore:

$$
(u\times v)\cdot u=0
$$

This confirms that the cross product is perpendicular to u.

### Step 3 – Check Perpendicularity to v

Now calculate the dot product with v:

$$
(u\times v)\cdot v
$$

Substitute the vectors:

$$
(6,-3,1)\cdot(0,1,3)
$$

Multiply the corresponding components:

$$
=6(0)+(-3)(1)+1(3)
$$

Simplify:

$$
=0-3+3
$$

Therefore:

$$
(u\times v)\cdot v=0
$$

This confirms that the cross product is also perpendicular to v.

### Step 4 – Calculate the Reverse Cross Product

Now reverse the order of the original vectors and calculate v × u.

Using the same cross product formula:

$$
v\times u=
(v_2u_3-v_3u_2,\;
v_3u_1-v_1u_3,\;
v_1u_2-v_2u_1)
$$

Substitute the components:

$$
v\times u=
(1(0)-3(2),\;
3(1)-0(0),\;
0(2)-1(1))
$$

Calculate:

$$
v\times u=(-6,3,-1)
$$

Therefore:

$$
\boxed{v\times u=(-6,3,-1)}
$$

### Step 5 – Compare the Results

We obtained:

$$
u\times v=(6,-3,1)
$$

And:

$$
v\times u=(-6,3,-1)
$$

Comparing the two results:

$$
v\times u=-(u\times v)
$$

This shows that reversing the order of the vectors changes the direction of the cross product but does not change its magnitude.

The two resulting vectors point in opposite directions.

### Step 6 – Geometrical Explanation

The cross product produces a vector that is perpendicular to both original vectors.

In this exercise, u and v lie in the same plane, while their cross product points perpendicular to that plane.

The direction of the cross product follows the right-hand rule.

When the order of the vectors is reversed, the resulting vector points in the opposite direction.

This is why:

$$
u\times v\neq v\times u
$$

Instead:

$$
u\times v=-(v\times u)
$$

### Final Answer

The cross product is:

$$
u\times v=(6,-3,1)
$$

Perpendicularity checks:

$$
(u\times v)\cdot u=0
$$

$$
(u\times v)\cdot v=0
$$

The reverse cross product is:

$$
v\times u=(-6,3,-1)
$$

The relationship between the results is:

$$
v\times u=-(u\times v)
$$

### Conclusion

The cross product of two vectors produces a new vector perpendicular to both original vectors.

The dot product can be used to verify this perpendicularity.

Unlike ordinary multiplication, the cross product is not commutative. Reversing the order of the vectors changes the direction of the result while preserving its magnitude.
