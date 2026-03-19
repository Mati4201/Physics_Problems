


### 7. Elimination of Time and Interpretation of Acceleration

**The Setup:**
We are given the parametric equations of a particle's path, meaning both the $x$ and $y$ coordinates are defined by a third variable, time $t$:
$$x(t) = 2t^2$$
$$y(t) = 3t^3$$

---

**Step 1: Eliminate the parameter $t$**
To find the direct mathematical relationship between $x$ and $y$ (the path equation), we need to eliminate $t$. 

First, solve for $t$ using the $x(t)$ equation. Assuming $t \geq 0$ (since time is usually positive in these kinematics problems):
$$x = 2t^2 \implies t^2 = \frac{x}{2} \implies t = \sqrt{\frac{x}{2}}$$

Next, substitute this expression for $t$ into the $y(t)$ equation:
$$y = 3\left(\sqrt{\frac{x}{2}}\right)^3 = 3\left(\frac{x}{2}\right)^{3/2}$$

*(Alternatively, you can cube the $x$ equation and square the $y$ equation to see that $\frac{x^3}{8} = t^6$ and $\frac{y^2}{9} = t^6$, meaning $y^2 = \frac{9}{8}x^3$.)*

---

**Step 2: Draw the trajectory**
The equation $y = 3(x/2)^{3/2}$ (or $y^2 \propto x^3$) describes a specific type of curve known as a **semi-cubical parabola**. If we plot this on an $xy$-plane for $t \geq 0$, it starts at the origin $(0,0)$ and curves upward and to the right, getting steeper as $x$ increases. If $t$ can be negative, the curve has a sharp point (a cusp) at the origin and mirrors itself in the fourth quadrant.

---

**Step 3: Calculate velocity vector and magnitude**
Velocity is the time derivative of the position vector $\vec{r}(t) = (2t^2, 3t^3)$.
* **Velocity vector $\vec{v}(t)$:**
  $$v_x(t) = \frac{d}{dt}(2t^2) = 4t$$
  $$v_y(t) = \frac{d}{dt}(3t^3) = 9t^2$$
  $$\vec{v}(t) = (4t)\hat{i} + (9t^2)\hat{j}$$

* **Velocity magnitude $|\vec{v}(t)|$ (speed):**
  Use the Pythagorean theorem on the velocity components:
  $$|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = \sqrt{16t^2 + 81t^4}$$
  Factoring out $t^2$ from inside the square root (assuming $t \geq 0$):
  $$|\vec{v}(t)| = t\sqrt{16 + 81t^2}$$

---

**Step 4: Calculate acceleration vector and magnitude**
Acceleration is the time derivative of the velocity vector.
* **Acceleration vector $\vec{a}(t)$:**
  $$a_x(t) = \frac{d}{dt}(4t) = 4$$
  $$a_y(t) = \frac{d}{dt}(9t^2) = 18t$$
  $$\vec{a}(t) = 4\hat{i} + 18t\hat{j}$$

* **Acceleration magnitude $|\vec{a}(t)|$:**
  $$|\vec{a}(t)| = \sqrt{(4)^2 + (18t)^2} = \sqrt{16 + 324t^2}$$

---

**Step 5: Is the acceleration constant?**
To be constant, the acceleration vector must not change as time changes. Looking at our acceleration vector $\vec{a}(t) = (4, 18t)$, the $x$-component is a constant **4**, but the $y$-component is **18t**, which grows as $t$ grows. 

Because the $y$-component depends on time, the acceleration vector is constantly changing. Therefore, the acceleration is **not constant**.

---

