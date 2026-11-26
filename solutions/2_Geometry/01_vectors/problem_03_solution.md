
# EXERCISE 3 – VECTOR NORMALIZATION

## Given

For the vector:

$$
v=(3,4)
$$

Find a unit vector e with the same direction and orientation.

Check that |e| = 1, reconstruct v in the form v = |v|e, and explain what changes during normalization and what remains unchanged.

## Solution

### Step 1 – Calculate the Length of the Vector

The length of a two-dimensional vector is calculated using:

$$
|v|=\sqrt{x^2+y^2}
$$

Given:

$$
v=(3,4)
$$

Substitute the components:

$$
|v|=\sqrt{3^2+4^2}
$$

$$
|v|=\sqrt{9+16}
$$

Therefore:

$$
|v|=\sqrt{25}=5
$$

The length of the original vector is 5.

### Step 2 – Calculate the Unit Vector

To normalize a vector, divide each component by its length.

The formula is:

$$
e=\frac{v}{|v|}
$$

Substitute the values:

$$
e=\frac{(3,4)}{5}
$$

Divide each component by 5:

$$
e=\left(\frac{3}{5},\frac{4}{5}\right)
$$

This is the unit vector with the same direction and orientation as v.

### Step 3 – Verify That the Unit Vector Has Length 1

The length of e is:

$$
|e|=\sqrt{\left(\frac{3}{5}\right)^2+
\left(\frac{4}{5}\right)^2}
$$

Calculate the squares:

$$
|e|=\sqrt{\frac{9}{25}+\frac{16}{25}}
$$

Combine the fractions:

$$
|e|=\sqrt{\frac{25}{25}}
$$

Therefore:

$$
|e|=\sqrt{1}=1
$$

The unit vector condition is satisfied.

### Step 4 – Reconstruct the Original Vector

We need to verify:

$$
v=|v|e
$$

We already know:

$$
|v|=5
$$

And:

$$
e=\left(\frac{3}{5},\frac{4}{5}\right)
$$

Multiply the unit vector by the original length:

$$
|v|e=5\left(\frac{3}{5},\frac{4}{5}\right)
$$

Multiply each component:

$$
|v|e=(3,4)
$$

Therefore:

$$
|v|e=v
$$

The original vector has been reconstructed correctly.

### Step 5 – Explain What Changes During Normalization

During normalization, the length of the vector changes to 1.

However, its direction and orientation remain unchanged.

For the original vector:

$$
v=(3,4)
$$

Its length is:

$$
|v|=5
$$

After normalization:

$$
e=\left(\frac{3}{5},\frac{4}{5}\right)
$$

Its length becomes:

$$
|e|=1
$$

Both vectors point in the same direction.

Normalization changes the magnitude but preserves the direction and orientation.

### Final Answer

The original vector is:

$$
v=(3,4)
$$

Its length is:

$$
|v|=5
$$

The normalized unit vector is:

$$
e=\left(\frac{3}{5},\frac{4}{5}\right)
$$

Verification:

$$
|e|=1
$$

Reconstruction:

$$
v=|v|e=(3,4)
$$

### Conclusion

Vector normalization converts a nonzero vector into a unit vector by dividing each component by its magnitude.

The magnitude becomes 1, while the direction and orientation remain unchanged.

The original vector can always be reconstructed by multiplying the unit vector by its original magnitude.
