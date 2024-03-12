# General Astronomy HW1

b09902004 資工四 郭懷元

## Problem 1

> References:
>
> None

### (a)

$$
\begin{gather*}
\begin{align*}
    m-M &= -2.5 \log_{10}{\frac{10 \space \text{pc}}{3000 \times 10^6 \space \text{pc}}} \\
    &= 5 \log_{10}{\frac{3 \times 10^9}{10}}
\end{align*}\\
\begin{align*}
    M &= m - 5 \log_{10}{(3 \times 10^8)} \\
    &= 22 - 5 \times (8 + \log_{10}{3}) \\
    &\approx -20.39
\end{align*}
\end{gather*}
$$

### (b)

Let $R$ be the signal-to-noise ratio.

$$
\begin{gather*}
\frac{N_{\text{photon, SDSS}}}{N_{\text{photon, GMT}}}
= \frac{d_{\text{SDSS}}^2 \cdot t_{\text{SDSS}} \cdot f}{d_{\text{GMT}}^2 \cdot t_{\text{GMT}} \cdot f} = \frac{d_{\text{SDSS}}^2}{d_{\text{GMT}}^2} = (\frac{2.5}{25.4})^2 \\
\frac{R_{\text{SDSS}}}{R_{\text{GMT}}} = \frac{N_{\text{photon, SDSS}}^{0.5}}{N_{\text{photon, GMT}}^{0.5}} = \frac{2.5}{25.4}\\
R_\text{GMT} = R_\text{SDSS} \times \frac{25.4}{25} = 50.8
\end{gather*}
$$

### (c)

Let $f'$ and $m'$ be the flux and magnitude that satisfies the given condition. Let $f$ be the flux of the galaxy observed with SDSS.

$$
\begin{gather*}
\begin{align*}
     & \frac{R_\text{GMT, $t=60$, $m'$}}{R_\text{SDSS, $t=60$, $m=22$}} = \frac{5}{5} = 1 \\
    \rArr & \frac{N_\text{photon, GMT, $60$, $m'$}}{N_\text{photon, SDSS, $60$, $22$}} = 1 \\
    \rArr & \frac{d^2_\text{GMT} \times 60 \times f'}{d^2_\text{SDSS} \times 60 \times f} = 1 \rarr \frac{f'}{f} = (\frac{2.5}{25.8})^2 \\
\end{align*}
\\
\begin{align*}
    m' - m &= -2.5 \log_{10}{\frac{f'}{f}} \\
    m' &= m - 2.5 \log_{10}{\frac{f'}{f}} = 22 - 2.5\log_{10}{(\frac{2.5}{25.8})^2} \approx 27.07 \\
\end{align*}
\end{gather*}
$$

### (d)

Let $t'$ be the time needed.

$$
\begin{gather*}
    \begin{align*}
        \frac{d^2_\text{GMT} \times t' \times f}{d^2_\text{SDSS} \times t \times f} & = 1 \\
        t' & = t \times \frac{d^2_\text{SDSS}}{d^2_\text{GMT}} = 60 \times (\frac{2.5}{25.4})^2 \space\text{sec} = 0.58 \space\text{sec}
    \end{align*}
\end{gather*}
$$
