# General Astronomy HW5

b09902004 資工四 郭懷元

## Problem 1

### a

Let $p = 1.77\ \text{days}$, $r=421700 \ \text{km}$

$$
p^2 = \frac{4 \pi^{2} r^{3}}{GM}
\rArr M = \frac{4 \pi^2 r^3}{G p^2}
\approx 1.897 \times 10^{30} \ \text{g}
$$

### b

> References
>
> 1. [Leverrier, M. "On the masses of the planets, and the parallax of the Sun." Monthly Notices of the Royal Astronomical Society, Vol. 32, p. 322 32 (1872): 322.](https://adsabs.harvard.edu/full/1872MNRAS..32..322L)
> 2. [Anderson, J. D., L. Efron, and G. E. Pease. "Mass, Dynamical Oblateness, and Position of Venus as Determined by Mariner V Tracking Data." The Astronomical Journal Supplement 73 (1968): 162.](https://ui.adsabs.harvard.edu/abs/1968AJS....73R.162A/abstract)
> 3. [Lyttleton, Raymond Arthur. History of the mass of Mercury. No. NASA-CR-163438. 1980.](https://ui.adsabs.harvard.edu/abs/1980QJRAS..21..400L/abstract)

Before we can send instruments into the space, astronomers used those planet's gravitational effect on other object's orbit to calculate their masses. For Mercury, some of the earliest results used the perturbation of a comet's orbit; for Venus, they used the perturbation of other planets such as Mars.

Nowadays we measure the velocity of a space probe that is effected by our target planet's gravitational field to calculate gravity, and then infer its mass.

---

## Problem 2

### a

The cooling rate of molecular clouds of early universe should be **lower**.

Almost all atoms in the early universe are not metallic, therefore the aforementioned molecules should be rare and their total effect on cooling were much less than now.

### b

Lower cooling rate should result in **higher temperature** of molecular clouds, since the heat from collapse is removed at a slower rate.

Therefore the temperature of molecular cloud at early universe should be higher that that of the current Milky Way.

<div style="page-break-before: always;"></div>

### c

Higher molecular cloud temperature would result in higher Jeans mass, because a higher gravitational force is needed to make the gas mass collapse.

### d

The stars formed in early universe should have higher mass than stars forming in the Milky Way now.

We have concluded that the Jeans mass in early universe is higher. Higher Jeans mass means that more molecules (more mass) are needed to start the star formation process, thus the stars would have higher mass.

---

## Problem 3

### a

Differentiating both sides yields:

$$
|d E_\text{gravity}| = \frac{GM^2}{r^2} dr
$$

### b

First:

$$
d E_\text{thermal} = nkT dV = (4 \pi k) \cdot (nTr^2) dr
$$

At equilibrium:

$$
\begin{align*}
    |d E_\text{gravity}| &= d E_\text{thermal} \\
    \frac{GM^2}{r^2} dr &= (4 \pi k) \cdot (nTr^2) dr \\
    M^2 &= \frac{4\pi k}{G} nTr^4 \\
    M &\propto n^{\frac{1}{2}} T^{\frac{1}{2}} r^2 \\
\end{align*}
$$

We also have the following relation:

$$
\begin{align*}
    M &= \frac{4}{3} \pi r^3 \cdot n \cdot m_\text{particle} \\
    M &\propto nr^3 \\
    r &\propto \frac{M}{n}^{\frac{1}{3}}
\end{align*}
$$

Substituting $r$ yields:

$$
\begin{align*}
M &\propto n^{\frac{1}{2}} T^{\frac{1}{2}} \frac{M}{n}^{\frac{2}{3}} \\
M^{\frac{1}{3}} &\propto n^{\frac{-1}{6}} T^{\frac{1}{2}} \\
M &\propto (\frac{T^3}{n})^{\frac{1}{2}}
\end{align*}
$$

---
<div style="page-break-before: always;"></div>

## Problem 4

### a

No. Pluto and Charon are actually tidally locked to each other, meaning that the apparent position of Charon seen from Pluto is always the same and vice versa.

### b

Nitrogen ice.

### c

Water ice.

### d

Yes. The atmosphere is visually thicker compared to that of Earth. The surface pressure also has a much higher variation than other objects in the solar system.

---

## Problem 5

> References:
>
> 1. [Hawking radiation - Wikipedia](https://en.wikipedia.org/wiki/Hawking_radiation)
> 2. [General Astronomy/Black Holes/Hawking Radiation - Wikibooks, open books for an open world](https://en.wikibooks.org/wiki/General_Astronomy/Black_Holes/Hawking_Radiation)
> 3. [Lopresto, Michael (May 2003). "Some Simple Black Hole Thermodynamics" (PDF). The Physics Teacher. 41 (5): 299–301.](https://web.stanford.edu/~oas/SI/SRGR/lib/BlackHoleThermoShort.pdf)
> 4. [Hawking, S. W. (1975). Particle creation by black holes. Communications in mathematical physics, 43(3), 199-220.](https://link.springer.com/article/10.1007/BF02345020)
> 5. [Black Holes and the Structure of Spacetime by Juan Maldacena - YouTube](https://www.youtube.com/watch?v=d7HuP_abpKU)
> 6. [Hawking Radiation](https://jila.colorado.edu/~ajsh/bh/hawk.html)

### a

An oversimplified illustration of the mechanism is that:

1. Our quantum theory says that in the vacuum, a pair of particles, one with positive energy and the other with negative energy, can be created. Under normal circumstances, these two particles would annihilate each other.
2. If the particle pair is created just outside the event horizon of a black hole, the negative particle may cross the event horizon and enter the black hole, while the positive particle goes the other way.
3. For an observer outside, it looks like the black hole is emitting particles that carries energy. This is "Hawking radiation".

### b

We have the formula for Hawking radiation temperature

$$
T_{M = 10^9 M_\odot} = \frac{\hbar c^3}{8 \pi k_B G M}
= \frac{\hbar c^3}{8 \pi k_B G \cdot 10^9 M_\odot}
\approx 6.170 \times 10^{-17} \ \text{K}
$$

<div style="page-break-before: always;"></div>

### c

By Stefan-Boltzmann law, we have:

$$
\begin{align*}
    L_{M = 10^9 M_\odot} &= A \cdot f \\
    &= 4 \pi r_s^2 \cdot \sigma T^4 \\
    &= \frac{16 \pi \sigma G^2}{c^4} M^2 T_{M = 10^9 M_\odot}^4 \\
    &\approx 9.01 \times 10^{-47} \text{Watts} \\
    &\approx 2.35 \times 10^{-73} L_\odot
\end{align*}
$$

### d

For a black hole of mass $10^9 M_\odot$, it should be nearly impossible to detect its Hawking radiation.

Considering the luminosity, even if the black hole is only $1 \ \text{AU}$ away from us, the apparent magnitude would be more thatn 100. Not to mention that the Schwarzschild radius of such black hole is about $19.74 \ \text{AU}$, so the optimal apparent magnitude is even larger.

---
