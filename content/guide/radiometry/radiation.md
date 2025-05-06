---
title: Radiation
weight: 1
prev: /guide/radiometry
---

Stars, galaxies, planets, and even you - everything in the universe emits some sort of radiation. This radiation can be in the form of electromagnetic radiation, such as light, or particles, such as electrons and protons. The study of this radiation is called radiometry. Here, we will be studying about electromagnetic radiation. Electromagnetic radiation is a wave in the electric and magnetic fields, which propagate through space, carrying energy and momentum. These waves can be characterized by a wavelength and frequency. Radiation can be classified on the basis of its wavelength or frequency:

- Radio waves: These are used by your radio and TV sets, and are the longest wavelength radiation.
- Microwaves: These are used in microwave ovens and radar systems.
- Infrared: These are used in remote controls and thermal imaging.
- Visible light: This is the light which we can see with our eyes.
- Ultraviolet: This is what causes sunburns.
- X-rays: These allow X-ray imaging.
- Gamma rays: These are the most energetic forms of radiation.

A surface which emits radiation isotropically (symmetrically in all directions) is called a Lambertian surface.

## Flux

### What is Flux?

Flux describes any effect that appears to pass or travel through a surface or substance. Here, the term flux density $F$ (flux and flux density are often used interchangeably without much thought, even though they're two different things) is the amount of radiant energy (energy carried by the radiation) passing through a unit area per unit time. The units of flux density are $\mathrm{W \, m^{-2}}$. Flux density is also called irradiance.

In astrophysics, we often have to deal with how much energy is being recieved by our telescopes from a star or any other astronomical object. This is where flux becomes important. For example, the flux density of Sun's radiation on earth is called the solar constant, which is about $1365 \mathrm{\, W \, m^{-2}}$.

{{< callout type="remark" >}}
If a surface receives power $P$ from radiation, at an angle $\theta$ to the normal, the flux density $F$ is given by

$$F = \frac{P}{A} \cos \theta$$

where $A$ is the area of the surface. The factor $\cos \theta$ accounts for the fact that the radiation is not perpendicular to the surface. The flux density is maximum when $\theta = 0$, i.e., when the radiation is perpendicular to the surface.
{{< /callout >}}

Now we will define some more useful quantities related to the flow of radiation.

### Radiance

Assume we have some radiation passing through a surface element $dA$. Some of the radiation will leave $dA$ within a solid angle $d \omega$; the angle between $d \omega$ (the direction of outgoing radiation) and the normal to the surface is denoted by $\theta$. The amount of energy with frequency in the range [$\nu$, $\nu + d\nu$] entering this solid angle in time $dt$ is

$$\tag{2.1.1} dE_\nu = B_\nu \cos \theta \, dA \, d\nu \, d\omega \, dt$$

Here the quantity $B_\nu$ is called the spectral radiance of the radiation at frequency $\nu$ and direction $\theta$. The total radiance is given by

$$\tag{2.1.2} B = \int_0^{\infty} B_\nu \, d\nu $$

The spectral flux density $F_\nu$ is the flux density of the radiation in the frequency range [$\nu$, $\nu + d\nu$]. This tells us how much flux is carried by radiation per unit frequency. In radio astronomy, spectral flux densities are often measured in Janskys. The flux density is related to the spectral radiance as

$$\tag{2.1.3} F_\nu = \int_\Omega B_\nu \cos \theta \, d\omega $$
$$\tag{2.1.4} F = \int_\Omega B \cos \theta \, d\omega $$

The integral is carried over the solid angle $\Omega$ through which the flux density is being calculated.

For isotropic radiation, the flux density leaving a spherical surface of radius $r$ is given by

$$F = \int_S B \cos \theta \, d\omega = \int_0^{\pi/2} \int_0^{2\pi} B \cos \theta \sin \theta \, d\theta \,  d\phi$$
$$\tag{2.1.5}  \implies \boxed{F = \pi B}$$

### Luminosity

Flux $L$ is defined as the power going through some surface, and is measured in units of $\mathrm{W}$. The flux emitted by a star (power emitted by the star) into a solid angle $\omega$ is $L = \omega r^2 F$, where $F$ is the flux density at a distance $r$. The total flux passing through a closed surface surrounding the source is known as the luminosity $L$. If the source radiates isotropically, $L = 4\pi r^2 F$. The luminosity does not depend on the distance; this gives that the flux density is inversely proportional to the square of the distance.

### Surface Brightness

For extended objects, surface brightness $B$ is defined as the flux density per unit solid angle. Here, the observer views an extended source and is located at the vertex of the solid angle subtended by the object.

$$\tag{2.1.6} B = \frac{F}{\omega}$$

Surface brightness is independent of distance. It is equal to radiance of the object if the object emits isotropically.

### A List of Radiometric Quantities

Name | Symbol | Unit | Description |
-----|--------|------|-------------|
Radiant Energy | $Q$ | $\mathrm{J}$ | Energy of electromagnetic radiation |
Radiant Flux or Luminosity | $L$ | $\mathrm{W}$ | Radiant energy emitted, reflected, transmitted or received, per unit time |
Spectral Flux or Spectral Luminosity | $L_\nu$ | $\mathrm{W \, Hz^{-1}}$ | Radiant flux per unit frequency or wavelength |
Radiant Intensity | $I$ | $\mathrm{W \, sr^{-1}}$ | Radiant flux emitted, reflected, transmitted or received, per unit solid angle |
Spectral Intensity | $I_\nu$ | $\mathrm{W \, Hz^{-1} \, sr^{-1}}$ | Radiant intensity per unit frequency or wavelength |
Radiance | $B$ | $\mathrm{W \, m^{-2} \, sr^{-1}}$ | Radiant flux emitted, reflected, transmitted or received by a surface, per unit solid angle per unit projected area. This is sometimes also confusingly called "intensity" |
Spectral Radiance | $B_\nu$ | $\mathrm{W \, m^{-2} \, sr^{-1} \, Hz^{-1}}$ | Radiance of a surface per unit frequency or wavelength. This is sometimes also confusingly called "spectral intensity" |
Irradiance or Flux density | $F$ | $\mathrm{W \, m^{-2}}$ | Radiant flux received by a surface per unit area |
Spectral Irradiance or Spectral Flux density | $F_\nu$ | $\mathrm{W \, m^{-2} \, Hz^{-1}}$ | Irradiance of a surface per unit frequency or wavelength |
Radiosity | $J$ | $\mathrm{W \, m^{-2}}$ | Radiant flux leaving (emitted, reflected and transmitted by) a surface per unit area |
Spectral Radiosity | $J_\nu$ | $\mathrm{W \, m^{-2} \, Hz^{-1}}$ | Radiosity of a surface per unit frequency or wavelength |
Radiant Exitance | $M$ | $\mathrm{W \, m^{-2}}$ | Radiant flux emitted by a surface per unit area |
Spectral Exitance | $M_\nu$ | $\mathrm{W \, m^{-2} \, Hz^{-1}}$ | Radiant exitance of a surface per unit frequency or wavelength |
Radiant Exposure | $H$ | $\mathrm{J \, m^{-2}}$ | Radiant energy received by a surface per unit area |
Spectral Exposure | $H_\nu$ | $\mathrm{J \, m^{-2} \, Hz^{-1}}$ | Radiant exposure of a surface per unit frequency or wavelength |

### Properties of Radiation

The energy of radiation is quantized in packets called photons. The energy of a photon is given by

$$\tag{2.1.7} E = h \nu = \frac{h c}{\lambda}$$

where $\nu$ is the frequency of the radiation. The momentum carried by a photon is given by

$$\tag{2.1.8} p = \frac{E}{c} = \frac{h \nu}{c} = \frac{h}{\lambda}$$

The energy density $u$ of radiation (measured in units of $\mathrm{J \, m^{-3}}$) is the amount of energy per unit volume. For an isotropic source having radiance $B$,

$$\tag{2.1.10} \boxed{u = \frac{4 \pi}{c} B}$$

The radiation pressure (measured in units of $\mathrm{Pa}$) is the force per unit area exerted by radiation on a surface. It is given by

$$\tag{2.1.11} \boxed{P = \frac{F}{c} \cos^2 \theta} $$

where $F$ is the flux density of the radiation falling on the surface, and $\theta$ is the angle between the direction of the radiation and the normal to the surface. The factor $\cos^2 \theta$ accounts for the fact that the radiation is not perpendicular to the surface. The radiation pressure is maximum when $\theta = 0$, i.e., when the radiation is perpendicular to the surface.

This shows that radiation can exert measurable forces, especially significant in stellar interiors or solar sails. The radiation pressure is equal to the momentum flux density of the radiation.

For an isotropic source with energy density $u$, the total radiation pressure is given by

$$\tag{2.1.11} P = \frac{1}{3} u = \frac{4\pi}{3c} B$$

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    What is the pressure of radiation from a flux density $F$ falling on a surface which perfectly absorbs all the radiation falling on it? What is the pressure of radiation on a surface which perfectly reflects all the radiation falling on it? Consider the case when the direction of the incoming radiation is perpendicular to the surface.
    {{< /tab >}}

    {{< tab >}}
    The pressure of radiation from a flux density $F$ falling on a surface which perfectly absorbs all the radiation falling on it is

    $$P = \frac{F}{c}$$

    If however, all the radiation falling on the surface is reflected, aside from the pressure due to the incident radiation, there is also a pressure due to the reflected radiation, since the reflected radiation carries momentum away from the surface. The net pressure is given by

    $$ P = P_\text{incident} + P_{emitted} = \frac{F}{c} + \frac{F}{c} = \frac{2F}{c} $$

    Hence the radiation pressure on a perfectly reflecting surface is twice that on a perfectly absorbing surface.
    {{< /tab >}}
{{< /tabs >}}

## Blackbody radiation

### What is a Blackbody?

A blackbody is an object that does not reflect or scatter any radiation falling on it, but absorbs all the radiation falling on it completely. It emits radiation evenly in all directions and at all wavelengths. Kirchoff's definition of a blackbody is an ideal body that neither reflects any light nor allows it to pass through. The emissivity $\epsilon$ of a body is defined as the ratio of the radiation emitted by the body to the radiation emitted by a blackbody of the same shape at the same temperature. The emissivity $\epsilon$ of a blackbody is 1, while that of a perfect reflector is 0. The emissivity of a real body lies between 0 and 1.

$$\tag{2.1.10} \epsilon = \frac{B}{B_\text{blackbody}}$$

where $B$ is the radiance of the body and $B_\text{blackbody}$ is the radiance of a blackbody at the same temperature.

Kirchoff's law states that the emissivity of a body is equal to its absorptivity $a$. This means that a good absorber is also a good emitter. So, a perfect absorber (like a blackbody) is also a perfect emitter.

Examples of blackbodies include stars (which closely approximate blackbody spectra), the cosmic microwave background (a nearly perfect blackbody from the early universe), and laboratory setups like a cavity with a small hole that traps radiation.

The radiation emitted by a blackbody only depends on its temperature, and follows Planck's law. Planck's law describes how the light from a blackbody is spread across different wavelengths or frequencies, depending only on its temperature. The spectral radiance of a blackbody at temperature $T$ is given by

$$
\tag{2.1.11} \boxed{
    \begin{aligned}
        B_\nu(T) &= \frac{2 h \nu^3}{c^2} \frac{1}{e^{h\nu / kT} - 1} \\
        B_\lambda(T) &= \frac{2 h c^2}{\lambda^5} \frac{1}{e^{h c / \lambda k T} - 1} \\
    \end{aligned}
}
$$

These two are connected by the relation $B_\nu(T) \, d\nu = -B_\lambda(T) \, d\lambda$ (the minus sign comes from the fact that as frequency increases, wavelength decreases.).

These equations for spectral radiance can be simplified when the wavelengths in question are much larger than the peak wavelength of the spectrum or when they are approximately equal to the peak wavelength of the spectrum.

When $\lambda \gg \lambda_\text{peak}$ or $\nu \ll \nu_\text{peak}$, we can use the Rayleigh-Jeans approximation

$$\tag{2.1.21} B_\nu(T) \approx \frac{2 \nu^2 kT}{c^2}$$
$$\tag{2.1.22} B_\lambda(T) \approx \frac{2c kT}{\lambda^4}$$

The Rayleigh-Jeans approximation is used often in radio astronomy, where the wavelengths are much larger than the peak wavelength of the blackbody spectrum.

{{< callout type="example" >}}
Derive the Rayleigh-Jeans approximation from Planck's law.
{{% /callout %}}

When $\lambda \approx \lambda_\text{peak}$ or $\nu \approx \nu_\text{peak}$, we can use the Wien approximation

$$\tag{2.1.23} B_\nu(T) \approx \frac{2 h \nu^3}{c^2} e^{-h\nu / kT}$$
$$\tag{2.1.24} B_\lambda(T) \approx \frac{2 h c^2}{\lambda^5} e^{-h c / \lambda k T}$$

### Stefan Boltzmann Law

The total radiance is the spectral radiance integrated over all frequencies. It is given by

$$
\begin{aligned}
B(T) &= \int_0^{\infty} B_\nu(T) \, d\nu \\
&= \frac{2 \pi^4 k^4}{15 h^3 c^2} T^4 \\
\end{aligned}
$$

This gives

$$\tag{2.1.12} B(T) = \frac{\sigma}{\pi} \, T^4$$

Here we have defined a new constant - called the Stefan-Boltzmann constant as

$$\tag{2.1.13} \sigma = \frac{2 \pi^5 k^4}{15 h^3 c^2}$$

It is numerically equal to $\sigma \approx 5.67 \times 10^{-8} \, \mathrm{W \, m^{-2} \, K^{-4}}$.

{{< callout type="math" >}}
{{% details title="The integral can be carried out as follows:" closed="true" %}}

$$
\begin{aligned}
\int_0^{\infty} B_\nu(T) \, d\nu &= \frac{2 h}{c^2} \int_0^{\infty} \frac{\nu^3}{e^{h\nu / kT} - 1} \, d\nu \\
&= \frac{2 h}{c^2} \left( \frac{kT}{h} \right)^4 \int_0^{\infty} \frac{x^3}{e^x - 1} \, dx \\
\end{aligned}
$$

The integral $\int_0^{\infty} \frac{x^3}{e^x - 1} \, dx = \frac{\pi^4}{15}$ is a standard result in mathematics. For the more curious readers, the result can be derived using the Riemann zeta function $\zeta(s)$ and the gamma function $\Gamma(s)$. We can use the following relation:

$$\int_0^{\infty} \frac{x^{s-1}}{e^x - 1} \, dx = \Gamma(s) \zeta(s)$$

For $s=4$, we have $\Gamma(4) = 6$ and $\zeta(4) = \frac{\pi^4}{90}$. Hence,

$$\int_0^{\infty} \frac{x^3}{e^x - 1} \, dx = \Gamma(4) \zeta(4) = 6 \cdot \frac{\pi^4}{90} = \frac{\pi^4}{15}$$

This gives the result

$$\int_0^{\infty} B_\nu(T) \, d\nu = \frac{2 h}{c^2} \left( \frac{kT}{h} \right)^4 \cdot \frac{\pi^4}{15} = \frac{2 \pi^4 k^4}{15 h^3 c^2} T^4$$

{{% /details %}}
{{< /callout >}}

The flux density for an isotropic source is given by (using eq 2.1.5)

$$\tag{2.1.14} \boxed{F(T) = \pi B(T) = \sigma T^4}$$

This is known as the Stefan-Boltzmann law.

If the radius of a star is $R$ and its temperature is $T$, then its luminosity is given by (assuming the star emits isotropically)

$$\tag{2.1.15} L = 4 \pi R^2 F = 4 \pi^2 R^2 B = 4 \pi R^2 \sigma T^4$$

The spectral luminosity is defined as $L_\lambda = 4 \pi^2 R^2 B_\lambda$. The spectral flux density at a distance $r$ is given by

$$\tag{2.1.16} F_\lambda = \frac{L_\lambda}{4\pi r^2} = \pi B_\lambda \left( \frac{R}{r} \right)^2 $$

For a blackbody having surface area $A$, its luminosity is given by

$$\tag{2.1.16} \boxed{L = A \sigma T^4}$$

If the object is not a perfect blackbody, we can still use the Stefan-Boltzmann law, but we need to multiply by the emissivity $\epsilon$ of the object. The luminosity is then given by

$$\tag{2.1.16} L = A \epsilon \sigma T^4$$

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    The flux density of a star on Earth is observed to be $F = 10^{-12} \, \mathrm{W \, m^{-2}}$. The star has a parallax of $4 \, \mathrm{mas}$. From spectroscopic measurements, it is found that the star has an effective temperature of $T = 5000 \, \mathrm{K}$. What is the radius of the star?
    {{< /tab >}}

    {{< tab >}}
    This distance to the star is

    $$ d = \frac{1}{\pi} = 250 \, \mathrm{kpc} $$

    The flux density of the star is given by

    $$ F = \frac{L}{4 \pi d^2} = \frac{4\pi R^2 \sigma T^4}{4 \pi d^2} $$

    Rearranging, we get the radius of the star to be

    $$ R = \frac{d}{T^2} \sqrt{\frac{F}{\sigma}} \approx 1.3 \times 10^9 \, \mathrm{m} \approx 1.9 \, \mathrm{R_\odot} $$

    {{< /tab >}}
{{< /tabs >}}

### Wien's Displacement Law

Hotter objects emit more at higher energies (higher frequencies and lower wavelengths). This can be quantified by Wien's law, which relates the peak wavelength and frequency (wavelength or frequency corresponding to the mode energy of the radiated photons; the wavelength or frequency at which the blackbody emits the most) of the blackbody spectrum to the temperature of the object. The peak of the blackbody spectrum shifts with temperature, and this is described by Wien's displacement law. This is the reason why stars have different colors, and why metals glow red then white when heated.

The wavelength corresponding to the peak of the blackbody spectrum is given by

$$\frac{d}{d\lambda} B_\lambda(T) = 0$$

This gives the relation

$$\tag{2.1.17} \boxed{\lambda_\text{peak} T = b_\lambda}$$

$B_\lambda$ peaks at the energy

$$\tag{2.1.18} E \approx 4.965 \,kT $$

{{< callout type="math" >}}

{{% details title="Taking the derivative gives" closed="true" %}}

Taking the derivative $\frac{d}{d\lambda} B_\lambda (T)$ and defining $x = \frac{hc}{\lambda kT}$, after some algebra we get

$$\frac{x e^x}{e^x - 1} = 5$$

This equation can be solved using the Lambert W function, which gives the solution for $x$ as $x = 5 + W_0(-5 e^{-5}) \approx 4.965$. This gives the value of $b_\lambda = \frac{hc}{kx} \approx 2.898 \times 10^{-3} \mathrm{\, m \, K}$.

The peak energy can be calculated using the relation $E = \frac{hc}{\lambda} = xkT \approx 4.965 \,kT$.

{{% /details %}}
{{< /callout >}}

The frequency corresponding to the peak of the blackbody spectrum is given by

$$\frac{d}{d\nu} B_\nu(T) = 0$$

This gives the relation

$$\tag{2.1.19} \boxed{\nu_\text{peak} / T = b_\nu}$$

$B_\nu$ peaks at the energy

$$\tag{2.1.20} E \approx 2.821 \,kT $$

{{< callout type="math" >}}
{{% details title="Taking the derivative gives" closed="true" %}}

Taking the derivative $\frac{d}{d\nu} B_\nu (T)$ and defining $y = \frac{h\nu}{kT}$, after some algebra we get

$$\frac{y e^y}{e^y - 1} = 3$$

This gives $y = 3 + W_0(-3 e^{-3}) \approx 2.821$. This gives the value of $b_\nu = \frac{ky}{h} \approx 5.879 \times 10^{10} \mathrm{\, Hz \, K}$.

The peak energy can be calculated using the relation $E = h \nu = ykT \approx 2.821 \,kT$.

{{% /details %}}
{{< /callout >}}

The reason eq 2.1.18 and 2.1.20 are different is because the peak of the spectrum is not at the same energy for both $\lambda$ and $\nu$. One cannot go from $B_\nu$ to $B_\lambda$ by simply changing the variable. One also needs to multiply by $|d\nu / d\lambda| = c /\lambda^2$, which shifts the peak of the distribution to higher energies. These peaks are the mode energy of a photon.

Equation 2.1.17 and 2.1.19 are together known as Wien's displacement law.

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    Using Wien's displacement law, determine the peak wavelength of radiation emitted by stars with the following temperatures, and indicate what color they would appear to human eyes:

    a) A red dwarf at 3000 K <br>
    b) A Sun-like star at 5800 K <br>
    c) A blue giant at 25,000 K
    {{< /tab >}}

    {{< tab >}}
    Using Wien's displacement law: $\lambda_\text{peak} = \frac{b_\lambda}{T}$

    a) Red dwarf (3000 K):

    $$\lambda_\text{peak} = \frac{2.898 \times 10^{-3}}{3000} \approx 966 \text{ nm}$$

    This is in the near-infrared range, but the visible spectrum tail extends into red wavelengths, making the star appear red.

    b) Sun-like star (5800 K):

    $$\lambda_\text{peak} = \frac{2.898 \times 10^{-3}}{5800} \approx 500 \text{ nm}$$

    This is in the green part of the visible spectrum, but the full spectrum makes the star appear yellow-white.

    c) Blue giant (25,000 K):

    $$\lambda_\text{peak} = \frac{2.898 \times 10^{-3}}{25000} \approx 116 \text{ nm}$$

    This is in the extreme ultraviolet range, but the visible tail makes the star appear blue.
    {{< /tab >}}
{{< /tabs >}}

### Properties of Blackbody Radiation

The energy density of blackbody radiation is given by

$$\tag{2.1.25} u(T) = \int_0^{\infty} \frac{4 \pi}{c} B_\nu(T) \, d\nu = \frac{4 \sigma}{c} T^4 = aT^4$$

where $a \approx 7.566 \times 10^{-16} \, \mathrm{J \, m^{-3} \, K^{-4}}$ is the radiation constant. The radiation pressure is given by

$$\tag{2.1.26} P = \frac{1}{3} u = \frac{1}{3} a T^4 $$

As stated earlier, energy comes in quantized packets called photons. The number density of photons emitted by a blackbody at temperature $T$ is given by

$$
\begin{aligned}
n(T) &= \int_0^{\infty} \frac{u_\nu(T)}{h \nu} \, d\nu \\
&= \frac{16 \pi k^3 \zeta(3)}{h^3 c^3} T^3 \\
\end{aligned}
$$

Hence,

$$\tag{2.1.27} n(T) = \beta \, T^3$$

where $\beta \approx 2.03 \times 10^7 \mathrm{m^{-3} K^{-3}}$.

{{< callout type="math" >}}

{{% details title="The integral can be carried out as follows:" closed="true" %}}

$$
\begin{aligned}
\int_0^{\infty} \frac{u_\nu(T)}{h \nu} \, d\nu &= \frac{2}{c^2} \frac{4 \pi}{c} \int_0^{\infty} \frac{\nu^2}{e^{h\nu / kT} - 1} \, d\nu \\
&= \frac{2}{c^2} \frac{4 \pi}{c} \left( \frac{kT}{h} \right)^3 \int_0^{\infty} \frac{x^2}{e^x - 1} \, dx \\
\end{aligned}
$$

Using the previously stated relation

$$\int_0^{\infty} \frac{x^{s-1}}{e^x - 1} \, dx = \Gamma(s) \zeta(s)$$

For $s=3$, we have $\Gamma(3) = 2$. This gives the result

$$\int_0^{\infty} \frac{u_\nu(T)}{h \nu} \, d\nu = \frac{2}{c^2} \frac{4 \pi}{c} \left( \frac{kT}{h} \right)^3 \cdot 2 \zeta(3) = \frac{16 \pi k^3 \zeta(3)}{h^3 c^3} T^3$$

{{% /details %}}
{{< /callout >}}

The mean energy of the photons emitted by the blackbody is

$$\tag{2.1.28} \langle E \rangle = \frac{u(T)}{n(T)} = \frac{\pi^4}{30 \zeta(3)} kT \approx 2.70 \, kT$$

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    Find the average energy of the cosmic microwave background (CMB) photons. The CMB is a nearly perfect blackbody radiation from the early universe, with a blackbody temperature of 2.7 K.
    {{< /tab >}}

    {{< tab >}}
    The average energy of the CMB photons can be calculated using the relation

    $$\langle E \rangle \approx 2.70 kT$$

    For $T = 2.7 \, \mathrm{K}$, we have

    $$\langle E \rangle \approx 1.02 \times 10^{-22} \, \mathrm{J} \approx 6.36 \times 10^{-4} \, \mathrm{eV} $$

    This is in the microwave range of the electromagnetic spectrum.
    {{< /tab >}}
{{< /tabs >}}

## Temperature

The temperature of a star can be defined in several ways.

- The effective temperature $T_e$ is defined as the temperature of a blackbody which radiates the same total luminosity as the star. For example, the Sun has a luminosity of $3.846 \times 10^{26} \, \mathrm{W}$ and a radius of $6.96 \times 10^8 \, \mathrm{m}$. The effective temperature of the Sun is given by

$$ T_e = \left( \frac{L}{4 \pi \sigma R^2} \right)^{1/4} \approx 5778 \mathrm{\, K}$$

- If we assume at some wavelength $\lambda$ the spectral flux density $F_\lambda$ at the surface of the star is given by Planck's law, we get the brightness temperature $T_b$. This is the temperature of a blackbody that matches the brightness of the star at that specific wavelength. Since stars are not ideal blackbodies, $T_b$ depends on the wavelength used. This is commonly used in radio astronomy, where the Rayleigh-Jeans approximation is used to find brightness temperature at a specific wavelength/frequency.

- The temperature giving the best fit for Planck's law in a wavelength range is the color temperature $T_c$ of the object.

## Problems

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    $\text{(IOAA 2010)}$ Estimate the effective temperature of the photosphere of the Sun using the naked eye colour of the Sun.
    {{< /tab >}}

    {{< tab >}}
    Using Wien's law,

    $$
    \begin{aligned}
    \lambda_\text{peak} T &= b_\lambda \\
    T &= \frac{b_\lambda}{\lambda_\text{peak}} \\
    &\approx \frac{2.898 \times 10^{-3}}{500 \times 10^{-9}} \, \mathrm{K} = 5800 \mathrm{\, K}\\
    &\approx \boxed{6000 \, \mathrm{K}} \\
    \end{aligned}
    $$

    The temperature is rounded as the peak wavelength has only one significant digit.
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    Find the size of a spherical grain of dust (density $\rho = 5000 \, \mathrm{kg \, m^{-3}}$) which can remain stationary in space due to radiation pressure from the Sun.
    {{< /tab >}}

    {{< tab >}}
    Let the radius of the grain of dust be $R$.
    The radiation pressure of Sun at a distance $r$ is given by

    $$P = \frac{F}{c} = \frac{L}{4 \pi r^2 c}$$

    This gives a radiation force acting on the grain of dust of area $A = \pi R^2$ as

    $$F_r = PA = \frac{L }{4 \pi r^2 c} \pi R^2$$

    The mass of the grain of dust is given by

    $$m = \rho \frac{4}{3} \pi R^3$$

    Hence, the gravitational force acting on the grain of dust is given by

    $$F_g = \frac{GMm}{r^2} = \frac{GM \rho \frac{4}{3} \pi R^3}{r^2}$$

    For the grain of dust to remain stationary, the radiation force must be equal to the gravitational force. Hence,

    $$\frac{L }{4 \pi r^2 c} \pi R^2 = \frac{GM \rho \frac{4}{3} \pi R^3}{r^2}$$

    Rearranging gives

    $$R = \frac{3L}{16 \pi \rho c GM} \approx \boxed{115 \, \mathrm{nm}} $$
    
    {{< /tab >}}
{{< /tabs >}}
