


### 3. Path Intersection

**The Setup:**
We are tracking two people moving along 2D paths defined by parametric equations over time $t$:
* **Alice:** $A(t) = (2+t, 8-3t)$
* **Bob:** $B(t) = (2t-1, 2t+2)$

There is a distinct difference between their *paths intersecting* (crossing the same spatial coordinates, regardless of when) and *colliding* (being at the exact same coordinates at the exact same time).

---

**Step 1: Check for Path Intersection**
To find if their paths cross, we set their $x$-coordinates equal to each other and their $y$-coordinates equal to each other. Because they might arrive at the crossing point at different times, we must use two separate time variables, $t_A$ and $t_B$.

* **x-coordinates:**
    $$2 + t_A = 2t_B - 1$$
    $$t_A = 2t_B - 3$$

* **y-coordinates:**
    $$8 - 3t_A = 2t_B + 2$$

Now, substitute the expression for $t_A$ into the $y$-coordinate equation:
$$8 - 3(2t_B - 3) = 2t_B + 2$$
$$8 - 6t_B + 9 = 2t_B + 2$$
$$17 - 6t_B = 2t_B + 2$$
$$15 = 8t_B$$
$$t_B = 1.875$$

Now plug $t_B$ back in to find $t_A$:
$$t_A = 2(1.875) - 3 = 3.75 - 3 = 0.75$$

Because we found valid, real solutions for both times, **yes, their paths intersect**. To find *where*, plug either time into its respective position equation. For Alice ($t_A = 0.75$):
* $x = 2 + 0.75 = 2.75$
* $y = 8 - 3(0.75) = 8 - 2.25 = 5.75$

The intersection point is **(2.75, 5.75)**.

---

**Step 2: Check for a Collision**
For a collision to occur, Alice and Bob must be at the intersection point at the exact same time. 
Since $t_A = 0.75$ and $t_B = 1.875$, Alice crosses the intersection point before Bob gets there. Therefore, **they do not collide**.

---

**Step 3: Determine Minimum Distance**
Since they don't collide, we need to find the point in time where they are closest to one another. The distance $D$ between them at any shared time $t$ is given by the distance formula:
$$D(t) = \sqrt{(x_A - x_B)^2 + (y_A - y_B)^2}$$

To make the calculus easier, we can minimize the *square* of the distance, $D^2(t)$, which will occur at the exact same time $t$ as the minimum of $D(t)$:
* Difference in $x$: $(2+t) - (2t-1) = 3 - t$
* Difference in $y$: $(8-3t) - (2t+2) = 6 - 5t$

$$D^2(t) = (3 - t)^2 + (6 - 5t)^2$$
$$D^2(t) = (9 - 6t + t^2) + (36 - 60t + 25t^2)$$
$$D^2(t) = 26t^2 - 66t + 45$$

To find the minimum, take the derivative with respect to time and set it to zero:
$$\frac{d(D^2)}{dt} = 52t - 66 = 0$$
$$52t = 66$$
$$t = \frac{66}{52} = \frac{33}{26} \approx \textbf{1.27}$$

They are closest at $t \approx$ **1.27**. To find that minimum distance, plug this time back into the $D^2(t)$ equation:
$$D^2\left(\frac{33}{26}\right) = 26\left(\frac{33}{26}\right)^2 - 66\left(\frac{33}{26}\right) + 45$$
$$D^2 = \frac{1089}{26} - \frac{2178}{26} + \frac{1170}{26} = \frac{81}{26}$$
$$D = \sqrt{\frac{81}{26}} = \frac{9}{\sqrt{26}} \approx \textbf{1.77}$$

The minimum distance between them is approximately **1.77 units**.

---

