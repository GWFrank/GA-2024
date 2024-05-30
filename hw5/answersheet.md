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


---

