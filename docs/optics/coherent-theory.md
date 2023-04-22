## What is Coherence?

We have discussed the *ideal case* for various interference devices.

The *ideal case* is referring to:

1. Point Source
2. Momochromatic light (single frequency)

Now we are going to study what will happen if the ideal case is not met.

### Contrast

$$\gamma = \frac{I_{max}-I_{min}}{I_{max} + I_{min}}$$

$\gamma$ is defined as the **contrast** in interference pattern.

The lager the contrast, the better the interference pattern.

1. **complete coherence** $\gamma=1$
2. **partial coherence** $0<\gamma<1$
3. **incoherent** $\gamma=0$

In two beam interference, $I(x)=I_0(1+\gamma\cos\phi(x))$

## Spatial Coherence

Extended source, instead of single point source, leads to spatial coherence, which results in decrease of contrast.

### Fringe Shift

Before, in Yong's double slits, the interference field by source (Q) on the axis is $I=I(1+\cos(k\frac{d}{D}x))$.

Now consider another source (A) with distance off the axis $x_0$, what is the interference field by A at position $x$ of the screen? 

$$\Delta\phi(x)=k\left(\sqrt{(x_0-\frac{d}{2})^2+R^2}+\sqrt{(x-\frac{d}{2})^2+D^2}-\sqrt{(x_0+\frac{d}{2})^2+R^2}-\sqrt{(x+\frac{d}{2})^2+D^2}\right)$$

Take Taylor Expansion:

$$\Delta\phi(x)=\frac{kd}{D}(x-x_0\frac{D}{R})$$

Here we denote $\delta x=x_0\frac{D}{R}$ as the fringe shift caused by source shift.

$$N=\frac{\delta x}{\Delta x}=\frac{d}{R\lambda}x_0$$

where $\Delta x=\frac{\lambda D}{d}$ is the fringe distance, $N$ is the number of fringes shifted.

Apply paraxial approximation, $U=U_0$, which means plane wave.

Thus we have:

$$I(x)=I_0(1+\cos\Delta\phi(x))=I_0\left(1+\cos\frac{kd}{D}(x-x_0\frac{D}{R})\right)$$

### Line Source Interference Field

What is the interference field by a line of light souce?

Since they are incoherent, we can directly sum up their intensity field to get the answer.

Suppose intensity density i.e. intensity contribution per unit length is $\rho_I$, then by integrating over the width of the source $b$.

$$I(x)=\int_{\frac{-b}{2}}^{\frac{b}{2}}\rho_I\left(1+\cos\frac{kd}{D}(x-x_0\frac{D}{R})\right)\mathrm{d}x_0$$

$$I(x)=I_0\left(1+\frac{\sin u}{u}\cos\frac{kd}{D}x\right)$$

where $u=\frac{\pi db}{\lambda R}$, $I_0=\rho_Ib$.

### Application

Apparently, $\gamma=\frac{\sin u}{u}$. If $u=\pi$, $\gamma=0$, which means incoherence. Although for $u>\pi$, $\gamma$ may be larger than $0$, but that is negligible.

Therefore, we define **threshold** of coherence to be $u=\pi$, which leads to the constraint:

$$db\leq\lambda R$$

The upper limit of light source width is $b=\lambda\frac{R}{d}$.

### Spatial Coherence Formula

Define $\Delta\theta=d/R$, its geometric meaning is the angle spaned by 2 slits.

The **spatial coherence formula**:

$$b\Delta\theta_0=\lambda$$

Where $\Delta\theta_0=d_0/R$ is the upper limit of $\Delta\theta$.

- $\Delta\theta=\Delta\theta_0$: $\gamma=0$, no coherence.
- $\Delta\theta<\Delta\theta_0$: $\gamma>0$, partial coherence.

## Temporal Coherence

Before, we take monocromatic light (single frequence) as granted. However consider light with multiple frequency components, e.g. $k$ as center wavenumber, $\Delta k$ as width.

### Quasi-mono Chromatic Light

Similarly as in spatial coherence, neglect the coherence between sources with different frequency.

Take intergration over $k$

$$I(x)=\int_{k-\frac{\Delta k}{2}}^{k+\frac{\Delta k}{2}}\rho_I\left(1+\cos\frac{kd}{D}x\right)dk$$

$$I(x)=\rho_Ib\left(1+\frac{\sin u}{u}\cos\frac{kd}{D}x\right)$$

where $u=\frac{xd\Delta k}{2D}$.

Define $\Delta L=\frac{d}{D}x$, we have: 

$$\Delta L\Delta k\leq 2\pi$$

Maximun OPL $L_m=\frac{2\pi}{\Delta k}=\frac{\lambda^2}{|\Delta\lambda|}$.

The spectral width picture and wave-packet picture agree because limited duration in space (time) implies width in wavelength (frequency).

Also, from $\Delta L$, we can calculate number of fringes.

### Temporal Coherence Formula

- Coherent Time: $\tau_0\Delta\nu=1$
- Coherent Length: $L_0=\frac{\lambda^2}{|\Delta\lambda|}$
