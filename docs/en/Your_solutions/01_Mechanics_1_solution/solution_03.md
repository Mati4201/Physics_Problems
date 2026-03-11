

## Question 3: Path Intersection

**1. Do they collide?**
A collision requires equal $x$ and $y$ coordinates at the *same* time $t$.

* Set $x$-coordinates equal: $2 + t = 2t - 1 \implies t = 3$
* Check $y$ at $t = 3$: Alice is at $8 - 3(3) = -1$. Bob is at $2(3) + 2 = 8$.
Since $-1 \neq 8$, **they do not collide.**

**2. Do their paths intersect?**
Eliminate $t$ to find their absolute path equations ($y$ in terms of $x$):

* **Alice:** $t = x - 2 \implies y = 8 - 3(x - 2) \implies y = -3x + 14$
* **Bob:** $t = \frac{x+1}{2} \implies y = 2(\frac{x+1}{2}) + 2 \implies y = x + 3$
Set them equal: $-3x + 14 = x + 3 \implies 4x = 11 \implies x = 2.75$.
Plug $x$ back in: $y = 2.75 + 3 = 5.75$.
**Yes, their paths intersect at $(2.75, 5.75)$.**

**3. Minimum distance**
The distance squared is $D(t)^2 = (x_A - x_B)^2 + (y_A - y_B)^2$:


$$D(t)^2 = (3 - t)^2 + (6 - 5t)^2 = 26t^2 - 66t + 45$$


To find the minimum, take the derivative and set it to zero:


$$\frac{d(D^2)}{dt} = 52t - 66 = 0 \implies t = \frac{33}{26} \approx 1.27 \text{ s}$$


Plug $t = 1.27$ back into the distance formula to get a minimum distance of **$\approx$ 1.76 units**.

---
