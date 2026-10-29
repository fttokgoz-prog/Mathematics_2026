# Exercise 9. Composing Transformations

## Given

S = ( 2  0 )
    ( 0  1 )


R = ( 0  -1 )
    ( 1   0 )


x = ( 1 )
    ( 2 )


The matrix S describes nonuniform scaling, while R describes a 90° counterclockwise rotation.

We need to compute RSx and SRx, compare the results, and explain why the order of the transformations matters.

## 1. Compute RSx

The expression RSx means that we first apply the scaling transformation S to the vector x, and then apply the rotation transformation R to the result.

Therefore, we calculate Sx first.

### Step 1: Calculate Sx

Sx = ( 2  0 ) ( 1 )
     ( 0  1 ) ( 2 )


First entry:

2 × 1 + 0 × 2 = 2 + 0 = 2


Second entry:

0 × 1 + 1 × 2 = 0 + 2 = 2


Therefore:

Sx = ( 2 )
     ( 2 )


The original vector (1, 2) becomes (2, 2). The first coordinate is doubled, while the second coordinate remains unchanged.

### Step 2: Apply the rotation matrix R

Now, we multiply R by the result Sx.

RSx = ( 0  -1 ) ( 2 )
      ( 1   0 ) ( 2 )


First entry:

0 × 2 + (-1) × 2 = 0 - 2 = -2


Second entry:

1 × 2 + 0 × 2 = 2 + 0 = 2


Therefore, the final result is:

RSx = ( -2 )
      (  2 )


## 2. Compute SRx

The expression SRx means that we first apply the rotation transformation R to the vector x, and then apply the scaling transformation S.

Therefore, we calculate Rx first.

### Step 1: Calculate Rx

Rx = ( 0  -1 ) ( 1 )
     ( 1   0 ) ( 2 )


First entry:

0 × 1 + (-1) × 2 = 0 - 2 = -2


Second entry:

1 × 1 + 0 × 2 = 1 + 0 = 1


Therefore:

Rx = ( -2 )
     (  1 )


The original vector (1, 2) becomes (-2, 1). This is a 90° counterclockwise rotation.

### Step 2: Apply the scaling matrix S

Now, we multiply S by the result Rx.

SRx = ( 2  0 ) ( -2 )
      ( 0  1 ) (  1 )


First entry:

2 × (-2) + 0 × 1 = -4 + 0 = -4


Second entry:

0 × (-2) + 1 × 1 = 0 + 1 = 1


Therefore, the final result is:

SRx = ( -4 )
      (  1 )


## 3. Compare the results

We obtained the following results:

RSx = ( -2 )
      (  2 )


SRx = ( -4 )
      (  1 )


The results are different:

RSx ≠ SRx


When we apply scaling first and rotation second, the final vector is (-2, 2).

When we apply rotation first and scaling second, the final vector is (-4, 1).

Therefore, changing the order of the transformations changes the final result.

## 4. Explain geometrically why the order matters

The scaling matrix S doubles the horizontal coordinate and leaves the vertical coordinate unchanged.

The rotation matrix R rotates a vector 90° counterclockwise. During this rotation, the horizontal and vertical coordinates change their positions and signs.

In the first case, we scale the original vector (1, 2) to obtain (2, 2), and then rotate it to obtain (-2, 2).

In the second case, we rotate the original vector (1, 2) to obtain (-2, 1), and then scale its horizontal coordinate to obtain (-4, 1).

The difference occurs because the scaling transformation treats the horizontal and vertical coordinates differently. Rotating the vector before scaling changes which original coordinate is affected by the scaling.

Therefore, these transformations are not interchangeable, and their order matters.

## Conclusion

RSx = (-2, 2)

SRx = (-4, 1)

Since RSx and SRx are different, applying scaling and rotation in different orders produces different results.

This demonstrates that matrix multiplication represents the composition of transformations, and the order in which the transformations are applied is important.
