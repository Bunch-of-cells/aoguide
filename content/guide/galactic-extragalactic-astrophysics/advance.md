---
title: Advanced Topics
weight: 5
---

## Recombination and Decoupling

The epoch of recombination is the time at which the baryonic component of the universe goes from being ionized to neutral. The epoch of photon decoupling is the time at which the rate at which the photons scatter from electrons becomes less than the Hubble parameter. Here the universe becomes transparent. The epoch of last scattering is the time at which a typical CMB photon underwent its last scattering from an electron.

In early universe,

$$H + \gamma \leftrightharpoons p + e$$

while the photons are still coupled to the baryonic component. This reaction will be in statistical equillibrium. In statistical equillibrium at temperature $T$, the number density $n_X$ of particles with mass $m_X$ is given by

$$\tag{7.4.1} n_X = g_X \left( \frac{m_X kT}{2 \pi \hbar^2} \right)^{3/2} \, \exp(-\frac{m_X c^2}{kT})$$

when $kT \ll m_X c^2$. Here $g_X$ is the statistical weight of the particle $X$. For electrons, protons and neutrons, $g = 2$. For Hydrogen, $g_H = g_p g_e = 4$.

Since $m_H \approx m_p$ and $Q = (m_p + m_e - m_H)c^2 \approx 13.6 \, \mathrm{eV}$, we get

$$\tag{7.4.2} \frac{n_H}{n_e n_p} = \left( \frac{m_e kT}{2 \pi \hbar^2} \right)^{-3/2} \, \exp(-\frac{Q}{kT})$$

This is called the Saha equation.

We define the fraction ionisation $X$ as

$$\tag{7.4.3} X = \frac{n_p}{n_p + n_H} = \frac{n_e}{n_\text{bary}} = \frac{n_e}{n_\text{bary}}$$

From this we get that $n_H = \frac{1-X}{X} n_p$. For overall charge neutrality, we have $n_e = n_p$. Therefore

$$\tag{7.4.4} \frac{1-X}{X} = n_p \left( \frac{m_e kT}{2 \pi \hbar^2} \right)^{-3/2} \, \exp(-\frac{Q}{kT})$$

We define

$$\eta = \frac{n_\text{bary}}{n_\gamma} = \frac{n_p}{X n_\gamma}$$

For the blackbody spectrum, $n_\gamma = 0.243 \left( \frac{kT}{\hbar c} \right)^3$.

For $X = 0.5$ and $\eta = 5.5 \times 10^{-10}$, we get $T_\text{rec} = 3740 \, \mathrm{K}$ and $z_\text{rec} = 1370$, which is $t = 240,000 \, \mathrm{yrs}$ after bigbang.

The rate of photon scattering is

$$\tag{7.4.5} \Gamma = \frac{c}{\lambda} = n_e \sigma_e c= X (1+z)^3 n_{\text{bary},0} \sigma_e c$$

where $\sigma_e$ is the Thomson cross-section. Since $\frac{H^2}{H_0^2} = \Omega_{\text{m},0} (1+z)^3$, we get

$$\tag{7.4.6} 1+z_\text{dec} \approx \frac{43}{X z_\text{dec}^{3/2}}$$

The redshift of photon decoupling was found to be $z_\text{dec} = 1120$. However, the exact value is somewhat smaller, about $z_\text{dec} = 1090$, for which $T_\text{dec} = 2970 \, \mathrm{K}$ and $t = 371,000 \, \mathrm{yrs}$. The last scattering happened too around this time, $z_\text{ls} \approx z_\text{dec} \approx 1100$.

## Gravitational Lensing

A gravitational lens is matter that bends light from a distant source as it travels towards an observer.

Strong lensing is when there are easily visible distortions, such as the formation of Einstein rings, arcs or multiple images of the same source.

Weak lensing does not produce arcs or muliple images, but only flattens the shape of the source.

Microlensing is when no distortion in shape can be seen but the amount of light recieved from a background object changes.

The impact parameter $\xi$ is the shortest separation between the center of the lens and path of a particular light ray. Here L is the massive object which bends the light emitted from S. The observed images are S$_1$ and S$_2$. Angles $\theta$, $\phi$ and $\beta$ are very  small. The deflection is given by

$$\tag{6.2.1} \alpha = \frac{4GM}{c^2} \frac{1}{\xi}$$

When the source is perfectly aligned with the lens ($\beta = 0$), a ring-like image is formed, called the Einstein ring, having angular radius (called the Einstein radius)

$$\tag{6.2.2} \theta_E = \sqrt{\frac{4GM}{c^2} \frac{D_S - D_L}{D_S D_L}}$$

where $D_S$ is distance to the source and $D_L$ is the distance to the lens.

## Cosmic Distance Ladder

The cosmic distance ladder is a succession of methods by which astronomers determine the distances to celestial objects.

### Trigonometric Parallax

This is based on the apprent yearly back and forth movement of stars in the sky, caused by the orbital motion of Earth. This can measure distances upto ~30pc.

### Statistical Parallax

The sun moves through the LSR with a speed of 20 km/s. Combining the apparent proper motion with observed radial motion allows the estimation of distance to a star cluster. This has been used to find the distance to Hyades.

### Main Sequence Fitting

If the distance to a cluster is known, its HR diagram can be plotted. Another cluster whose distance is to be determined can be plotted on the same HR diagram and compared to get the distance modulus.

### Standard Candles

Standard candles are classes of objects that have a calibrated absolute magnitude $M_V$.

Type Ia supernova is a type of supernova that occurs in binary systems in which one of the stars is a white dwarf. It occurs when the white dwarf exceeds the Chandrasekhar limit. The peak absolute magnitude of every Type Ia supernova is the same, $M_V = -19.3$.

Cepheid variables display a unique property known as the period-luminosity relationship. All cepheids exhibit a linear relationship between their luminosity and period. Another class of stars, RR Lyrae, also exhibit this property. The absolute magnitude of RR Lyrae stars is $M_V = 0.6$.

### Hubble's Law

Edwin Hubble discovered that galaxies move away from us with velocities propotional to their separation, i.e. that the universe is expanding. In terms of the redshift $z = \Delta \lambda / \lambda$,

$$\tag{6.2.3} v = cz = H_0 r$$

where $H_0 = 70 \pm 7$ km/s/Mpc is the Hubble constant, and $r$ is the distance to the galaxy.

## Apparent Superluminal Motion

Naivelym an object moving with $\mu = 0.7 \, \mathrm{mas \, yr^{-1}}$ at a distance of $700 \, \mathrm{Mpc}$gives a tangential velocity of $v_t \approx 7c$, which is not possible. However, this apparent superluminal motion results from relativistic motion close to the line of sight. At time $t_1$, a radio source is at $B_1$ and at time $t_2 = t_1 + \delta t$ at $B_2$, then the photons emitted at $B_1$ at time $t_1$ are detected by the observer at

$$\tag{6.2.4} t_1' = t_1 + \frac{d + v \delta t \cos \theta}{c}$$

where $D$ is the distance from the source to the observer. Photons emitted at $B_2$ at time $t_2$ are detected at

$$\tag{6.2.5} t_2' = t_2 + \frac{(d^2 + v^2 \delta t^2 \cos^2 \theta)^{1/2}}{c} \approx t_2 + \frac{d}{c}$$

where $v \delta t \ll d$. Therfore the time difference between the two photons is

$$\tag{6.2.6} \Delta t = t_2' - t_1' = \delta t (1 - \beta \cos \theta)$$

where $\beta = v/c$. The angle $\theta$ is the angle between the line of sight and the direction of motion of the source.

During the time $\Delta t$, the radio source will move by an angle $\Delta \phi$. Hence the proper motion $\mu$ is

$$\tag{6.2.7} \mu = \frac{\Delta \phi}{\Delta t} = \frac{v \sin \theta}{d(1 - \beta \cos \theta)}$$

This gives the transverse velocity

$$\tag{6.2.8} \beta_t = \frac{\mu d}{c} = \frac{\beta \sin \theta}{1 - \beta \cos \theta}$$

The maximum value of $\beta_t$ occurs when $\theta = \cos^{-1} \beta$. As $\beta \to 1$, $\beta_t \to \infty$.
