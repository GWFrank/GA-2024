# General Astronomy HW2

b09902004 資工四 郭懷元

Note: I use $M_\odot$ for $M_\text{Sun}$

## Problem 1

Let $\rho$ be the mass density of dark matters in the solar system.

$$
\begin{align*}
    M_{\text{1 AU dark matter}}
    &= V_{\text{1 AU sphere}} \times \rho_{\text{dark matter}} \\
    &= \frac{4\pi}{3} (1\space\text{AU})^3
        \times (6 \times 10^6 \space\frac{M_\odot}{\text{kpc}^3}) \\
    &= \frac{4\pi}{3} \times 6 \times 10^6 \times (
        \frac{1.5 \times 10^8}{3 \times 10^{13} \times 10^3}
    )^3 \space M_\odot \\
    &\approx 3.142 \times 10^{-18} \space M_\odot
\end{align*}
$$

---

## Problem 2

We already know that the mean temperature for CMB $T \approx 3 \space\text{K}$. The maximum temperature on this map would be $T' = T + \Delta{T} \approx 3.0033 \space\text{K}$.

By Wien's law and Doppler's effect:

$$
\begin{gather*}
    \lambda = \frac{0.29 \space\text{cm}\cdot\text{K}}{T} \approx 0.09667 \space\text{cm} \\
    \lambda' = \frac{0.29 \space\text{cm}\cdot\text{K}}{T'} \approx 0.09656 \space\text{cm} \\
    \frac{v_\text{solar system}}{c} = \frac{\Delta{\lambda}}{\lambda} = \frac{\lambda' - \lambda}{\lambda} \\
    v_\text{solar system} = \frac{\lambda' - \lambda}{\lambda} \times c \approx 3.4137 \times 10^5 \space \text{m/s}
\end{gather*}
$$

The solar system is moving at around $3.4137 \times 10^5 \space \text{m/s}$ towards the higher temperature direction.

---

## Problem 3

### (a)

$1.036195 \times 10^3 \space\text{km/s}$

### (b)

$5.614492 \times 10^2 \space\text{km/s}$

### (c)

$M_\text{dynamic} = 4.603509 \times 10^{14} \space M_\odot$

### (d)

$M_\text{star} = 3.303712 \times 10^{12} \space M_\odot$

### Source Code

[Rendered ipynb version in secret gist](https://gist.github.com/GWFrank/9b7bbd16d76e1ff11a5f782081dfeab5)

```python
import numpy as np
import pandas as pd
from scipy import constants

virgo_galaxy = pd.read_csv("Virgo_galaxy_catalog.csv")
virgo_galaxy.head()

R_VIRGO = 2 * 10**6 * constants.parsec # m
SOLAR_MASS = 1.9891 * 10**30 # kg

cz_mean = virgo_galaxy["cz"].mean()
print(f"cz_mean: {cz_mean:e} km/s", )

cz_std = virgo_galaxy["cz"].std()
print(f"cz_std: {cz_std:e} km/s")

sigma = cz_std * 1000 # m/s
M_dynamic = ((constants.pi * sigma**2 * R_VIRGO)/constants.G) # kg
print(f"Mass from σ: {M_dynamic/SOLAR_MASS:e} M☉")

def zmag_to_mass(z_mag):
    global solar_mass
    d = 20 * 10**6 # pc
    zmag_abs = z_mag + 5*np.log10(10/d)
    zmag_abs_sun = 4.5
    flux_relative_sun = 10**((zmag_abs_sun-zmag_abs)/2.5)
    return flux_relative_sun # solar mass

mass_arr = virgo_galaxy["zmag"].apply(zmag_to_mass)

M_star = mass_arr.sum()
print(f"Mass from stars: {M_star:e} M☉")
```

---

## Problem 4

### (a)

$$
\begin{gather*}
E = \frac{hc}{\lambda} \\
13.6 \space\text{eV} = \frac{
    (4.14 \times 10^{-15} \space\text{eV}\cdot\text{s}) \times (3 \times 10^8 \space\text{m/s})
}{
    \lambda
} \\
\lambda \approx 9.13 \times 10^{-8} \space\text{m} = 913 \space\r{\text{A}}
\end{gather*}
$$

### (b)

$$
\begin{gather*}
    \lambda \cdot T = 0.29 \space\text{cm}\cdot\text{K} \\
    T \approx 31800 \space\text{K}
\end{gather*}
$$

### (c)

At temperature below $31800 \space\text{K}$, the peak wavelength of SED does not have energy, but a significant portion of SED is still below the required wavelength to ionize hydrogen. We should also consider the total **number** of photons with enough energy compared to hydrogen.
