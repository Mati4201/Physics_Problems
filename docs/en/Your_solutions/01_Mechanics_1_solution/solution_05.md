


### 5. Relative Velocity

**The Setup:**
We are dealing with a classic vector addition problem. The boat's actual movement across the Earth (its velocity relative to the shore) is the sum of two vectors:
1. The boat's velocity relative to the water (**5 m/s** at some angle).
2. The water's velocity relative to the shore (**2 m/s** East).

We know the final combined vector needs to point directly **North**. 

---

**Step 1: Determine the Heading (Angle)**
If the boat wants to travel straight North, it has to completely cancel out the river's eastward current. This means the boat must angle itself toward the West so that its *westward* velocity component exactly matches the river's *eastward* velocity.

Let $\theta$ be the angle the boat points West of North. 
* The river's eastward speed is **2 m/s**.
* The boat's westward component is given by $5\sin(\theta)$.

Set these equal to each other to cancel the eastward drift:
$$5\sin(\theta) = 2$$
$$\sin(\theta) = \frac{2}{5} = 0.4$$
$$\theta = \arcsin(0.4) \approx 23.6^\circ$$

The boat should head approximately **23.6° West of North**.

---

**Step 2: Determine the Crossing Time**
To find out how long it takes to cross the river, we only care about the boat's speed in the northward direction. Since part of the boat's **5 m/s** speed is being used to fight the current, its effective northward speed will be less than 5 m/s.

We can find this effective northward speed ($v_{north}$) using the Pythagorean theorem, treating the boat's total speed as the hypotenuse of a right triangle:
$$v_{north}^2 + 2^2 = 5^2$$
$$v_{north}^2 + 4 = 25$$
$$v_{north}^2 = 21$$
$$v_{north} = \sqrt{21} \approx 4.58 \text{ m/s}$$

Now that we have the straight-across speed, we can find the time $t$ it takes to cross the **200 m** wide river using the basic kinematic formula $d = vt$:
$$t = \frac{d}{v_{north}}$$
$$t = \frac{200}{\sqrt{21}} \approx 43.6 \text{ s}$$

It will take the boat approximately **43.6 seconds** to cross the river.

---

