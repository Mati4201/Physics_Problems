```python
import numpy as np

a = np.array([2, 1, -3])
b = np.array([4, -2, 1])

mag_a = np.linalg.norm(a)
mag_b = np.linalg.norm(b)
dot_ab = np.dot(a, b)
cross_ab = np.cross(a, b)
cos_theta = dot_ab / (mag_a * mag_b)
theta_rad = np.arccos(cos_theta)
theta_deg = np.degrees(theta_rad)

print(f"mag_a: {mag_a} (sqrt 14 = {np.sqrt(14)})")
print(f"mag_b: {mag_b} (sqrt 21 = {np.sqrt(21)})")
print(f"dot: {dot_ab}")
print(f"cross: {cross_ab}")
print(f"theta_deg: {theta_deg}")
print(f"theta_rad: {theta_rad}")


```

```text
mag_a: 3.7416573867739413 (sqrt 14 = 3.7416573867739413)
mag_b: 4.58257569495584 (sqrt 21 = 4.58257569495584)
dot: 3
cross: [ -5 -14  -8]
theta_deg: 79.92346287144585
theta_rad: 1.3949275767021716


```

Here is the step-by-step solution for the given vectors $\vec{a} = [2, 1, -3]$ and $\vec{b} = [4, -2, 1]$:

**a) The magnitude of each vector**

The magnitude (or length) of a 3D vector $\vec{v} = [x, y, z]$ is given by the formula $|\vec{v}| = \sqrt{x^2 + y^2 + z^2}$.

For vector $\vec{a}$:


$$|\vec{a}| = \sqrt{2^2 + 1^2 + (-3)^2}$$

$$|\vec{a}| = \sqrt{4 + 1 + 9}$$

$$|\vec{a}| = \sqrt{14} \approx 3.74$$

For vector $\vec{b}$:


$$|\vec{b}| = \sqrt{4^2 + (-2)^2 + 1^2}$$

$$|\vec{b}| = \sqrt{16 + 4 + 1}$$

$$|\vec{b}| = \sqrt{21} \approx 4.58$$

**b) The dot product $\vec{a} \cdot \vec{b}$**

The dot product is calculated as $\vec{a} \cdot \vec{b} = a_x b_x + a_y b_y + a_z b_z$.

$$\vec{a} \cdot \vec{b} = (2)(4) + (1)(-2) + (-3)(1)$$

$$\vec{a} \cdot \vec{b} = 8 - 2 - 3$$

$$\vec{a} \cdot \vec{b} = 3$$

**c) The cross product $\vec{a} \times \vec{b}$**

The cross product can be found by evaluating the determinant of the formal matrix:

$$\vec{a} \times \vec{b} = \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\ 
2 & 1 & -3 \\ 
4 & -2 & 1 
\end{vmatrix}$$

Expanding this along the top row:


$$= \mathbf{i}((1)(1) - (-3)(-2)) - \mathbf{j}((2)(1) - (-3)(4)) + \mathbf{k}((2)(-2) - (1)(4))$$

$$= \mathbf{i}(1 - 6) - \mathbf{j}(2 - (-12)) + \mathbf{k}(-4 - 4)$$

$$= \mathbf{i}(-5) - \mathbf{j}(14) + \mathbf{k}(-8)$$

So, the cross product is $[-5, -14, -8]$.

**d) The angle between vectors $\vec{a}$ and $\vec{b}$**

The angle $\theta$ between two vectors can be found using the dot product formula: $\vec{a} \cdot \vec{b} = |\vec{a}| |\vec{b}| \cos(\theta)$.

Rearranging to solve for $\cos(\theta)$:


$$\cos(\theta) = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}| |\vec{b}|}$$

$$\cos(\theta) = \frac{3}{\sqrt{14} \cdot \sqrt{21}}$$

$$\cos(\theta) = \frac{3}{\sqrt{294}} = \frac{3}{7\sqrt{6}}$$

Now, solve for $\theta$:


$$\cos(\theta) \approx 0.17496$$

$$\theta = \arccos(0.17496)$$

$$\theta \approx 79.92^\circ \text{ (or } 1.395 \text{ radians)}$$