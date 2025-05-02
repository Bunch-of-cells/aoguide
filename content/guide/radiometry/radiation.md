---
title: Radiation
weight: 1
prev: /guide/radiometry
---

Radiation, or electromagnetic radiation, is a self-propagating wave of the electromagnetic field that carries momentum and radiant energy through space. Radiation with wavelength lying in the visible region of the electromagnetic spectrum is called light. A surface which emits radiation isotropically is called a Lambertian surface.

## Flux

Assume we have some radiation passing through a surface element $dA$. Some of the radiation will leave $dA$ within a solid angle $d \omega$; the angle between $d \omega$ and the normal to the surface is denoted by $\theta$. The amount of energy with frequency in the range [$\nu$, $\nu + d\nu$] entering this solid angle in time $dt$ is

$$\tag{2.1.1} dE_\nu = B_\nu \cos \theta \, dA \, d\nu \, d\omega \, dt$$

Here $B_\nu$ is called the spectral radiance of the radiation at frequency $\nu$ and direction $\theta$. The total radiance is given by

$$\tag{2.1.2} B = \int_0^{\infty} B_\nu \, d\nu $$

The flux density $F$ gives the power of radiation per unit area and is measured in $\mathrm{W \, m^{-2}}$. It is also called irradiance. The spectral flux density $F_\nu$ is the flux density of the radiation in the frequency range [$\nu$, $\nu + d\nu$]. In radio astronomy, spectral flux densities are often measured in Janskys. The flux density is related to the spectral radiance as

$$\tag{2.1.3} F_\nu = \int_S B_\nu \cos \theta \, d\omega $$
$$\tag{2.1.4} F = \int_S B \cos \theta \, d\omega $$

The integral is carried over the surface $S$ through which the flux density is being calculated.

For isotropic radiation, the flux density leaving a spherical surface of radius $r$ is given by

$$F = \int_S B \cos \theta \, d\omega = \int_0^{\pi/2} \int_0^{2\pi} B \cos \theta \sin \theta \, d\theta \,  d\phi$$
$$\tag{2.1.5}  \implies \boxed{F = \pi B}$$

Flux $L$ is the power going through some surface, and is measured in $\mathrm{W}$. The flux emitted by a star into a solid angle $\omega$ is $L = \omega r^2 F$, where $F$ is the flux density at a distance $r$. The total flux is the flux passing through a closed surface encompassing the source, also called the luminosity $L$. If the source radiates isotropically, $L = 4\pi r^2 F$. The luminosity does not depend on the distance, however the flux density is inversely proportional to the square of the distance.

For extended objects, surface brightness $B$ is defined as the flux density per unit solid angle. Here the observer is at the apex of the solid angle.

$$\tag{2.1.6} B = \frac{F}{\omega}$$

Surface brightness is independent of distance. It is equal to radiance of the object if the object emits isotropically.

Name | Symbol | Unit | Description |
-----|--------|------|-------------|
Radiant Energy | $Q$ | $\mathrm{J}$ | Energy of electromagnetic radiation |
Radiant Flux | $L$ | $\mathrm{W}$ | Radiant energy emitted, reflected, transmitted or received, per unit time |
Spectral Flux | $L_\nu$ | $\mathrm{W \, Hz^{-1}}$ | Radiant flux per unit frequency or wavelength |
Radiant Intensity | $I$ | $\mathrm{W \, sr^{-1}}$ | Radiant flux emitted, reflected, transmitted or received, per unit solid angle |
Spectral Intensity | $I_\nu$ | $\mathrm{W \, Hz^{-1} \, sr^{-1}}$ | Radiant intensity per unit frequency or wavelength |
Radiance | $B$ | $\mathrm{W \, m^{-2} \, sr^{-1}}$ | Radiant flux emitted, reflected, transmitted or received by a surface, per unit solid angle per unit projected area. This is sometimes also confusingly called "intensity" |
Spectral Radiance | $B_\nu$ | $\mathrm{W \, m^{-2} \, sr^{-1} \, Hz^{-1}}$ | Radiance of a surface per unit frequency or wavelength. This is sometimes also confusingly called "spectral intensity" |
Irradiance or Flux density | $F$ | $\mathrm{W \, m^{-2}}$ | Radiant flux received by a surface per unit area |
Spectral irradiance or Spectral flux density | $F_\nu$ | $\mathrm{W \, m^{-2} \, Hz^{-1}}$ | Irradiance of a surface per unit frequency or wavelength |
Radiosity | $J$ | $\mathrm{W \, m^{-2}}$ | Radiant flux leaving (emitted, reflected and transmitted by) a surface per unit area |
Spectral radiosity | $J_\nu$ | $\mathrm{W \, m^{-2} \, Hz^{-1}}$ | Radiosity of a surface per unit frequency or wavelength |
Radiant exitance | $M$ | $\mathrm{W \, m^{-2}}$ | Radiant flux emitted by a surface per unit area |
Spectral exitance | $M_\nu$ | $\mathrm{W \, m^{-2} \, Hz^{-1}}$ | Radiant exitance of a surface per unit frequency or wavelength |
Radiant exposure | $H$ | $\mathrm{J \, m^{-2}}$ | Radiant energy received by a surface per unit area |
Spectral exposure | $H_\nu$ | $\mathrm{J \, m^{-2} \, Hz^{-1}}$ | Radiant exposure of a surface per unit frequency or wavelength |

The energy of radiation is quantized in packets called photons. The energy of a photon is given by

$$\tag{2.1.7} E = h \nu$$

where $\nu$ is the frequency of the radiation. The momentum carried by a photon is given by

$$\tag{2.1.8} p = \frac{E}{c} = \frac{h \nu}{c}$$

The energy density of radiation is the amount of energy per unit volume, given by

$$\tag{2.1.9} u = \frac{1}{c} \int_S B d \omega $$

where $B$ is the radiance of the radiation.

For an isotropic source, $u = \frac{4 \pi}{c} B$.

The radiation pressure is the force per unit area exerted by radiation on a surface. It is given by

$$ P = \frac{1}{c} \int_S B \cos \theta \, d\omega $$

For an isotropic source, $P = \frac{1}{3} u$.  The radiation pressure is given by

$$ P = \frac{F}{A} = \frac{L}{A c} $$

where $A$ is the area of the surface. The radiation pressure is equal to the momentum flux density of the radiation.

## Blackbody radiation

A blackbody is an object that does not reflex or scatter any radiation falling on it, but absorbs all the radiation falling on it completely. It emits at all wavelengths isotropically. Kirchoff's definition of a blackbody is an ideal body that neither reflects any light nor allows it to pass through. The emissivity $\epsilon$ of a body is defined as the ratio of the radiation emitted by the body to the radiation emitted by a blackbody of the same shape at the same temperature. The emissivity of a blackbody is 1, while that of a perfect reflector is 0. The emissivity of a real body lies between 0 and 1.

$$\tag{2.1.9} \epsilon = \frac{B}{B_\text{blackbody}}$$

where $B$ is the radiance of the body and $B_\text{blackbody}$ is the radiance of a blackbody at the same temperature.

Kirchoff's law states that the emissivity of a body is equal to its absorptivity $a$. This means that a good absorber is also a good emitter.

Examples of blackbodies are stars, the CMB, and a large cavity with a small hole.

The radiation emitted by a blackbody only depends on its temperature, and follows Planck's law. The spectral radiance of a blackbody at temperature $T$ is given by

$$
\tag{2.1.10} \boxed{
    \begin{aligned}
        B_\nu(T) &= \frac{2 h \nu^3}{c^2} \frac{1}{e^{h\nu / kT} - 1} \\
        B_\lambda(T) &= \frac{2 h c^2}{\lambda^5} \frac{1}{e^{h c / \lambda k T} - 1} \\
    \end{aligned}
}
$$

These two are connected by the relation $B_\nu(T) \, d\nu = -B_\lambda(T) \, d\lambda$.

The total radiance is

$$
\begin{aligned}
B(T) &= \int_0^{\infty} B_\nu(T) \, d\nu \\
&= \frac{2 h}{c^2} \int_0^{\infty} \frac{\nu^3}{e^{h\nu / kT} - 1} \, d\nu \\
&= \frac{2 \pi^4 k^4}{15 h^3 c^2} T^4 \\
\end{aligned}
$$

This gives

$$\tag{2.1.11} \boxed{B = \frac{\sigma}{\pi} \, T^4}$$

We define the Stefan-Boltzmann constant as

$$\tag{2.1.12} \sigma = \frac{2 \pi^5 k^4}{15 h^3 c^2}$$

The flux density for an isotropic source is given by

$$\tag{2.1.13} F(T) = \pi B = \sigma T^4$$

This is known as the Stefan-Boltzmann law.

If the radius of a star is $R$ and its temperature is $T$, then its luminosity is given by

$$\tag{2.1.14} L = 4 \pi R^2 F = 4 \pi^2 R^2 B = 4 \pi R^2 \sigma T^4$$

The spectral luminosity is defined as $L_\lambda = 4 \pi^2 R^2 B_\lambda$. The spectral flux density at a distance $r$ is given by

$$\tag{2.1.15} F_\lambda = \frac{L_\lambda}{4\pi r^2} = \pi B_\lambda \left( \frac{R}{r} \right)^2 $$

The wavelength corresponding to the peak of the blackbody spectrum is given by

$$\frac{d}{d\lambda} B_\lambda(T) = 0 \implies \frac{hc}{\lambda kT} \frac{e^{h c / \lambda k T}}{e^{h c / \lambda k T} - 1} - 5 = 0$$

Redefining $x = \frac{hc}{\lambda kT}$,

$$\frac{x e^x}{e^x - 1} = 5 \implies x = 5 + W_0(-5 e^{-5})$$

where $W_0$ is the principal branch of the Lambert W function. This gives the relation

$$\tag{2.1.16} \boxed{\lambda_\text{peak} T = b_\lambda}$$

Thus $B_\lambda$ peaks at the energy

$$\tag{2.1.17} E = x kT \approx 2.821 \,kT $$

Doing the same analysis for $\nu_\text{peak}$, defining $y = \frac{h \nu}{kT}$, we get

$$\frac{y e^y}{e^y - 1} = 3 \implies y = 3 + W_0(-3 e^{-3})$$

This gives the relation

$$\tag{2.1.18} \boxed{\nu_\text{peak} / T = b_\nu}$$

Thus $B_\nu$ peaks at the energy

$$\tag{2.1.19} E = y kT \approx 4.965 \,kT $$

The reason eq 2.1.17 and 2.1.19 are different is because the peak of the spectrum is not at the same energy for both $\lambda$ and $\nu$. One cannot go from $B_\nu$ to $B_\lambda$ by simply changing the variable. One also needs to multiply by $|d\nu / d\lambda| = c /\lambda^2$, which shifts the peak of the distribution to higher energies. These peaks are the mode energy of a photon.

Equation 2.1.16 and 2.1.18 are together known as Wien's displacement law.

When $\lambda \gg \lambda_\text{peak}$ or $\nu \ll \nu_\text{peak}$, we can use the Rayleigh-Jeans approximation to get

$$\tag{2.1.18} B_\nu(T) \approx \frac{2 \nu^2 kT}{c^2}$$
$$\tag{2.1.19} B_\lambda(T) \approx \frac{2c kT}{\lambda^4}$$

When $\lambda \approx \lambda_\text{peak}$ or $\nu \approx \nu_\text{peak}$, we can use the Wein approximation to get

$$\tag{2.1.20} B_\nu(T) \approx \frac{2 h \nu^3}{c^2} e^{-h\nu / kT}$$
$$\tag{2.1.21} B_\lambda(T) \approx \frac{2 h c^2}{\lambda^5} e^{-h c / \lambda k T}$$

The energy density of blackbody radiation is given by

$$\tag{2.1.22} u(T) = \int_0^{\infty} \frac{4 \pi}{c} B_\nu(T) \, d\nu = \frac{4 \sigma}{c} T^4 = aT^4$$

where $a$ is the radiation constant. The radiation pressure is given by

$$\tag{2.1.23} P = \frac{1}{3} u = \frac{1}{3} a T^4 $$

The number density of photons is given by

$$
\begin{aligned}
n(T) &= \int_0^{\infty} \frac{u_\nu(T)}{h \nu} \, d\nu \\
&= \frac{2}{c^2} \frac{4 \pi}{c} \int_0^{\infty} \frac{\nu^2}{e^{h\nu / kT} - 1} \, d\nu \\
&= \frac{16 \pi k^3 \zeta(3)}{h^3 c^3} T^3 \\
\end{aligned}
$$

Hence,

$$\tag{2.1.24} n(T) = \beta \, T^3$$

where $\beta \approx 2.03 \times 10^7 \mathrm{m^{-3} K^{-3}}$.

The mean photon energy is given by

$$\tag{2.1.25} \langle E \rangle = \frac{u(T)}{n(T)} = \frac{\pi^4}{30 \zeta(3)} kT \approx 2.70 \, kT$$

## Temperature

The effective temperature $T_e$ is defined as the temperature of a blackbody which radiates the same total luminosity as the star.

If we assume at some wavelength $\lambda$ the spectral flux density $F_\lambda$ at the surface of the star is given by Planck's law, we get the brightness temperature $T_b$. Since stars are not ideal blackbodies, $T_b$ depends on the wavelength used.

The temperature giving the best fit for Planck's law in a wavelength range is the color temperature $T_c$ of the object.
