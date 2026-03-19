


### 10. Kinematics in 3D

**The Setup:**
We are given the 3D position vector of a point $M$ as a function of time, $t$:
$$\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)$$
Here, $a$, $b$, and $\omega$ are positive constants. We can break this down into three parametric equations:
* $x(t) = a \cos(\omega t)$
* $y(t) = b \sin(\omega t)$
* $z(t) = bt$

---

**Part a) Equation of the trajectory**
To understand the shape of the path, we want to look at the relationship between the $x$ and $y$ coordinates. We can eliminate the time parameter $t$ using the fundamental trigonometric identity $\cos^2(\theta) + \sin^2(\theta) = 1$.

First, rearrange the $x$ and $y$ equations:
$$\frac{x}{a} = \cos(\omega t)$$
$$\frac{y}{b} = \sin(\omega t)$$

Now, square both sides and add them together:
$$\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = \cos^2(\omega t) + \sin^2(\omega t)$$
$$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$$

This is the standard equation for an **ellipse** in the $xy$-plane. Because the $z$-coordinate ($z = bt$) increases linearly over time, the point continuously spirals upward while tracing an ellipse horizontally. 

Therefore, the equation describes an **elliptical helix** resting on the surface of an elliptical cylinder.

---

**Part b) Path length from $t=0$ to $t=t_0$**
The path length $L$ of a curve in 3D space is the integral of the velocity's magnitude (the speed) over the given time interval:
$$L = \int_0^{t_0} |\vec{v}(t)| dt$$

*Step 1: Find the velocity vector $\vec{v}(t)$*
$$\vec{v}(t) = \frac{d\vec{r}}{dt} = \left( \frac{d}{dt}[a \cos(\omega t)], \frac{d}{dt}[b \sin(\omega t)], \frac{d}{dt}[bt] \right)$$
$$\vec{v}(t) = (-a\omega \sin(\omega t), b\omega \cos(\omega t), b)$$

*Step 2: Find the magnitude $|\vec{v}(t)|$*
$$|\vec{v}(t)| = \sqrt{(-a\omega \sin(\omega t))^2 + (b\omega \cos(\omega t))^2 + (b)^2}$$
$$|\vec{v}(t)| = \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2}$$

*Step 3: Set up the integral*
$$L = \int_0^{t_0} \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2} dt$$

**Note:** If $a \neq b$, this is an *elliptic integral of the second kind*. It does not have a simple, closed-form algebraic solution and must be evaluated numerically! 

However, if $a = b$ (a special case we'll discuss below), the math simplifies beautifully:
$$|\vec{v}(t)| = \sqrt{a^2\omega^2 (\sin^2(\omega t) + \cos^2(\omega t)) + b^2} = \sqrt{a^2\omega^2 + b^2}$$
Since the speed is constant, the integral becomes very easy:
$$L = \int_0^{t_0} \sqrt{a^2\omega^2 + b^2} dt = \textbf{t}_0 \sqrt{\textbf{a}^2\omega^2 + \textbf{b}^2}$$

---

**Part c) Code and Special Cases**

**Special Cases:**
1.  **If $a = b$:** The horizontal cross-section becomes a perfect circle ($x^2 + y^2 = a^2$). The trajectory simplifies to a standard **circular helix** (like a regular spring).
2.  **If $\omega$ is very small:** The particle takes a long time to complete a horizontal loop, so the trajectory stretches out vertically into a very steep, wavy line.
3.  **If $b$ approaches zero:** The upward movement stops, and the particle just traces a flat ellipse over and over in the $xy$-plane. (Though the prompt states $b$ is strictly positive, it's a helpful theoretical limit!).

