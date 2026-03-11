To determine if Alice and Bob cross paths or actually smash into each other, we treat their movement as a system of parametric equations. Think of $t$ as the "clock" ticking for both of them.

### 1. Do their paths intersect?

An **intersection** means they both pass through the exact same $(x, y)$ coordinate at *some* point in time, even if they aren't there at the same moment.

We set Alice's coordinates equal to Bob's, using two different time variables ($t_1$ for Alice, $t_2$ for Bob):

* **X-coordinates:** $2 + t_1 = 2t_2 - 1$
* **Y-coordinates:** $8 - 3t_1 = 2t_2 + 2$

From the X equation, we isolate $t_1$:


$$t_1 = 2t_2 - 3$$

Substitute this into the Y equation:


$$8 - 3(2t_2 - 3) = 2t_2 + 2$$

$$8 - 6t_2 + 9 = 2t_2 + 2$$

$$17 - 6t_2 = 2t_2 + 2 \implies 8t_2 = 15 \implies \mathbf{t_2 = 1.875}$$

Now find $t_1$:


$$t_1 = 2(1.875) - 3 = \mathbf{0.75}$$

**Result:** Since we found a valid solution, their paths **do intersect**.
**Where?** Plug $t_1 = 0.75$ into Alice's path: $A(0.75) = (2.75, 5.75)$.

---

### 2. Do they collide?

A **collision** only happens if they reach that intersection point at the **exact same time** ($t_1 = t_2$).

* Alice reaches $(2.75, 5.75)$ at $t = 0.75$.
* Bob reaches $(2.75, 5.75)$ at $t = 1.875$.

Since $0.75 \neq 1.875$, **they do not collide.** Alice passes the point over a second before Bob gets there.

---

### 3. Minimum Distance

Since they don't collide, we want to find when they are closest. We define the distance squared $D^2$ to avoid messy square roots:


$$D^2(t) = (x_B - x_A)^2 + (y_B - y_A)^2$$


Using the same "clock" $t$ for both:


$$\Delta x = (2t - 1) - (2 + t) = t - 3$$

$$\Delta y = (2t + 2) - (8 - 3t) = 5t - 6$$

Substitute these into the distance formula:


$$f(t) = (t - 3)^2 + (5t - 6)^2$$

$$f(t) = (t^2 - 6t + 9) + (25t^2 - 60t + 36) = 26t^2 - 66t + 45$$

To find the minimum, take the derivative and set it to zero:


$$f'(t) = 52t - 66 = 0 \implies \mathbf{t \approx 1.27 \text{ s}}$$

---

### Understanding the Symbols:

* $A(t), B(t)$: The **Position Vectors** of Alice and Bob.
* $t_1, t_2$: Independent time variables used to check if paths cross at *any* time.
* $\Delta x, \Delta y$: The **Separation** between them in the horizontal and vertical directions.
* $f'(t)$: The derivative used to find the "valley" or minimum point of their distance.
