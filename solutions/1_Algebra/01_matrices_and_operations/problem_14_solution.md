
# EXERCISE 14
# ROTATION MATRICES

---

## 1. GIVEN

The matrix representing a rotation through an angle θ is:

```math
R(\theta)=
\begin{pmatrix}
\cos\theta & -\sin\theta \\
\sin\theta & \cos\theta
\end{pmatrix}
```

We need to calculate R(α)R(β), prove that it equals R(α + β), and explain the result geometrically.

---

## 2. SOLUTION

### STEP 1 - Write Both Rotation Matrices

The first rotation matrix is:

```math
R(\alpha)=
\begin{pmatrix}
\cos\alpha & -\sin\alpha \\
\sin\alpha & \cos\alpha
\end{pmatrix}
```

The second rotation matrix is:

```math
R(\beta)=
\begin{pmatrix}
\cos\beta & -\sin\beta \\
\sin\beta & \cos\beta
\end{pmatrix}
```

### STEP 2 - Multiply the Matrices

We calculate:

```math
R(\alpha)R(\beta)
```

The upper-left entry is:

```math
\cos\alpha\cos\beta-\sin\alpha\sin\beta
```

The upper-right entry is:

```math
-\cos\alpha\sin\beta-\sin\alpha\cos\beta
```

The lower-left entry is:

```math
\sin\alpha\cos\beta+\cos\alpha\sin\beta
```

The lower-right entry is:

```math
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
```

Therefore, the resulting matrix is:

```math
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos\alpha\cos\beta-\sin\alpha\sin\beta &
-\cos\alpha\sin\beta-\sin\alpha\cos\beta \\
\sin\alpha\cos\beta+\cos\alpha\sin\beta &
-\sin\alpha\sin\beta+\cos\alpha\cos\beta
\end{pmatrix}
```

---

## 3. APPLY THE ANGLE-SUM FORMULAS

We use two important trigonometric identities.

### 3.1. Cosine Addition Formula

```math
\cos(\alpha+\beta)
=
\cos\alpha\cos\beta
-
\sin\alpha\sin\beta
```

### 3.2. Sine Addition Formula

```math
\sin(\alpha+\beta)
=
\sin\alpha\cos\beta
+
\cos\alpha\sin\beta
```

### 3.3. Simplifying the Matrix

Using these identities, the four entries become:

- Upper-left: cos(α + β)
- Upper-right: -sin(α + β)
- Lower-left: sin(α + β)
- Lower-right: cos(α + β)

---

## 4. FINAL MATRIX RESULT

After applying the angle-sum formulas, we obtain:

```math
R(\alpha)R(\beta)=
\begin{pmatrix}
\cos(\alpha+\beta) & -\sin(\alpha+\beta) \\
\sin(\alpha+\beta) & \cos(\alpha+\beta)
\end{pmatrix}
```

This is exactly the rotation matrix for the angle α + β.

Therefore:

```math
\boxed{R(\alpha)R(\beta)=R(\alpha+\beta)}
```

The required identity is proven.

---

## 5. GEOMETRICAL EXPLANATION

A rotation matrix changes the direction of a vector without changing its length.

When we apply two rotations one after another:

1. First, we rotate the vector by angle β.
2. Then, we rotate it by angle α.
3. The total rotation is the sum of both angles.

For example:

```math
30^\circ+60^\circ=90^\circ
```

Rotating a vector by 30 degrees and then by 60 degrees gives the same result as rotating it directly by 90 degrees.

Therefore, two consecutive rotations can be combined into one rotation.

---

## 6. CONCLUSION

We calculated the product of two rotation matrices and used the angle-sum formulas for sine and cosine.

We proved that:

```math
\boxed{R(\alpha)R(\beta)=R(\alpha+\beta)}
```

Geometrically, this means that two consecutive rotations are equivalent to one rotation through the sum of their angles.

The matrix result is consistent with the geometric properties of rotations.
