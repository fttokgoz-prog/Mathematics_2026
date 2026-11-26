
# EXERCISE 11 – DECOMPOSITION INTO PARALLEL AND PERPENDICULAR COMPONENTS

## Given

Decompose the vector u into components parallel and perpendicular to v.

$$
u=(3,4)
$$

$$
v=(1,2)
$$

Check that:

$$
u=u_{\parallel}+u_{\perp}
$$

and

$$
u_{\perp}\cdot v=0
$$

Explain why these are two independent checks of correctness.

## Solution

### Step 1 – Calculate the Dot Product

First, calculate the dot product of u and v.

$$
u\cdot v=3(1)+4(2)
$$

Simplify:

$$
u\cdot v=3+8=11
$$

### Step 2 – Calculate the Length Squared of v

Calculate the dot product of v with itself.

$$
v\cdot v=1(1)+2(2)
$$

Therefore:

$$
v\cdot v=1+4=5
$$

### Step 3 – Calculate the Parallel Component

The parallel component is calculated using the projection formula:

$$
u_{\parallel}=
\frac{u\cdot v}{v\cdot v}v
$$

Substitute the calculated values:

$$
u_{\parallel}=
\frac{11}{5}(1,2)
$$

Multiply each component:

$$
u_{\parallel}=
\left(\frac{11}{5},\frac{22}{5}\right)
$$

This is the component of u parallel to v.

### Step 4 – Calculate the Perpendicular Component

The perpendicular component is obtained by subtracting the parallel component from the original vector.

$$
u_{\perp}=u-u_{\parallel}
$$

Substitute the values:

$$
u_{\perp}=
(3,4)-\left(\frac{11}{5},\frac{22}{5}\right)
$$

Subtract the corresponding components:

$$
u_{\perp}=
\left(3-\frac{11}{5},4-\frac{22}{5}\right)
$$

Convert the integers into fractions:

$$
u_{\perp}=
\left(\frac{15}{5}-\frac{11}{5},
\frac{20}{5}-\frac{22}{5}\right)
$$

Therefore:

$$
u_{\perp}=
\left(\frac{4}{5},-\frac{2}{5}\right)
$$

### Step 5 – Check the Decomposition

The first condition is:

$$
u=u_{\parallel}+u_{\perp}
$$

Substitute the calculated components:

$$
(3,4)=
\left(\frac{11}{5},\frac{22}{5}\right)
+
\left(\frac{4}{5},-\frac{2}{5}\right)
$$

Add the corresponding components:

$$
(3,4)=
\left(\frac{15}{5},\frac{20}{5}\right)
$$

Simplify:

$$
(3,4)=(3,4)
$$

The first condition is satisfied.

### Step 6 – Check Perpendicularity

The second condition is:

$$
u_{\perp}\cdot v=0
$$

Substitute the vectors:

$$
\left(\frac{4}{5},-\frac{2}{5}\right)
\cdot(1,2)=0
$$

Calculate the dot product:

$$
\frac{4}{5}(1)+
\left(-\frac{2}{5}\right)(2)
$$

Simplify:

$$
\frac{4}{5}-\frac{4}{5}=0
$$

Therefore:

$$
u_{\perp}\cdot v=0
$$

The perpendicularity condition is also satisfied.

### Step 7 – Explain Why Both Checks Are Necessary

The two checks verify different properties of the decomposition.

The first check:

$$
u=u_{\parallel}+u_{\perp}
$$

confirms that the two components reconstruct the original vector correctly.

The second check:

$$
u_{\perp}\cdot v=0
$$

confirms that the perpendicular component is actually perpendicular to v.

These checks are independent because reconstructing the original vector alone does not guarantee that the components have the correct directions.

Similarly, perpendicularity alone does not guarantee that the components add up to the original vector.

Both conditions are necessary for a correct decomposition.

### Final Answer

The parallel component is:

$$
u_{\parallel}=
\left(\frac{11}{5},\frac{22}{5}\right)
$$

The perpendicular component is:

$$
u_{\perp}=
\left(\frac{4}{5},-\frac{2}{5}\right)
$$

First verification:

$$
u=u_{\parallel}+u_{\perp}
$$

Second verification:

$$
u_{\perp}\cdot v=0
$$

Both conditions are satisfied.

### Conclusion

A vector can be decomposed into parallel and perpendicular components relative to a given direction.

The parallel component is obtained using vector projection, while the perpendicular component is the remaining part.

Checking the reconstruction and perpendicularity independently confirms that the decomposition is correct.
