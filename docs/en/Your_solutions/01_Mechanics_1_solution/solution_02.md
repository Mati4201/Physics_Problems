
---

## Question 2: Range Optimization

**The Goal**
We need to prove analytically (using calculus) that for any given initial velocity, a projectile will travel the absolute furthest horizontal distance when launched at exactly a **45°** angle.

### The Mathematical Proof

The formula for the horizontal range of a projectile is:


$$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$

To find the maximum value of this function, we need to find where its rate of change (its first derivative) is zero. We take the derivative with respect to the launch angle $\theta$:


$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot 2\cos(2\theta) = 0$$

Because the initial velocity ($v_0$) and gravity ($g$) are constants and not zero, the only way for this entire equation to equal zero is if the cosine part equals zero:


$$\cos(2\theta) = 0$$

In trigonometry, the cosine of an angle is zero at **90°**.


$$2\theta = 90^\circ \implies \theta = 45^\circ$$

To guarantee this is a maximum range (and not a minimum), we check the second derivative. It must be negative:


$$\frac{d^2R}{d\theta^2} = -4 \frac{v_0^2}{g} \sin(2\theta)$$

Plugging in $\theta = 45^\circ$, we get $\sin(90^\circ) = 1$. Since the constants $v_0$ and $g$ are positive, the result of the second derivative is strictly negative. Therefore, **45° gives the absolute maximum horizontal range.**

---