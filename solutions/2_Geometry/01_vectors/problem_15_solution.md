
# EXERCISE 15 – COMPARING DIRECTIONS USING THE COSINE OF THE ANGLE

## Given

The three vectors are:

$$
a=(1,2,1)
$$

$$
b=(2,4,2)
$$

$$
c=(2,0,3)
$$

For each pair of vectors, we need to calculate the cosine of the angle using:

$$
\cos(\theta)=
\frac{u\cdot v}{|u|\cdot|v|}
$$

Then, we will order the pairs by increasing angle and explain why vectors a and b have a cosine value of 1 despite having different lengths.

## Solution

### Step 1 – Calculate the Lengths of the Vectors

First, calculate the length of each vector.

For vector a:

$$
|a|=\sqrt{1^2+2^2+1^2}
$$

$$
|a|=\sqrt{1+4+1}
$$

$$
|a|=\sqrt{6}
$$

For vector b:

$$
|b|=\sqrt{2^2+4^2+2^2}
$$

$$
|b|=\sqrt{4+16+4}
$$

$$
|b|=\sqrt{24}=2\sqrt{6}
$$

For vector c:

$$
|c|=\sqrt{2^2+0^2+3^2}
$$

$$
|c|=\sqrt{4+0+9}
$$

$$
|c|=\sqrt{13}
$$

Therefore, the lengths are:

$$
|a|=\sqrt{6}
$$

$$
|b|=2\sqrt{6}
$$

$$
|c|=\sqrt{13}
$$

### Step 2 – Calculate the Cosine Between a and b

First, calculate the dot product:

$$
a\cdot b=1(2)+2(4)+1(2)
$$

$$
a\cdot b=2+8+2=12
$$

Now use the cosine formula:

$$
\cos(\theta)=
\frac{a\cdot b}{|a|\cdot|b|}
$$

Substitute the values:

$$
\cos(\theta)=
\frac{12}{\sqrt{6}\cdot2\sqrt{6}}
$$

Simplify:

$$
\cos(\theta)=\frac{12}{12}
$$

Therefore:

$$
\boxed{\cos(\theta)=1}
$$

The angle is:

$$
\theta=0^\circ
$$

This means that vectors a and b have the same direction.

### Step 3 – Calculate the Cosine Between a and c

First, calculate the dot product:

$$
a\cdot c=1(2)+2(0)+1(3)
$$

$$
a\cdot c=2+0+3=5
$$

Now use the cosine formula:

$$
\cos(\theta)=
\frac{a\cdot c}{|a|\cdot|c|}
$$

Substitute the values:

$$
\cos(\theta)=
\frac{5}{\sqrt{6}\cdot\sqrt{13}}
$$

Simplify:

$$
\boxed{\cos(\theta)=\frac{5}{\sqrt{78}}}
$$

The approximate value is:

$$
\cos(\theta)\approx0.5661
$$

Therefore, the angle is approximately:

$$
\theta\approx55.5^\circ
$$

### Step 4 – Calculate the Cosine Between b and c

First, calculate the dot product:

$$
b\cdot c=2(2)+4(0)+2(3)
$$

$$
b\cdot c=4+0+6=10
$$

Now use the cosine formula:

$$
\cos(\theta)=
\frac{b\cdot c}{|b|\cdot|c|}
$$

Substitute the values:

$$
\cos(\theta)=
\frac{10}{2\sqrt{6}\cdot\sqrt{13}}
$$

Simplify:

$$
\cos(\theta)=\frac{10}{2\sqrt{78}}
$$

Therefore:

$$
\boxed{\cos(\theta)=\frac{5}{\sqrt{78}}}
$$

The approximate value is:

$$
\cos(\theta)\approx0.5661
$$

Therefore, the angle is approximately:

$$
\theta\approx55.5^\circ
$$

### Step 5 – Order the Pairs by Increasing Angle

We have calculated the following results:

| Vector pair | Cosine value | Angle |
|---|---|---|
| a and b | 1 | 0° |
| a and c | 5/√78 ≈ 0.5661 | 55.5° |
| b and c | 5/√78 ≈ 0.5661 | 55.5° |

The increasing order of the angles is:

1. a and b – 0°
2. a and c – approximately 55.5°
3. b and c – approximately 55.5°

The last two pairs have equal angles.

### Step 6 – Explain Why a and b Have a Cosine Value of 1

Notice that vector b is exactly twice vector a:

$$
b=2a
$$

This means that both vectors point in the same direction, but vector b is twice as long.

The cosine formula measures the angle between two vectors, not their lengths.

Since the vectors have the same direction, the angle between them is zero degrees.

Therefore:

$$
\cos(0^\circ)=1
$$

This explains why the cosine value is 1 even though the vectors have different lengths.

### Final Answer

The cosine values for all three pairs are:

$$
\boxed{\cos(a,b)=1}
$$

$$
\boxed{\cos(a,c)=\frac{5}{\sqrt{78}}}
$$

$$
\boxed{\cos(b,c)=\frac{5}{\sqrt{78}}}
$$

The increasing order of the angles is:

$$
\boxed{
\theta_{ab}<\theta_{ac}=\theta_{bc}
}
$$

### Conclusion

The cosine of the angle measures the relationship between the directions of two vectors.

Vectors a and b have different lengths, but they point in exactly the same direction because b is twice a.

Therefore, their angle is zero degrees and their cosine value is 1.

The other two pairs have equal angles because vector b is a positive scalar multiple of vector a. Scaling a vector by a positive number changes its length but does not change its direction.
