
## Question 10: 3D Kinematics

**The Setup**
Point M moves according to the 3D vector:


$$\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)$$


*(Where $a, b,$ and $\omega$ are positive constants)*

**What do these symbols mean?**

* **$a$ and $b$:** These stretch the $x$ and $y$ directions. If $a$ and $b$ were equal, the path would be a perfect circle. Because they are different, it's an oval (ellipse).
* **$\omega$ (omega):** The angular frequency. It dictates how fast the object spins around the $z$-axis.
* **$bt$:** The $z$-coordinate grows constantly over time, meaning the object is rising at a steady speed.

### a) Equation of the Trajectory

To find the physical shape of the path, we look at just the $x$ and $y$ parts and eliminate time ($t$):


$$\frac{x}{a} = \cos(\omega t) \quad \text{and} \quad \frac{y}{b} = \sin(\omega t)$$


Square both sides and add them together using the trig identity $\cos^2(\theta) + \sin^2(\theta) = 1$:


$$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1$$


This is the standard equation for an **ellipse**. Because the object is also rising along the $z$-axis ($z = bt$), the full 3D shape is an **elliptical helix** (think of a stretched, oval-shaped spring).

### b) Path Length

The path length $L$ is the integral of the object's speed from $t=0$ to $t=t_0$.
First, find the velocity vector (derivative of position):


$$\vec{v}(t) = (-a\omega \sin(\omega t), b\omega \cos(\omega t), b)$$


Next, find the speed (magnitude of velocity):


$$|\vec{v}(t)| = \sqrt{(-a\omega \sin(\omega t))^2 + (b\omega \cos(\omega t))^2 + b^2}$$

$$|\vec{v}(t)| = \sqrt{\omega^2(a^2 \sin^2(\omega t) + b^2 \cos^2(\omega t)) + b^2}$$


Finally, set up the integral:


$$L = \int_{0}^{t_0} \sqrt{\omega^2(a^2 \sin^2(\omega t) + b^2 \cos^2(\omega t)) + b^2} dt$$


*(Note: Because $a \neq b$, this cannot be solved with basic calculus. It results in a special math function called an "incomplete elliptic integral of the second kind".)*

### c) Special Cases to Discuss

* **If $a = b$:** The base ellipse becomes a perfect circle, making the 3D path a standard **circular helix** (like a slinky).
* **If $\omega = 0$:** The sine and cosine parts freeze. The object just moves straight up the $z$-axis in a **straight line**.

---