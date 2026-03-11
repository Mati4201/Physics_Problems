
## Question 7: Elimination of Time & Acceleration

**The Setup**
Parametric equations of the path:
$x(t) = 2t^2$
$y(t) = 3t^3$

**What do these symbols mean?**

* **Parametric Form:** Instead of $y$ being a direct formula of $x$, both $x$ and $y$ are driven by an independent third variable, $t$ (time).
* **Eliminating the parameter:** This means using algebra to remove $t$ completely, leaving us with a standard $y$-versus-$x$ equation that describes the physical shape of the track the object moves on.

**1. Eliminate the parameter $t$**
Let's solve the $x$ equation for $t$ (assuming time $t \ge 0$):


$$x = 2t^2 \implies t^2 = \frac{x}{2} \implies t = \sqrt{\frac{x}{2}}$$


Now substitute this $t$ into the $y$ equation:


$$y = 3\left(\sqrt{\frac{x}{2}}\right)^3 = 3\left(\frac{x}{2}\right)^{3/2} = \frac{3}{2\sqrt{2}} x^{3/2}$$


*(Alternatively, you can square both sides to get rid of the fraction exponent: $y^2 = \frac{9}{8}x^3$. This shape is called a semicubical parabola, which has a sharp point or "cusp" at the origin).*

**2. Kinematic Vectors and Magnitudes**

* **Velocity Vector ($\vec{v}$):** Take the derivative of $x$ and $y$ with respect to $t$.

$$\vec{v}(t) = \frac{dx}{dt}\hat{i} + \frac{dy}{dt}\hat{j} = 4t\hat{i} + 9t^2\hat{j}$$


* **Speed ($|\vec{v}|$):** The magnitude of the velocity vector (using Pythagorean theorem).

$$|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = \sqrt{16t^2 + 81t^4} = t\sqrt{16 + 81t^2}$$


* **Acceleration Vector ($\vec{a}$):** Take the derivative of the velocity vector.

$$\vec{a}(t) = \frac{d\vec{v}}{dt} = 4\hat{i} + 18t\hat{j}$$


* **Acceleration Magnitude ($|\vec{a}|$):**

$$|\vec{a}(t)| = \sqrt{4^2 + (18t)^2} = \sqrt{16 + 324t^2}$$



**3. Is acceleration constant?**
**No.** While the horizontal acceleration is a constant $4$, the vertical acceleration is $18t$. Because time $t$ is still in the equation, the acceleration vector changes both its length and its angle as time ticks forward.

---

