


### 4. Vector Calculus

**The Setup:**
We are given the position vector of an object as a function of time, $t$:
$$\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$$

In this notation, $\hat{i}$ represents the horizontal ($x$) component and $\hat{j}$ represents the vertical ($y$) component. To find the velocity and acceleration vectors, we need to apply basic calculus—specifically, taking derivatives with respect to time.

---

**Step 1: Find the Velocity Vector**
Velocity is the rate of change of position over time. Mathematically, it is the first derivative of the position vector: 
$$\vec{v}(t) = \frac{d\vec{r}}{dt}$$

We differentiate the $x$ and $y$ components separately:
* **x-component:** $\frac{d}{dt}(3t^2) = 6t$
* **y-component:** $\frac{d}{dt}(5t - 8t^2) = 5 - 16t$

Putting it back together in vector notation, the velocity vector is:
$$\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}$$

---

**Step 2: Find the Acceleration Vector**
Acceleration is the rate of change of velocity over time. It is the first derivative of the velocity vector, or the second derivative of the position vector:
$$\vec{a}(t) = \frac{d\vec{v}}{dt} = \frac{d^2\vec{r}}{dt^2}$$

Again, we differentiate the components of our new velocity vector separately:
* **x-component:** $\frac{d}{dt}(6t) = 6$
* **y-component:** $\frac{d}{dt}(5 - 16t) = -16$

Putting it back into vector notation, the acceleration vector is constant (it does not depend on time $t$):
$$\vec{a}(t) = 6\hat{i} - 16\hat{j}$$

---

