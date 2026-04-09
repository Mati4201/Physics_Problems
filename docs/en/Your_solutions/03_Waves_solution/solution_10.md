## 10. Wave Sources

$$u = \sum \left( \frac{A}{d^\alpha} \right) \sin(k \cdot d - \omega \cdot t)$$



* **$u$ (Total Displacement):** The final calculated height or strength of the wave at a specific point on the canvas. 
* **$\sum$ (Sigma / Summation):** This tells us to add up the individual displacements from *every* active wave source. If you have three sources dropping ripples, you calculate the formula for each one and add the results together.
* **$A$ (Initial Amplitude):** The base strength or height of the wave right at the source before it starts spreading out.
* **$d$ (Distance):** The physical distance from the wave source to the specific point (or pixel) you are measuring.
* **$\alpha$ (Attenuation Coefficient):** This defines how quickly the wave loses energy as it travels. In the term $\frac{A}{d^\alpha}$, if $\alpha$ is high, the wave dies out very close to the source. If $\alpha$ is $0$, the wave travels forever without losing strength.
* **$k$ (Angular Wave Number):** This controls the spatial frequency of the wave. It is related to the wavelength ($\lambda$) by the formula $k = \frac{2\pi}{\lambda}$. A higher $k$ means the ripples are physically closer together.
* **$\omega$ (Angular Frequency):** This controls how fast the wave oscillates over time. It is related to standard frequency ($f$) by the formula $\omega = 2\pi f$. A higher $\omega$ means the source is bobbing up and down much faster.
* **$t$ (Time):** The current time in the simulation. As $t$ increases, the wave propagates outward.