
# EXERCISE 6 – PROJECTION AND PERPENDICULAR COMPONENT

## Given

Find the projection of u onto the direction v:

$$
u=(4,2)
$$

$$
v=(1,1)
$$

Then compute the perpendicular component r using:

$$
r=u-p
$$

where p is the projection of u onto v.

Verify that:

$$
r\cdot v=0
$$

Explain the result geometrically.

## Solution

### Step 1 – Calculate the Dot Product

First, calculate the dot product of u and v.

$$
u\cdot v=4(1)+2(1)
$$

$$
u\cdot v=4+2=6
$$

### Step 2 – Calculate the Length Squared of v

$$
v\cdot v=1(1)+1(1)
$$

$$
v\cdot v=2
$$

### Step 3 – Calculate the Projection

The projection vector is calculated using:

$$
p=\frac{u\cdot v}{v\cdot v}v
$$

Substitute the values:

$$
p=\frac{6}{2}(1,1)
$$

$$
p=3(1,1)
$$

Therefore:

$$
p=(3,3)
$$

### Step 4 – Calculate the Perpendicular Component

The perpendicular component is:

$$
r=u-p
$$

Substitute the vectors:

$$
r=(4,2)-(3,3)
$$

$$
r=(4-3,2-3)
$$

Therefore:

$$
r=(1,-1)
$$

### Step 5 – Verify Perpendicularity

Two vectors are perpendicular when their dot product equals zero.

Calculate:

$$
r\cdot v=(1,-1)\cdot(1,1)
$$

$$
r\cdot v=1(1)+(-1)(1)
$$

$$
r\cdot v=1-1
$$

Therefore:

$$
r\cdot v=0
$$

This confirms that r is perpendicular to v.

### Step 6 – Geometrical Explanation

The original vector u is divided into two components:

1. The projection p, which is parallel to v.
2. The perpendicular component r, which is perpendicular to v.

Together, these components reconstruct the original vector:

$$
u=p+r
$$

Substitute the values:

$$
(4,2)=(3,3)+(1,-1)
$$

This equality is correct.

Geometrically, the two components form a right angle.

The projection represents the part of u that points in the direction of v, while r represents the remaining perpendicular part.

### Final Answer

The projection vector is:

$$
p=(3,3)
$$

The perpendicular component is:

$$
r=(1,-1)
$$

Verification:

$$
r\cdot v=0
$$

### Conclusion

Projection separates a vector into a parallel component and a perpendicular component.

The two components add up to the original vector, and their perpendicular relationship is confirmed by a zero dot product.
