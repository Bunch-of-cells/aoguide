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

Flux describes any effect that appears to pass or travel through a surface or substance. Here, the flux $\Phi$ is defined as the radiant power (power associated with the radiation) going through some surface, and is measured in units of $\mathrm{W}$.

The term flux density $F$ (flux and flux density are often used interchangeably without much thought, even though they're two different things) is the amount of radiant energy (energy carried by the radiation) passing through a unit area per unit time. The units of flux density are $\mathrm{W \, m^{-2}}$. Flux density is also called irradiance.

The flux emitted by a spherically symmetric body, such as a star (power emitted by the star) into a solid angle $\omega$ is $\Phi = \omega r^2 F$, where $F$ is the flux density at a distance $r$. The total flux passing through a closed surface surrounding the source is known as the luminosity $L$. Here, $L = 4\pi r^2 F$.

The luminosity is independent of distance; this gives that the flux density is inversely proportional to the square of the distance from the source.

In astrophysics, we often have to deal with how much energy is being recieved by our telescopes from a star or any other astronomical object. This is where flux and flux density becomes important. For example, the flux density of Sun's radiation on earth is called the solar constant, which is about $1365 \mathrm{\, W \, m^{-2}}$.

{{< callout type="remark" >}}
If a surface of surface area $A$ receives flux $\Phi$ from radiation, the flux density $F$ at a point is given by

$$\tag{2.1.1} F = \frac{\partial \Phi}{\partial A}$$

If the surface is illuminated uniformly (flux at each point is the same), then

$$F = \frac{\Phi}{A}$$

If the cross sectional area of the radiation beam (projected surface area) is $A_\text{proj}$, and the radiation is hitting the surface at an angle $\theta$ to the normal, then we have the relation $A_\text{proj} = A \cos \theta$. Therefore the flux density due to radiation becomes

$$\tag{2.1.2} F = \frac{\Phi}{A_\text{proj}} \cos \theta$$
The factor $\cos \theta$ accounts for the fact that the radiation is not perpendicular to the surface. For a given beam, the flux density is maximum when $\theta = 0$, i.e., when the radiation is perpendicular to the surface.
{{< /callout >}}

The spectral flux density $F_\nu$ is the flux density of the radiation in the frequency range [$\nu$, $\nu + d\nu$]. This tells us how much power carried by radiation is passing through unit area per unit frequency. In radio astronomy, spectral flux densities are often measured in Janskys (Jy), where $1 \, \mathrm{Jy} = 10^{-26} \mathrm{\, W \, m^{-2} \, Hz^{-1}}$.

Now we will define some more useful quantities related to the flow of radiation.

### Radiance

Radiance is the radiant flux passing through a given surface, per unit solid angle per unit projected area. Radiance is also called brightness, since this is the quantity that determines how bright an object will appear, independent of its shape, size and other physical properties. It is useful because it indicates how much of the power emitted, reflected, transmitted or received by a surface will be received by an optical system looking at that surface from a specified angle of view.

{{< callout type="remark" >}}
Assume we have some radiation passing through a surface element $dA$. Some of the radiation will leave $dA$ within a solid angle $d \omega$; the angle between $d \omega$ (the direction of outgoing radiation) and the normal to the surface is denoted by $\theta$. If spectral flux or power of radiation with frequency in the range [$\nu$, $\nu + d\nu$] passing through the area is $\Phi_\nu$, then the spectral radiance is defined as

$$\tag{2.1.3} B_\nu = \frac{\partial^2 \Phi_\nu}{\partial \omega \, \partial A_\text{proj}}$$

Here the quantity $B_\nu$ is called the spectral radiance of the radiation at frequency $\nu$ and direction $\theta$. $A_\text{proj} = A \cos \theta$ is the projected area on which the radiation is incident. The total radiance is given by

$$\tag{2.1.4} B = \int_0^{\infty} B_\nu \, d\nu $$
{{% /callout %}}

{{< callout type="image" >}}
{{< svg "images/radiance.svg" "Radiance" "The radiance B is related to the energy passing through a surface element dA into a solid angle dω, in a direction θ (source: Fundamental Astronomy)" >}}
{{% /callout %}}

The flux density is related to the spectral radiance as

$$\tag{2.1.5} F_\nu = \int_\Omega B_\nu \cos \theta \, d\omega $$
$$\tag{2.1.6} F = \int_\Omega B \cos \theta \, d\omega $$

The integral is carried over the solid angle $\Omega$ through which the flux density is being calculated.

For isotropic radiation, the flux density leaving a spherical surface of radius $r$ is given by

$$F = \int_\Omega B \cos \theta \, d\omega = \int_0^{\pi/2} \int_0^{2\pi} B \cos \theta \sin \theta \, d\theta \,  d\phi$$
$$\tag{2.1.7}  \implies \boxed{F = \pi B}$$

### Surface Brightness

For extended objects, surface brightness $B$ is defined as the flux density per unit solid angle. Here, the observer views an extended source and is located at the vertex of the solid angle subtended by the object.

$$\tag{2.1.8} B = \frac{F}{\omega}$$

Surface brightness is independent of distance. It is equal to radiance of the object if the object emits isotropically.

{{< callout type="image" >}}
{{< svg "images/surfbright.svg" "Surface Brightness" "The surface brightness B is the flux received by the observer, divided by the solid angle the object is spread over as seen by the observer" >}}
{{% /callout %}}

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

$$\tag{2.1.9} E = h \nu = \frac{h c}{\lambda}$$

where $\nu$ is the frequency of the radiation. The momentum carried by a photon is given by

$$\tag{2.1.10} p = \frac{E}{c} = \frac{h \nu}{c} = \frac{h}{\lambda}$$

The radiation pressure (measured in units of $\mathrm{Pa}$) is the force per unit area exerted by radiation on a surface. It is given by

$$\tag{2.1.11} \boxed{P = \frac{F}{c} \cos^2 \theta} $$

where $F$ is the flux density of the radiation falling on the surface, and $\theta$ is the angle between the direction of the radiation and the normal to the surface. The factor $\cos^2 \theta$ accounts for the fact that the radiation is not perpendicular to the surface. The radiation pressure is maximum when $\theta = 0$, i.e., when the radiation is perpendicular to the surface. This shows that radiation can exert measurable forces, especially significant in stellar interiors or solar sails.

The energy density $u$ of the radiation source (measured in units of $\mathrm{J \, m^{-3}}$) is the amount of energy stored in it per unit volume. For an isotropic source having radiance $B$,

$$\tag{2.1.12} \boxed{u = \frac{4 \pi}{c} B}$$

For an isotropic source with energy density $u$, the its internal pressure $P$ is

$$\tag{2.1.13} P = \frac{1}{3} u = \frac{4\pi}{3c} B$$

{{< tabs items="P1,Solution" >}}
    {{< tab >}}
    What is the pressure of radiation from a flux density $F$ falling on a surface which perfectly absorbs all the radiation falling on it? What is the pressure of radiation on a surface which perfectly reflects all the radiation falling on it? Consider the case when the direction of the incoming radiation is perpendicular to the surface.
    {{< /tab >}}

    {{< tab >}}
    The pressure of radiation from a flux density $F$ falling on a surface which perfectly absorbs all the radiation falling on it is

    $$P = \frac{F}{c}$$

    If however, all the radiation falling on the surface is reflected, aside from the pressure due to the incident radiation, there is also a pressure due to the reflected radiation, since the reflected radiation carries momentum away from the surface. The net pressure is thus

    $$ P = P_\text{incident} + P_{emitted} = \frac{F}{c} + \frac{F}{c} = \frac{2F}{c} $$

    Hence the radiation pressure on a perfectly reflecting surface is twice that on a perfectly absorbing surface.
    {{< /tab >}}
{{< /tabs >}}

## Blackbody radiation

### What is a Blackbody?

A blackbody is an object that does not reflect or scatter any radiation falling on it, but absorbs all the radiation falling on it completely. It emits radiation evenly in all directions and at all wavelengths. Kirchoff's definition of a blackbody is an ideal body that neither reflects any light nor allows it to pass through. The emissivity $\epsilon$ of a body is defined as the ratio of the radiation emitted by the body to the radiation emitted by a blackbody of the same shape at the same temperature. The emissivity $\epsilon$ of a blackbody is 1, while that of a perfect reflector is 0. The emissivity of a real body lies between 0 and 1.

$$\tag{2.1.14} \epsilon = \frac{B}{B_\text{blackbody}}$$

where $B$ is the radiance of the body and $B_\text{blackbody}$ is the radiance of a blackbody at the same temperature.

Kirchoff's law states that the emissivity of a body is equal to its absorptivity $a$. This means that a good absorber is also a good emitter. So, a perfect absorber (like a blackbody) is also a perfect emitter.

Examples of blackbodies include stars (which closely approximate blackbody spectra), the cosmic microwave background (a nearly perfect blackbody from the early universe), and laboratory setups like a cavity with a small hole that traps radiation.

The radiation emitted by a blackbody only depends on its temperature, and follows Planck's law. Planck's law describes how the light from a blackbody is spread across different wavelengths or frequencies, depending only on its temperature. The spectral radiance of a blackbody at temperature $T$ is given by

$$
\tag{2.1.15} \boxed{
    \begin{aligned}
        B_\nu(T) &= \frac{2 h \nu^3}{c^2} \frac{1}{e^{h\nu / kT} - 1} \\
        B_\lambda(T) &= \frac{2 h c^2}{\lambda^5} \frac{1}{e^{h c / \lambda k T} - 1} \\
    \end{aligned}
}
$$

These two are connected by the relation $B_\nu(T) \, d\nu = -B_\lambda(T) \, d\lambda$ (the minus sign comes from the fact that as frequency increases, wavelength decreases.).

{{< callout type="image" >}}
{{< svg "images/blackbody.svg" "Black Body Radiation Curve" "Black Body Radiation Curve (source: Wikipedia)" >}}
{{% /callout %}}

These equations for spectral radiance can be simplified when the wavelengths in question are much larger than the peak wavelength of the spectrum or when they are approximately equal to the peak wavelength of the spectrum.

When $\lambda \gg \lambda_\text{peak}$ or $\nu \ll \nu_\text{peak}$, we can use the Rayleigh-Jeans approximation

$$\tag{2.1.16} B_\nu(T) \approx \frac{2 \nu^2 kT}{c^2}$$
$$\tag{2.1.17} B_\lambda(T) \approx \frac{2c kT}{\lambda^4}$$

The Rayleigh-Jeans approximation is used often in radio astronomy, where the wavelengths are much larger than the peak wavelength of the blackbody spectrum.

{{< callout type="example" >}}
Derive the Rayleigh-Jeans approximation from Planck's law.
{{% /callout %}}

When $\lambda \lesssim \lambda_\text{peak}$ or $\nu \gtrsim \nu_\text{peak}$, we can use the Wien approximation

$$\tag{2.1.18} B_\nu(T) \approx \frac{2 h \nu^3}{c^2} e^{-h\nu / kT}$$
$$\tag{2.1.19} B_\lambda(T) \approx \frac{2 h c^2}{\lambda^5} e^{-h c / \lambda k T}$$

### Stefan Boltzmann Law

The total radiance is the spectral radiance integrated over all frequencies. It is given by

$$
\begin{aligned}
B(T) &= \int_0^{\infty} B_\nu(T) \, d\nu \\
&= \frac{2 \pi^4 k^4}{15 h^3 c^2} T^4 \\
\end{aligned}
$$

This gives

$$\tag{2.1.20} B(T) = \frac{\sigma}{\pi} \, T^4$$

Here we have defined a new constant - called the Stefan-Boltzmann constant as

$$\tag{2.1.21} \sigma = \frac{2 \pi^5 k^4}{15 h^3 c^2}$$

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

The flux density for an isotropic source is given by (using eq 2.1.7)

$$\tag{2.1.22} \boxed{F(T) = \pi B(T) = \sigma T^4}$$

This is known as the Stefan-Boltzmann law.

If the radius of a star is $R$ and its temperature is $T$, then its luminosity is given by (assuming the star emits isotropically)

$$\tag{2.1.23} L = 4 \pi R^2 F = 4 \pi^2 R^2 B = 4 \pi R^2 \sigma T^4$$

The spectral luminosity is defined as $L_\lambda = 4 \pi^2 R^2 B_\lambda$. The spectral flux density at a distance $r$ is given by

$$\tag{2.1.24} F_\lambda = \frac{L_\lambda}{4\pi r^2} = \pi B_\lambda \left( \frac{R}{r} \right)^2 $$

For a blackbody having surface area $A$, its luminosity is given by

$$\tag{2.1.25} \boxed{L = A \sigma T^4}$$

If the object is not a perfect blackbody, we can still use the Stefan-Boltzmann law, but we need to multiply by the emissivity $\epsilon$ of the object. The luminosity is then given by

$$\tag{2.1.26} L = A \epsilon \sigma T^4$$

{{< tabs items="P2,Solution" >}}
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

$$\tag{2.1.27} \boxed{\lambda_\text{peak} T = b_\lambda}$$

$B_\lambda$ peaks at the energy

$$\tag{2.1.28} E \approx 4.965 \,kT $$

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

$$\tag{2.1.29} \boxed{\nu_\text{peak} / T = b_\nu}$$

$B_\nu$ peaks at the energy

$$\tag{2.1.30} E \approx 2.821 \,kT $$

{{< callout type="math" >}}
{{% details title="Taking the derivative gives" closed="true" %}}

Taking the derivative $\frac{d}{d\nu} B_\nu (T)$ and defining $y = \frac{h\nu}{kT}$, after some algebra we get

$$\frac{y e^y}{e^y - 1} = 3$$

This gives $y = 3 + W_0(-3 e^{-3}) \approx 2.821$. This gives the value of $b_\nu = \frac{ky}{h} \approx 5.879 \times 10^{10} \mathrm{\, Hz \, K}$.

The peak energy can be calculated using the relation $E = h \nu = ykT \approx 2.821 \,kT$.

{{% /details %}}
{{< /callout >}}

The reason eq 2.1.28 and 2.1.30 are different is because the peak of the spectrum is not at the same energy for both $\lambda$ and $\nu$. One cannot go from $B_\nu$ to $B_\lambda$ by simply changing the variable. One also needs to multiply by $|d\nu / d\lambda| = c /\lambda^2$, which shifts the peak of the distribution to higher energies. These peaks are the mode energy of a photon.

Equation 2.1.27 and 2.1.29 are together known as Wien's displacement law.

{{< tabs items="P3,Solution" >}}
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

$$\tag{2.1.31} u(T) = \int_0^{\infty} \frac{4 \pi}{c} B_\nu(T) \, d\nu = \frac{4 \sigma}{c} T^4 = aT^4$$

where $a \approx 7.566 \times 10^{-16} \, \mathrm{J \, m^{-3} \, K^{-4}}$ is the radiation constant. The radiation pressure is given by

$$\tag{2.1.32} P = \frac{1}{3} u = \frac{1}{3} a T^4 $$

As stated earlier, energy comes in quantized packets called photons. The number density of photons emitted by a blackbody at temperature $T$ is given by

$$
\begin{aligned}
n(T) &= \int_0^{\infty} \frac{u_\nu(T)}{h \nu} \, d\nu \\
&= \frac{16 \pi k^3 \zeta(3)}{h^3 c^3} T^3 \\
\end{aligned}
$$

Hence,

$$\tag{2.1.33} n(T) = \beta \, T^3$$

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

$$\tag{2.1.34} \langle E \rangle = \frac{u(T)}{n(T)} = \frac{\pi^4}{30 \zeta(3)} kT \approx 2.70 \, kT$$

{{< tabs items="P4,Solution" >}}
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

{{< tabs items="P5,Solution,IOAA 2010" >}}
    {{< tab >}}
    Estimate the effective temperature of the photosphere of the Sun using the naked eye colour of the Sun.
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

{{< tabs items="P6,Solution" >}}
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

{{< tabs items="P7,Solution" >}}
    {{< tab >}}
    Consider a surface of surface area $A$ and reflection coefficient of $\alpha$, that is it reflects a fraction $\alpha$ of the radiation falling on it. The rest of the radiation is absorbed. The surface is illuminated by radiation of flux density $F$, at an angle $\theta$ to the normal. Find the force exerted on the surface by the radiation.
    {{< /tab >}}

    {{< tab >}}
    Let the normal of the surface be pointing along the $z$-axis, the surface being in the $xy$-plane, and the incoming radiation be in the $zx$-plane, making angle $\theta$ with the $z$-axis. The unit vector corresponding to the direction of the incoming radiation is thus $\hat{i} = \sin \theta \,\hat{x} + \cos \theta \, \hat{z}$. Since the radiation is incident at an angle $\theta$, the projected area of the surface in the direction of the radiation is $A_\text{proj} = A \cos \theta$.

    The flux density incident on the surface is $F$, and that reflected away is $\alpha F$. The reflected radiation will be in the direction $\hat{r} = -\sin \theta \,\hat{x} + \cos \theta \, \hat{z}$, according to the laws of reflection (the angle between incident ray and the normal is equal to the angle between the reflected ray and the normal, and that the incident ray, reflected ray and normal all lie in a single plane).
    
    The force due to incident radiation on the surface is

    $$F_\text{incident} = \frac{F}{c} A_\text{proj} \, \hat{i}$$

    The force due to the reflected radiation is

    $$F_\text{reflected} = \frac{\alpha F}{c} A_\text{proj} \, (-\hat{r})$$

    The direction of the force due to reflected radiation will be opposite to its direction of propagation.

    The net force on the surface is therefore

    $$F_\text{net} = F_\text{incident} + F_\text{reflected} = \frac{F}{c} A_\text{proj} \, \hat{i} + \frac{\alpha F}{c} A_\text{proj} \, (-\hat{r})$$
    $$= \frac{F}{c} A_\text{proj} \left( \hat{i} - \alpha \hat{r} \right)$$
    $$= \frac{F}{c} \, A \cos \theta \, \left[ (1 - \alpha) \sin \theta \, \hat{x} + (1 + \alpha) \cos \theta \, \hat{z} \right]$$

    We see that if the surface is perfectly reflecting ($\alpha = 1$), the force is directed opposite to the normal ($z$-axis), having a magnitude of $\frac{F}{c} A \cos^2 \theta$. Whereas if the surface is perfectly absorbing ($\alpha = 0$), the force is directed along the direction of the incoming radiation, having a magnitude of $\frac{F}{c} A \cos \theta$.

    If $\theta = 0$, that is the radiation is falling normal to the surface, the force experienced by the surface will be opposite to the normal or the direction of incident radiation, having a magnitude of $\frac{F}{c} A \, (1 + \alpha)$.

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P8,Solution,NAC 2025" >}}
    {{< tab >}}
    Consider a hypothetical solar sail that starts its trajectory just outside the surface of the Sun and aims to reach Jupiter’s orbit. This is a square sail with a size length of $l = 50 \, \mathrm{m}$, a mass of $m = 2.0 \, \mathrm{kg}$, and a reflectivity of $\eta = 85\%$. The remaining $15\%$ of the photons are absorbed by the sail. In order to simplify the calculations, only take into account the gravity and radiation pressure from the Sun, and assume that the sail is initially stationary with respect to the Sun. Estimate how long it would take for this sail to reach Jupiter’s orbit. Feel free to make reasonable approximations if needed.
    {{< /tab >}}

    {{< tab >}}
    The radiation flux on the sail when it is at a distance $r$ from the Sun is $\frac{L_\odot}{4 \pi r^2}$. Therefore the radiation force acting on the sail is

    $$ F_\text{rad} = \frac{L_\odot}{4 \pi r^2} \frac{1}{c} A \, (1 + \eta) $$

    where $A = l^2$ is the area of the sail. The gravitational force acting on the sail is

    $$ F_g = \frac{GM_\odot m}{r^2} $$

    The net force acting on the sail is thus

    $$ F = F_\text{rad} - F_g = \frac{L_\odot}{4 \pi r^2} \frac{1}{c} A \, (1 + \eta) - \frac{GM_\odot m}{r^2} $$

    Defining the constant $\alpha$ to be

    $$\alpha = \frac{L_\odot l^2}{4 \pi \, m c} (1 + \eta) - GM_\odot m$$

    The acceleration of the sail is therefore

    $$ a = \frac{F}{m} = \frac{\alpha}{r^2} $$

    Since the acceleration is only in the radial direction, 
    
    $$a = \frac{dv}{dt} = \frac{dv}{dr} \frac{dr}{dt} = v \frac{dv}{dr}$$

    We can write

    $$v \frac{dv}{dr} = \frac{\alpha}{r^2}$$

    Integrating and substituting the limits, we get

    $$\int_0^v v dv = \int_{R_\odot}^r \frac{\alpha}{r^2} dr$$
    $$v^2 = -2\alpha \left( \frac{1}{r} - \frac{1}{R_\odot} \right) $$
    $$v = \frac{dr}{dt} = \sqrt{\frac{2\alpha}{R_\odot} \left( 1-\frac{R_\odot}{r}\right)}$$

    Further integrating a second time and substituting the limits, we get

    $$\int_{R_\odot}^{a_J} dr = \int_0^T \sqrt{\frac{2\alpha}{R_\odot} \left( 1-\frac{R_\odot}{r}\right)} dt$$

    where $a_J$ is the orbital radius of Jupiter. Rearranging and defining $r = (u + 1) R_\odot$ and $a_J = (a + 1) R_\odot$ gives

    $$T = T_0 \int_{0}^{a} \sqrt{1 + \frac{1}{u}} \, du$$

    where $T_0 = \sqrt{\frac{R_\odot^3}{2\alpha}} \approx 21.4 \, \mathrm{min}$ and $a \approx 1117$. This integral cannot be evaluated analytically, and numerical methods need to be used. Thus, we will approximate the integral. Here, we will be working with a very crude approximating.

    Notice that when $u \gg 1$, the integrand is approximately equal to $1$.
    When $u \ll 1$, the integrand is approximately equal to $u^{-1/2}$. Splitting the integral at $u = 1$ and evaluating them separately gives

    $$T \approx T_0 \left( \int_{0}^{1} u^{-1/2} \, du + \int_{1}^{a} 1 \, du \right)$$
    $$= T_0 \left( 2 + a - 1 \right) = T_0 (a + 1)$$

    This gives the time taken to reach Jupiter's orbit as $\boxed{T \approx 16.6 \, \mathrm{days}}$.

    Numerically integrating, the time taken to reach Jupiter's orbit is $T \approx 16.7 \, \mathrm{days}$, very close to our crude approximation.
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P9,Solution" >}}
    {{< tab >}}
    Assuming the human body to be a perfect blackbody, estimate the number of photons emitted in a bandwidth 10% wide around wavelength 550 nm (peak emission wavelength of Sun), by a person in their entire life. Make reasonable assumptions.
    {{< /tab >}}

    {{< tab >}}

    Assuming the human body to be a perfect blackbody, its spectral luminosity will be

    $$L_\lambda = A \pi B_\lambda$$

    where $A \approx 1.7 \, \mathrm{m^2}$ is the surface area of the human body. The temperature of the body is $T \approx 310 \, \mathrm{K}$. The number of photons emitted per unit time per unit wavelength is thus

    $$\frac{\partial^2 N}{\partial t \,\partial \lambda} = \frac{L_\lambda}{h c / \lambda} = \frac{A \pi}{hc} \lambda B_\lambda$$

    Therefore the number of photons emitted by the human body in the given wavelength range in its entire lifetime of $\tau \approx 80 \, \mathrm{yrs}$ is

    $$N = \frac{A \pi \tau}{hc} \int_{\lambda_1}^{\lambda_2} \lambda B_\lambda d\lambda $$

    where $\lambda_1 = \lambda_0 + 0.05 \lambda_0$ and $\lambda_2 = \lambda_0 - 0.05 \lambda_0$ are the limits of the bandwidth ($\lambda_0 = 550 \, \mathrm{nm}$). Using planck's law and definfing $x = \frac{hc}{\lambda kT}$, the integral becomes

    $$N = \frac{2 \pi k^3 T^3 A \tau}{h^3 c^2} \int_{x_2}^{x_1} \frac{x^2 \, dx}{e^x - 1}$$

    where $x_1 = \frac{hc}{\lambda_1 kT} \approx 89$ and $x_2 = \frac{hc}{\lambda_2 kT} \approx 81$. Since $x \gg 1$, we can approximate $e^x - 1 \approx e^x$ and the integral becomes

    $$N = N_0 \int_{x_2}^{x_1} x^2 e^{-x} dx$$

    where $N_0 = \frac{2 \pi k^3 T^3 A \tau}{h^3 c^2} \approx 8 \times 10^{31} \, \mathrm{photons}$. The integral now can be evaluated by parts to give

    $$\int_{x_2}^{x_1} x^2 e^{-x} dx = e^{-x} (x^2 + 2x + 2) \bigg|_{x_2}^{x_1} \approx 4.5 \times 10^{-32}$$

    Therefore the total number of photons emitted by a human body in a $10\%$ bandwidth centered around $550 \, \mathrm{nm}$ in its entire lifetime is

    $$\boxed{N \approx 4 \, \mathrm{photons}}$$
    
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P10,Solution,IOAA 2018" >}}
    {{< tab >}}
    The Five-hundred-meter Aperture Spherical radio Telescope (FAST) is a single-dish radio telescope located  in Guizhou Province, China. The physical diameter of the dish is 500 m, but during observations, the  effective diameter of the collecting area is 300 m. Consider observations of the thermal radio emission from the photosphere of the Sun at 3.0 GHz with this  telescope and a receiver with bandwidth 0.3 GHz.

    a) Calculate the total energy ($E_\odot$) that the receiver will collect during 1 hour of observation.  <br>
    b) Estimate the energy needed to turn over one page of your answer sheet ($E'$). Hint: the typical surface  density of paper is $80 \mathrm{\,g \, m^{-2}}$ <br>
    c) Which one is larger?
    {{< /tab >}}

    {{< tab >}}
    Since we are measuring radio frequencies, we can use the Rayleigh-Jeans approximation

    $$ B_\nu(T) = \frac{2 \nu^2 kT}{c^2} $$

    The spectral luminosity of the Sun is

    $$L_\nu = 4 \pi^2 R_\odot^2 B_\nu(T)$$

    The spectral flux density recieved at Earth is

    $$F_\nu = \frac{L_\nu}{4 \pi D^2}$$

    Hence the total energy collected by FAST in 1 hour is

    $$E_\odot = F_\nu \Delta \nu \cdot A \cdot t = \pi \frac{2 \nu^2 kT}{c^2} \frac{R_\odot^2}{D^2} \Delta \nu \cdot \frac{\pi}{4} d^2 \cdot t$$

    This gives $\boxed{E_\odot \approx 8.5 \times 10^{-5} \mathrm{\,J}}$
    
    The total mass of an A4 paper is

    $$ m = \rho A = 80 \, \mathrm{g \, m^{-2}} \times 297 \, \mathrm{mm} \times 210 \, \mathrm{mm} \approx 5 \, \mathrm{g} $$

    The energy required to turn the paper is the same as the energy required to lift the center of mass of the paper by $h = \frac{210}{2} , \mathrm{mm} = 105 \, \mathrm{mm}$

    $$E' = mgh \approx \boxed{5 \times 10^{-3} \, \mathrm{J}}$$

    Therefore, $\boxed{E' > E_\odot}$
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P11,Solution,IOAA 2019" >}}
    {{< tab >}}
    Since the human body is made mostly of water, it is very efficient at absorbing microwave photons.  Assume that an astronaut’s body is a perfect spherical absorber with mass of $m = 60 \,\mathrm{kg}$, and its  average density and heat capacity are the same as for pure water, i.e. $\rho = 1000 \, \mathrm{kg\,m^{-3}}$ and $C = 4200 \mathrm{\,J\,kg^{-1}\,K^{-1}}$.

    a) What is the approximate rate, in watts, at which an astronaut in intergalactic space would absorb  radiative energy from the Cosmic Microwave Background (CMB)? The spectral energy  distribution of CMB can be approximated by blackbody radiation of temperature $T_\text{CMB} = 2.728 \,\mathrm{K}$. </br>
    b) Approximately how many CMB photons per second would the astronaut absorb? </br>
    c) Ignoring other energy inputs and outputs, how long would it take for the CMB to raise the  astronaut’s temperature by $\Delta T = 1 \, \mathrm{K}$?
    {{< /tab >}}

    {{< tab >}}
    The radius of the spherical astronaut is

    $$\frac{4}{3} \pi r^3 \rho = m \implies r = \left( \frac{3m}{4\pi \rho} \right)^{1/3}$$

    The surface area of the astronaut is

    $$A = 4 \pi r^2 = 4 \pi \left( \frac{3m}{4\pi \rho} \right)^{2/3}$$

    The power thus absorbed by the astronaut is

    $$P = A \sigma T^4 = 4 \pi \left( \frac{3m}{4\pi \rho} \right)^{2/3} \sigma T_\text{CMB}^4 \approx \boxed{2.3 \times 10^{-6} \, \mathrm{W}}$$
    
    The number of photons absorbed per second can be approximated by dividing the total energy absorbed by the mean energy of a CMB photon.The mean energy of a photon is given by

    $$E = 2.70 kT_\text{CMB} \approx 1 \times 10^{-22} \, \mathrm{J}$$

    Thus the number of photons absorbed is

    $$n = \frac{P}{E} \approx \boxed{2.3 \times 10^{16} \, \mathrm{s^{-1}}}$$

    If the time taken to raise the temperature of the astronaut by $\Delta T$ is $t$, then

    $$\Delta Q = m C \Delta T = P t$$

    Rearranging gives

    $$t = \frac{m C \Delta T}{P} \approx \boxed{3430 \, \mathrm{yr}}$$
    {{< /tab >}}
{{< /tabs >}}
