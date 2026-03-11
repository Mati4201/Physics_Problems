To show that $45^\circ$ is the magic number for maximum distance, we need to combine the horizontal and vertical components of motion into one single formula for the **Range ($R$)**, and then use a little calculus to find the "peak" of that formula.

---

### 1. The Setup: Deriving the Range Formula

From the previous problem, we know:

* **Horizontal distance:** $x = (v_0 \cos \theta)t$
* **Vertical position:** $y = (v_0 \sin \theta)t - \frac{1}{2}gt^2$

To find the Range, we set $y = 0$ (the moment it hits the ground) to find the total time of flight ($t$):


$$t = \frac{2v_0 \sin \theta}{g}$$

Now, substitute this time back into the horizontal distance formula:


$$R = (v_0 \cos \theta) \left( \frac{2v_0 \sin \theta}{g} \right)$$

$$R = \frac{v_0^2 (2 \sin \theta \cos \theta)}{g}$$

Using the trigonometric identity $2 \sin \theta \cos \theta = \sin(2\theta)$, we get the standard Range equation:


$$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$

---

### 2. The Optimization: Using Calculus

To find the angle $\theta$ that gives the maximum $R$, we take the derivative of the Range with respect to the angle ($\frac{dR}{d\theta}$) and set it to **zero** (this identifies the "top" of the curve where the slope is flat).

$$\frac{dR}{d\theta} = \frac{d}{d\theta} \left[ \frac{v_0^2 \sin(2\theta)}{g} \right]$$

Since $v_0$ and $g$ are constants, we only differentiate $\sin(2\theta)$:


$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \cos(2\theta) \cdot 2$$

Now, set the derivative to zero:


$$0 = \frac{2v_0^2}{g} \cos(2\theta)$$

---

### 3. The Result

For the equation to equal zero, the cosine term must be zero:


$$\cos(2\theta) = 0$$

We know that $\cos(90^\circ) = 0$. Therefore:


$$2\theta = 90^\circ$$

$$\theta = 45^\circ$$

**Conclusion:** At $45^\circ$, the trade-off between "hanging in the air long enough" (vertical) and "moving forward fast enough" (horizontal) is perfectly balanced, resulting in the maximum possible range.

---

### Understanding the Variables:

* $R(\theta)$: The Range as a function of the angle.
* $\sin(2\theta)$: The part of the formula that changes based on your aim.
* $\frac{dR}{d\theta}$: The "rate of change" of the range; setting it to zero finds the maximum point.

