


### 2. Range Optimization

**The Goal:** Show mathematically that the maximum range for a given initial velocity ($v_0$) is achieved when the launch angle ($\theta$) is **45°**. 

**Given:** The formula for the range of a projectile on level ground is:
$$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$
*(Note: $v_0$ and $g$ are constants, so $R$ is solely a function of the launch angle $\theta$.)*

---

**Step 1: Find the first derivative**
To find the maximum value of the function, we need to find its critical points. We do this by taking the first derivative of $R$ with respect to $\theta$ using the chain rule:

$$\frac{dR}{d\theta} = \frac{d}{d\theta} \left( \frac{v_0^2}{g} \sin(2\theta) \right)$$
$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta)$$

---

**Step 2: Set the derivative to zero**
Maximums and minimums occur where the slope of the function is zero. 

$$\frac{v_0^2}{g} \cdot 2\cos(2\theta) = 0$$

Since the initial velocity $v_0$ is not zero and $g$ is a non-zero constant, the only way for this equation to equal zero is if the cosine term equals zero:

$$\cos(2\theta) = 0$$

---

**Step 3: Solve for $\theta$**
For projectile motion, the launch angle $\theta$ is physically restricted between **0°** and **90°** ($0 \leq \theta \leq \pi/2$ radians). This means $2\theta$ must be between **0°** and **180°**. 

The cosine of an angle is zero when the angle is **90°** (or $\pi/2$ rad). Therefore:

$$2\theta = 90^\circ$$
$$\theta = 45^\circ$$

---

**Step 4: Verify it is a maximum (Second Derivative Test)**
To prove this point is a maximum (and not a minimum), we take the second derivative of the range function:

$$\frac{d^2R}{d\theta^2} = \frac{d}{d\theta} \left( \frac{2v_0^2}{g} \cos(2\theta) \right)$$
$$\frac{d^2R}{d\theta^2} = -\frac{4v_0^2}{g} \sin(2\theta)$$

Now, plug in our critical point $\theta = 45^\circ$:

$$\frac{d^2R}{d\theta^2} = -\frac{4v_0^2}{g} \sin(90^\circ) = -\frac{4v_0^2}{g} (1) = -\frac{4v_0^2}{g}$$

Because $v_0^2$ and $g$ are always positive, the second derivative is **negative**. A negative second derivative confirms that the function is concave down at this point, meaning $\theta = 45^\circ$ is indeed the absolute maximum.

---

