## Question 1: Projectile Motion

**The Setup**
An object is launched with an initial velocity of **100 m/s** at an angle of **37°** above the horizontal. We assume standard gravity (**9.8 m/s²**) and zero air resistance. For clean calculations, we will use the standard geometric approximations for a 37° angle:

* $\sin(37^\circ) \approx 0.60$
* $\cos(37^\circ) \approx 0.80$

### 1. Differential Equations of Motion

Because we are ignoring air resistance, the only force acting on the projectile after launch is gravity, which pulls it straight down. This means the horizontal and vertical motions are completely independent.

* **Horizontal ($x$) Motion:** There is no horizontal force, so there is zero horizontal acceleration.

$$m\frac{d^2x}{dt^2}=0 \implies \frac{d^2x}{dt^2}=0$$


* **Vertical ($y$) Motion:** Gravity applies a constant downward acceleration ($-g$).

$$m\frac{d^2y}{dt^2}=-mg \implies \frac{d^2y}{dt^2}=-g$$



### 2. Time of Flight

To find out how long the projectile is in the air, we calculate the time it takes for its vertical position ($y$) to return to zero (hitting the ground).

* **The Math:** 
$$t_{flight}=\frac{2v_0\sin(\theta)}{g}$$


* **The Calculation:** 
$$t_{flight}=\frac{2(100)(0.60)}{9.8} \approx 12.24$$


* **Result:** The time of flight is approximately **12.24 s**.

### 3. Maximum Height

The projectile reaches its peak height at the exact moment its vertical velocity becomes zero (right before it starts falling back down).

* **The Math:**

$$H=\frac{v_0^2\sin^2(\theta)}{2g}$$


* **The Calculation:**

$$H=\frac{100^2 \cdot 0.60^2}{2(9.8)} = \frac{10000 \cdot 0.36}{19.6} \approx 183.67$$


* **Result:** The maximum height is approximately **183.67 m**.

### 4. Range

The range is the total horizontal distance the projectile travels. Since the horizontal velocity never changes, we multiply the initial horizontal speed by the total time of flight.

* **The Math:**

$$R=\frac{v_0^2\sin(2\theta)}{g}=\frac{v_0^2(2\sin(\theta)\cos(\theta))}{g}$$


* **The Calculation:**

$$R=\frac{10000(2 \cdot 0.60 \cdot 0.80)}{9.8} = \frac{9600}{9.8} \approx 979.59$$


* **Result:** The total range is approximately **979.59 m**.

---



