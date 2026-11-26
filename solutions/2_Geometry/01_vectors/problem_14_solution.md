
# EXERCISE 14 – CLOSEST POINT ON A LINE

## Given

The point is:

$$
P=(4,1)
$$

The line passes through the origin and has direction vector:

$$
v=(1,2)
$$

### Graphical Representation

The following graph shows the point P, the line y = 2x, the closest point Q, and the perpendicular segment connecting P to Q.

![Exercise 14 - Closest Point on a Line](exercise14_closest_point_graph.png)

The red point represents P, the blue point represents Q, and the dashed line represents the perpendicular distance from P to the line.

We need to find the closest point on the line to P using projection, calculate the distance from P to the line, and verify that the appropriate vector is perpendicular to the direction of the line.

## Solution

### Step 1 – Identify the Direction Vector

The line passes through the origin and has direction vector:

$$
v=(1,2)
$$

Every point on this line can be written as:

$$
Q=t(1,2)
$$

where t is a real number.

### Step 2 – Calculate the Projection

The closest point on the line is the projection of P onto v.

The projection formula is:

$$
Q=\frac{P\cdot v}{v\cdot v}v
$$

First, calculate the dot product of P and v:

$$
P\cdot v=4(1)+1(2)
$$

$$
P\cdot v=4+2=6
$$

Next, calculate the dot product of v with itself:

$$
v\cdot v=1(1)+2(2)
$$

$$
v\cdot v=1+4=5
$$

Substitute these values into the projection formula:

$$
Q=\frac{6}{5}(1,2)
$$

Multiply each component:

$$
Q=\left(\frac{6}{5},\frac{12}{5}\right)
$$

Therefore, the closest point on the line is:

$$
\boxed{Q=\left(\frac{6}{5},\frac{12}{5}\right)}
$$

### Step 3 – Calculate the Distance from P to the Line

The distance is the length of the vector from Q to P.

First, calculate the difference:

$$
P-Q=
(4,1)-\left(\frac{6}{5},\frac{12}{5}\right)
$$

Subtract the corresponding components:

$$
P-Q=
\left(\frac{20}{5}-\frac{6}{5},
\frac{5}{5}-\frac{12}{5}\right)
$$

Therefore:

$$
P-Q=\left(\frac{14}{5},-\frac{7}{5}\right)
$$

Now calculate its length:

$$
d(P,Q)=
\sqrt{\left(\frac{14}{5}\right)^2+
\left(-\frac{7}{5}\right)^2}
$$

Calculate the squares:

$$
=\sqrt{\frac{196}{25}+\frac{49}{25}}
$$

Simplify:

$$
=\sqrt{\frac{245}{25}}
$$

$$
=\frac{\sqrt{245}}{5}
$$

Since 245 = 49 × 5:

$$
d(P,Q)=\frac{7\sqrt{5}}{5}
$$

The approximate distance is:

$$
d(P,Q)\approx3.13
$$

### Step 4 – Verify Perpendicularity

The vector from Q to P must be perpendicular to the direction vector v.

We already calculated:

$$
P-Q=\left(\frac{14}{5},-\frac{7}{5}\right)
$$

Calculate its dot product with v:

$$
(P-Q)\cdot v
$$

Substitute the values:

$$
=\frac{14}{5}(1)+
\left(-\frac{7}{5}\right)(2)
$$

Simplify:

$$
=\frac{14}{5}-\frac{14}{5}
$$

Therefore:

$$
(P-Q)\cdot v=0
$$

This confirms that the vector from Q to P is perpendicular to the direction of the line.

### Step 5 – Explain the Geometrical Meaning

The point Q is the projection of P onto the line.

The shortest distance between a point and a line is always measured along a perpendicular segment.

Since the vector P - Q is perpendicular to the direction vector v, the segment connecting P and Q represents the shortest possible distance.

Any other point on the line would produce a longer distance from P.

Therefore, Q is the closest point on the line to P.

### Final Answer

The closest point on the line is:

$$
Q=\left(\frac{6}{5},\frac{12}{5}\right)
$$

The distance from P to the line is:

$$
d(P,\text{line})=\frac{7\sqrt{5}}{5}
$$

The approximate distance is:

$$
d(P,\text{line})\approx3.13
$$

The perpendicularity check gives:

$$
(P-Q)\cdot v=0
$$

### Conclusion

Projection provides a direct method for finding the closest point on a line to a given point.

The distance is calculated using the length of the perpendicular vector between the original point and its projection.

The dot product confirms that this vector is perpendicular to the line, proving that the calculated point gives the minimum distance.
