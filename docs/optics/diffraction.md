!!! quote "Interference or Diffraction?"
    There is no significant physical distinction between interference and diffraction. It is somewhat customary to speak of interference when considering the superposition of only a few waves and diffraction when treating a large number of waves. Even so, one refers to multiple-beam interference in one context and diffraction from a grating in another.

## Huygens-Fresnel Principle

### Hygens Principle

**Hygens stated**, Each point on a wavefront can be envisaged as a source of secondary spherical wavelets. At any particular time, the shape of the wavefront is supposed to be the envelope of the secondary wavelets.

However, this principle ignores most of each secondary wavelet, retaining only the envelope part. That is to say we don't konw how these different secondary wavelets interact with each other.

### Fresnel's Addition

**Hygens-Fresnel Principle** states that every unobstructed point of a wavefront, at a given instant, serves as a source of spherical secondary wavelets (with the same frequency as that of the primary wave). The amplitude of the optical field at any point beyond is the superposition of all these wavelets (*They interfer with each other*).

!!! note "compare wavelength and aperture"
    By triangle inqueality:

    - $\lambda\geq a$: all interfere constructively, there's only 0th order Principal Maximum on the screen.
    - $\lambda\leq a$: interfere constructively and destructively.

### Kirchhoff Modification

Rigorous equation is:

$$ U(P)= K\iint_\Sigma\frac{U(x,y)e^{ikr}}{r}F(\theta_0,\theta)d\Sigma$$

where

$$\begin{aligned}
    K&=\frac{-i}{\lambda}\\
    F(\theta_0,\theta)&=\frac{\cos\theta_0+\cos\theta}{2}
\end{aligned}$$

## Diffraction Types

Roughly speaking, There are two types of diffraction.

- **Fresnell Diffraction**

    Distances between source, diffraction screen or observation screen is finite, or at least one of them is finite, aka. Near-Field Diffraction.

- **Fraunhoffer Diffraction**

    Distances are infinite. aka. Far-Field Diffraction.

## Fraunhoffer Diffraction

### Derivation

$$r=r_0-\frac{xx^\prime+yy^\prime}{z}$$

where $r_0$ is distance between center of slit and field point P.

Normal incident: $\theta=0$ and $\theta^\prime=0$, thus $F(\theta_0,\theta)=1$.

### Single Slit

$$U(\theta^\prime)=KU_0\frac{e^{ikr_0}}{r_0}\int_{-\frac{a}{2}}^\frac{a}{2}e^{-ik\frac{xx^\prime}{z}}\mathrm{d}x=KU_0a\frac{e^{ikr_0}}{r_0}\frac{\sin\alpha}{\alpha}$$

$\alpha=\frac{\pi a\sin\theta}{\lambda}$.

- Width (half angular width) $\Delta\alpha=\pi\Rightarrow a\Delta\theta=\lambda$

### Rectangular Aperture

Suppose window is a square, then

$$U(x^\prime,y^\prime)=KU_0a_1a_2\frac{e^{ikr_0}}{r_0}\frac{\sin\alpha_1}{\alpha_1}\frac{\sin\alpha_2}{\alpha_2}$$

where $\alpha_1=\frac{\pi a_1\sin\theta_1}{\lambda}$ and $\alpha_2=\frac{\pi a_2\sin\theta_2}{\lambda}$.

$\sin\theta_1=\frac{x^\prime}{z},\sin\theta_2=\frac{y^\prime}{z}$

$$I(x^\prime,y^\prime)=I_0(\mathrm{sinc}^2\alpha_1)(\mathrm{sinc}^2\alpha_2)$$

### Circular Aperture and Resolving Power

$$U(\theta)=U(0)e^{ikr_0}\left(\frac{2J_1(\alpha)}{\alpha}\right)$$

$\alpha=\pi D\sin\theta/\lambda$, $\sin\theta=q/z$.

$J_1(x)$ is the first order Bessel function, at $x=0$, $J_1(x)=\frac{1}{2}$, and its first zero is at $x=1.22\pi$. That is $\Delta\alpha=1.22\pi$ or $\Delta\theta=1.22\frac{\lambda}{D}$

Consider resolution limit by circular aperture diffraction:

- $\Delta\phi$ is angular separation between dot-like objects.
- $\Delta\theta$ is half angular width of Airy Disk (the maximum of the diffraction pattern formed by each dot)

**Resolution Limit** by Rayleigh Criteria: $\Delta\phi=\Delta\theta=1.22\frac{\lambda}{D}$

## N Slits Fraunhoffer Diffraction

$$U(\theta)=u(\theta)N(\theta)=u(0)\mathrm{sinc}\alpha \frac{\sin N\beta}{\sin\beta}$$

where $\beta=\frac{\pi d\sin\theta}{\lambda}$, $d\sin\theta$ is the OPL difference between adjacent slits.

### Characteristic

- Principal Maxima: $\beta=m\pi, m=0,\pm1,\cdots \Leftrightarrow d\sin\theta=m\lambda$
- Zeros of $N(\theta)$: $\beta=\frac{\pi}{N}\cdots\frac{N-1}{N}\pi\cdots\frac{N+1}{N}\pi\cdots$, there are $N-1$ zeros between each adjacent Principal Maxima.
- Missing Order: if $\frac{d}{a}=\frac{m}{n}$, then $m,2m\cdots$th Principal Maxima will be missing.

### 半角宽度

定义半角宽度为主极大到相邻一侧暗线之间的角距离。

- $\theta$ 较小可近似：$\delta\theta=\frac{\lambda}{Nd}$
- $\theta$ 较大：$\delta\theta=\frac{\lambda}{Nd\cos\theta_m}$

### 斜入射

假设入射存在夹角 $\theta_0$，那么有：

- $\alpha=\frac{\pi a}{\lambda}(\sin\theta-\sin\theta_0)$
- $\beta=\frac{\pi d}{\lambda}(\sin\theta-\sin\theta_0)$

## Grating Spectrometer

### Basics

- Dispersion Relation: $\beta=m\pi\Leftrightarrow d\sin\theta=m\lambda$
- The analyzable wavelength limit: $\lambda_{max}=d\sin\theta_{max}\leq d$

### Chromatic Dispersion Power

What's $\Delta\theta$ or $\Delta l$ on screen caused by wavelength difference $\Delta\lambda$?

- Angular Separation: $\Delta\theta=\frac{m}{d\cos\theta_m}\Delta\lambda$. 角色散本领：$\frac{m}{d\cos\theta_m}$
- Linear Separation: $\Delta l=\frac{fm}{d\cos\theta_m}\Delta\lambda$. 线色散本领：$\frac{fm}{d\cos\theta_m}$

### Resolution Limit

$\delta\theta$ is FWHM (半角宽度) of the P.M.

by Rayleigh Criteria, $\delta\theta=\Delta\theta \Rightarrow \frac{\lambda}{Nd\cos\theta_m}=\frac{m}{d\cos\theta_m}\Delta\lambda$. Define $R$ as resolution power.

$$R=\frac{\lambda}{\Delta\lambda}=mN$$

### Free Spectral Range

假设使用 $m$ 级（$m\geq 1$）主极大，$\lambda_{min}$ 与 $\lambda_{max}$ 需要满足 $\frac{\lambda_{min}}{m}\geq\lambda_{max}-\lambda_{min}$

自由光谱程：

- $\Delta\lambda_{FSR}=\frac{\lambda_{min}}{m}=\frac{\lambda_{max}}{m+1}$
- $\Delta\nu_{FSR}=\frac{c}{m\lambda_{max}}=\frac{c}{d\sin\theta_{max}}$

## F-P versus Grating

|            | F-P                                                    | Grating                                              |
| ---------- | ------------------------------------------------------ | ---------------------------------------------------- |
| Parameters | $h,\mathscr F$                                         | $d,N$                                                |
| Dispersion | $m\lambda=2nh$                                         | $d\sin\theta=m\lambda$                               |
| Resolution | $R=m \mathscr F\sim 10^6,m\sim10^4,\mathscr F\sim 100$ | $R=mN\sim 10^{4-5}$                                  |
| FSR        | $\frac{c}{2nh}\sim10^{10} \mathrm{Hz}$                 | $\frac{c}{d\sin\theta_{max}}\sim 10^{14}\mathrm{Hz}$ |
|            |                                                        |                                                      |

## Blazed Grating

特定波长的光可以通过闪耀光栅利用原先不能色散的 0 级主极大，关键之处在于：

- 闪耀角 $\theta_b$ 的存在
- $a\approx d$

对于一个闪耀光栅，照明方式可有为两种：

### 方式一

平行光束垂直光栅平面入射，$\theta$ 为平行光束与光栅平面法线的夹角。

$$\alpha=\frac{\pi}{\lambda}a(sin(\theta-\theta_b)-\sin\theta_b), \beta=\frac{\pi}{\lambda}dsin\theta$$

于是若

$$\lambda_{1b}=2d\sin2\theta_b, 2\lambda_{2b}=2d\sin2\theta_b$$

那么 1 级闪耀波长 $\lambda_{1b}$ 或 2 级闪耀波长 $\lambda_{2b}$ 都能在 $\theta=2\theta_b$ 方向得到唯一的主极大。

### 方式二

平行光束垂直槽平面入射，注意，这种情况下 由于主极大对应的 $\theta$ 的不同，1，2 级闪耀波长也不同。

$$\alpha=\frac{\pi}{\lambda}asin(\theta-\theta_b), \beta=\frac{\pi}{\lambda}d(\sin\theta_b+\sin\theta)$$

$$\lambda_{1b}=2d\sin\theta_b, 2\lambda_{2b}=2d\sin\theta$$
