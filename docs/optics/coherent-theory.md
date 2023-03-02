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

## Spatial Coherence

Extended source, instead of single point source, leads to spatial coherence, which results in decrease of contrast.

### Setup

Suppose two slits separated by $d$, distance between the slits and the screen is $z$, sources are separated by $b$ and $R$ to slits.

$$\Delta\phi=k\left(\sqrt{(x_S-\frac{d}{2})^2+R^2}+\sqrt{(x-\frac{d}{2})^2+D^2}-\sqrt{(x_S+\frac{d}{2})^2+R^2}-\sqrt{(x+\frac{d}{2})^2+D^2}\right)$$

where $x_S$ is the distance source off the axis.

Take Taylor Expansion:

$$\Delta\phi=\frac{kd}{D}(x-x_S\frac{D}{R})$$

Apply paraxial approximation, $U=U_0$, which means plane wave.

Thus we have:

$$I(x)=2I_0(1+\cos\Delta\phi)=2I_0\left(1+\cos\frac{kd}{D}(x-x_S\frac{D}{R})\right)$$

### Intensity Summation

Note that we can sum intensity directly here is because there is no coherence between different points along the source.

Suppose intensity density i.e. intensity contribution per unit length is $\rho_I$, then by integrating over the length $b$

$$I(x)=\int_{\frac{-b}{2}}^{\frac{b}{2}}\rho_I\left(1+\cos\frac{kd}{D}(x-x_S\frac{D}{R})\right)\mathrm{d}x_S$$

$$I(x)=\rho_Ib\left(1+\frac{\sin u}{u}\cos\frac{kd}{D}x\right)$$

where $u=\frac{\pi db}{\lambda R}$.

### Application

Apparently, $\gamma=\frac{\sin u}{u}$. If $u=\pi$, $\gamma=0$, which means incoherence. Although for $u>\pi$, $\gamma$ may be larger than $0$, which is negligible.

Therefore, we define **threshold** to be $u=\pi$, which leads to the following constraint:

$$db\leq\lambda R$$

## Temporal Coherence

Before, we take monocromatic light (single frequence) as granted. However consider light with multiple frequency components, e.g. $k$ as center wavenumber, $\Delta k$ as width, for convenience of calculation.

### Setup

Also, aussme square intensity distribution over $k$, which is $\rho_I$.

In this case, we assume single point source:

$$I(x)=2I_0\left(1+\cos\frac{kd}{D}x\right)$$

Similarly, neglect the coherence between sources with different frequency.

Take intergration over $k$

$$I(x)=\int_{k-\frac{\Delta k}{2}}^{k+\frac{\Delta k}{2}}\rho_I\left(1+\cos\frac{kd}{D}x\right)dk$$

$$I(x)=\rho_Ib\left(1+\frac{\sin u}{u}\cos\frac{kd}{D}x\right)$$

where $u=\frac{xd\Delta k}{2D}$.

Note $\frac{kd}{D}x$ as $\Delta L$, we have: 

$$\Delta L\Delta k\leq 2\pi$$

The spectral width picture and wave-packet picture agree because limited duration in space (time) implies width in wavelength (frequency).

Also, from $\Delta L$, we can calculate number of fringes.