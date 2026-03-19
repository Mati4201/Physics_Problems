 



### 1. Projectile Motion

First, let's establish our initial values. The initial velocity is **100 m/s** and the launch angle is **37°**. We will use standard gravity (**9.8 m/s²**) and the common trigonometric approximations for 37° ($\sin(37^\circ) \approx 0.6$ and $\cos(37^\circ) \approx 0.8$). 

This gives us our initial velocity components:
* Horizontal: $v_{0x} = 100 \times 0.8 =$ **80 m/s**
* Vertical: $v_{0y} = 100 \times 0.6 =$ **60 m/s**

---

**1. Differential Equations of Motion**
Assuming no air resistance, the only force acting on the projectile is gravity, which acts strictly in the vertical direction. Using Newton's Second Law ($F = ma$):

* **Horizontal direction:** There are no horizontal forces.
    $$m\frac{d^2x}{dt^2} = 0 \implies \frac{d^2x}{dt^2} = 0$$

* **Vertical direction:** Gravity pulls the object downward.
    $$m\frac{d^2y}{dt^2} = -mg \implies \frac{d^2y}{dt^2} = -g$$

---

**2. Time of Flight**
By integrating the vertical differential equation twice, we get the equation for vertical position over time:
$$y(t) = v_{0y}t - \frac{1}{2}gt^2$$
The projectile lands when its vertical position is zero ($y(t) = 0$). Setting the equation to zero and solving for $t$ gives the total time of flight:
$$t = \frac{2v_{0y}}{g} = \frac{2(60)}{9.8}$$
The time of flight is approximately **12.24 s**.

---

**3. Maximum Height**
The projectile reaches its maximum height when its vertical velocity is zero ($v_y(t) = 0$). The equation for maximum height $H$ is:
$$H = \frac{v_{0y}^2}{2g} = \frac{60^2}{2(9.8)}$$
The maximum height is approximately **183.67 m**.

---

**4. Range**
By integrating the horizontal differential equation twice, we get the equation for horizontal position over time:
$$x(t) = v_{0x}t$$
The range $R$ is the horizontal distance traveled during the total time of flight ($t \approx 12.24$ s):
$$R = v_{0x}t = 80 \times 12.24$$
The range is approximately **979.2 m**.

---

