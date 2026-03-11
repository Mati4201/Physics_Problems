# Solutions goes here

To solve a projectile motion problem from scratch, we break the motion into two independent parts: **horizontal ($x$)** and **vertical ($y$)**.

### 1. Derive the Differential Equations of Motion

In a vacuum (no air resistance), the only force acting on the projectile after it is fired is **gravity**, which acts straight down.

* **Horizontal ($x$):** There are no horizontal forces ($F_x = 0$).
Using Newton's Second Law ($F = ma$):

$$m\frac{d^2x}{dt^2} = 0 \implies \frac{d^2x}{dt^2} = 0$$



*Interpretation: The horizontal acceleration is zero; the horizontal velocity remains constant.*
* **Vertical ($y$):** The force of gravity acts downward ($F_y = -mg$).

$$m\frac{d^2y}{dt^2} = -mg \implies \frac{d^2y}{dt^2} = -g$$



*Interpretation: The vertical acceleration is a constant $-9.8 \text{ m/s}^2$.*

---

### 2. Determine the Time of Flight ($T$)

First, we find the initial velocity components using trigonometry:

* $v_{0x} = v_0 \cos(37^\circ) = 100 \times 0.8 = 80 \text{ m/s}$
* $v_{0y} = v_0 \sin(37^\circ) = 100 \times 0.6 = 60 \text{ m/s}$

The projectile hits the ground when its vertical position $y(t) = 0$. Using the kinematic equation $y = v_{0y}t - \frac{1}{2}gt^2$:


$$0 = (60)T - \frac{1}{2}(9.8)T^2$$


Factoring out $T$: $T(60 - 4.9T) = 0$.
Since $T=0$ is the launch time, we solve for the other root:


$$T = \frac{60}{4.9} \approx \mathbf{12.24 \text{ s}}$$

---

### 3. Determine the Maximum Height ($H$)

The projectile reaches its peak when its vertical velocity $v_y$ becomes **zero**.
Using the formula $v_y^2 = v_{0y}^2 - 2gH$:


$$0 = (60)^2 - 2(9.8)H$$

$$19.6H = 3600$$

$$H = \frac{3600}{19.6} \approx \mathbf{183.67 \text{ m}}$$

---

### 4. Determine the Range ($R$)

The range is the total horizontal distance traveled during the total time of flight ($T$). Since horizontal velocity is constant:


$$R = v_{0x} \times T$$

$$R = 80 \text{ m/s} \times 12.24 \text{ s} \approx \mathbf{979.2 \text{ m}}$$


*(Note: If using the exact range formula $R = \frac{v_0^2 \sin(2\theta)}{g}$ with $\sin(74^\circ) \approx 0.961$, you get approximately $980.6 \text{ m}$. The slight difference is due to rounding $37^\circ$ components).*

---

### Summary of Variables used:

* $v_0$: Initial launch speed ($100 \text{ m/s}$).
* $v_{0x} / v_{0y}$: Horizontal and vertical parts of that speed.
* $g$: Gravity ($9.8 \text{ m/s}^2$).
* $\frac{d^2x}{dt^2}$: Calculus notation for acceleration (the second derivative of position).
