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

---

## Problem 2

### a

The cooling rate of molecular clouds that form the first stars should be lower. As stated, many molecules that contributes to cooling are consist of metallic atoms.

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
