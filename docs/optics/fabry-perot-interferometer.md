## Stokes Relation

British physicist Sir George Gabriel Stokes developled an elegant and novel way of looking at reflection and transmission at a boundary.

The Basic idea is that the process of reflection and transmission is reversible.

Thus we have:

$$\begin{aligned}
    r(\theta_i)+r^\prime(\theta_i)&=0\\
    r^2(\theta_i)+t(\theta_t)t^\prime(\theta_t)&=1
\end{aligned}
$$

Also, by Snell's law: $n_1\sin\theta_i=n_2\sin\theta_t$

## Mulitple Beam Interference

Before, we only consider the double beam because the higher order reflection is negligible. (low reflection of surface)

However, when $r$ (the reflection coefficient) is large, beams reflected between these two surfaces can not be neglected.

$$\begin{aligned}
\delta&=\frac{4\pi nh\cos i}{\lambda_0}\\
I_T&=\frac{I_0}{1+F\sin^2\delta}\\
I_R&=I_0-I_T=\frac{I_0}{1+\frac{1}{F\sin^2\delta}}\\  
\end{aligned}  $$

where $F=\frac{4R}{(1-R)^2}$, **coefficient of finesse**.

If $R\ll1$, $I_T=I_0(1-2R(1-\cos\delta)), I_R=2I_0R(1-\cos\delta)$, which is for a double beam interference.


## Fabry-Perot Interferometer

The Fabry-Perot interferometer is a device that uses the multiple beam interference of light reflected from two extremely flat (order of $\frac{\lambda}{100}$) mirrors.

### Properties

$$\begin{aligned}
\varepsilon &= \frac{4}{\arcsin\sqrt F}\approx\frac{4}{\sqrt F}\\
\mathscr F&=\frac{\pi\sqrt F}{2}\end{aligned}
$$

$\mathscr F$ is **Finesse**.

$\varepsilon$ is **Full Width at Half Maxima** in phase space.

$\delta$ relats phase with measurable parameters, $h,\lambda, i$.

### Etalon as Frequence Selector

The $h$ of an etalon is fixed, and also the case is that the incident angle is fixed, say $i=0$.

$$\begin{aligned}
\delta_m&=2m\pi\\
\lambda_m&=\frac{2nh}{m}\\
\nu_m&=\frac{mc}{2nh}
\end{aligned}$$



So the output would be a group of equally spaced lines in frequence domain, with **free spectral range** defined as: $\Delta\nu=\nu_{m+1}-\nu_m=\frac{c}{2nh}$.

$$\begin{aligned}
\lambda_{FWHM}&=\frac{-\lambda}{m\mathscr F}\\
\nu_{FWHM}&=\frac{c}{m\lambda\mathscr F}
\end{aligned}$$

## Fabry-Perot Spectrometer

In this case, h is not fixed but scanning, i.e. changing in a range, which is achived by a piezo driven by some voltage.

Consider monochromatic light, only certain values of $h$ can detect such light.

$$h_{FWHM}=\frac{\lambda}{n\pi\sqrt F}=\frac{\lambda}{2n\mathscr{F}}$$

### Rayleigh Criteria

Now consider light having various frequency components. As scanning, different frequency componet would pass at different $h$.

For example, light from souce is consist of 2 components $\lambda$ and $\lambda^\prime$. Then $\delta\lambda$ can not be too small, otherwise, we can't tell one from another.

Rayleigh claims that $\delta\lambda\geq\lambda_{FWHM}$ must be granted, that's **Rayleigh Criteria**.

**minimum reslovable wave length** at $\lambda$ is:

$$\delta\lambda=\frac{\lambda}{m\mathscr F}$$

**Resolving power** is defined as:

$$ R\equiv\frac{\lambda}{\delta\lambda}= m\mathscr F$$
