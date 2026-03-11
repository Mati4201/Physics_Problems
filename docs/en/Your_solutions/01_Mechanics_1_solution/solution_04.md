In vector calculus, we treat each direction ($x$ and $y$) independently when differentiating. If we know where an object is, its **velocity** is how its position changes over time, and its **acceleration** is how its velocity changes over time.

---

## The Solution

### 1. The Position Vector

We are given the position $\vec{r}(t)$ in terms of unit vectors $\hat{i}$ (horizontal) and $\hat{j}$ (vertical):


$$\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$$

### 2. Finding Velocity ($\vec{v}$)

Velocity is the first derivative of position with respect to time ($t$). We apply the power rule ($d/dt [t^n] = nt^{n-1}$) to each component:

* **Horizontal component ($x$):** $\frac{d}{dt}(3t^2) = 6t$
* **Vertical component ($y$):** $\frac{d}{dt}(5t - 8t^2) = 5 - 16t$

Combining these back into a vector:


$$\vec{v}(t) = \mathbf{(6t)\hat{i} + (5 - 16t)\hat{j}}$$

### 3. Finding Acceleration ($\vec{a}$)

Acceleration is the derivative of velocity. We differentiate our previous result:

* **Horizontal component ($v_x$):** $\frac{d}{dt}(6t) = 6$
* **Vertical component ($v_y$):** $\frac{d}{dt}(5 - 16t) = -16$

Combining these:


$$\vec{a}(t) = \mathbf{6\hat{i} - 16\hat{j}}$$

---

## Explanation of Symbols

* **$\vec{r}(t)$**: The position vector. It tells you exactly "where" the object is at any time $t$.
* **$\hat{i}$ and $\hat{j}$**: These are direction markers. $\hat{i}$ means "along the x-axis" and $\hat{j}$ means "along the y-axis."
* **$\vec{v}(t)$**: The velocity vector. Its magnitude tells you the speed, and its direction tells you where the object is heading. Note that it depends on $t$, so the speed changes as time passes.
* **$\vec{a}(t)$**: The acceleration vector. In this specific problem, the acceleration is **constant** ($6$ and $-16$ don't have a $t$ next to them), meaning the "push" on the object never changes.

---

