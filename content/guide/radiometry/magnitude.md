---
title: Magnitude
weight: 2
---

Magnitude is a measure of the brightness of a star, astronomical object or other celestial objects like artificial satellites. These are denoted by the unit 'mag', or with a superscript $^m$, although it has no dimensions. The scale is reverse logarithmic: the brighter an object is, the lower its magnitude number. A difference of 1.0 mag in magnitude corresponds to the brightness ratio of $\sqrt[5]{100}$, or about 2.512. For example, a magnitude 2.0 star is 2.512 times as bright as a magnitude 3.0 star, 6.31 times as magnitude 4.0, and 100 times magnitude 7.0.

Apparent magnitude is a measure of the brightness of an object as seen from Earth. Its value depends on its intrinsic luminosity, its distance, and any extinction of the object's light caused by interstellar dust along the line of sight to the observer.

Absolute magnitude is a measure of the intrinsic brightness of an object, defined as the apparent magnitude it would have if it were located at a distance of 10 parsecs from the observer. The absolute magnitude of a star is directly related to its luminosity.

## Pogson's Equation

The dimmer an object appears, the higher the numerical value given to its magnitude, with a difference of 5 magnitudes corresponding to a brightness factor of exactly 100. Let a flux value of $F_0$ correspond to a magnitude of $m_0$. Then, the magnitude $m$ corresponding to an object having a flux of $F$ is given by Pogson's equation, which reads

$$m - m_0 = -5 \log_{100} \left( \frac{F}{F_0} \right) $$

or equivalently,

$$\tag{2.2.1} \boxed{m - m_0 = -2.5 \log \frac{F}{F_0}} $$

where the base of the logarithm is 10.

Consider an object with luminosity $L$, distance $r$, apparent magnitude $m$, and absolute magnitude $M$. The flux $F$ received from the object at Earth is $F = L/4\pi r^2$. The flux $F_0$ at $10 \mathrm{pc}$ from the object is $F_0 = L/4\pi (10 \mathrm{pc})^2$. Ignoring extinction, we get

$$
\begin{aligned}
    m - M &= -2.5 \log \left( \frac{F}{F_0} \right) \\
    &= -2.5 \log \left( \frac{L/4\pi r^2}{L/4\pi (10 \, \mathrm{pc})^2} \right) \\
    &= -2.5 \log \left( \frac{(10 \, \mathrm{pc})^2}{r^2} \right) \\
    &= 5 \log \frac{r}{10 \, \mathrm{pc}} \\
\end{aligned}
$$

Hence we get that

$$\tag{2.2.2} \boxed{m - M = 5 \log \frac{r}{10 \, \mathrm{pc}}} $$

If $r$ is measured in parsecs,

$$m - M = 5 \log r - 5 $$

The distance modulus is defined as $\mu = m - M$.

The difference in absolute magnitudes of two objects gives the ratio of their luminosities. If $M_1$ and $M_2$ are the absolute magnitudes of two objects, then

$$M_1 - M_2 = -2.5 \log \frac{L_1}{L_2} $$

where $L_1$ and $L_2$ are the luminosities of the two objects.

## Bolometric Magnitude

Apparent magnitude is defined in a specific bandpass, such as the visual band, and depends on the sensitivity of the detectors used. The apparent magnitude of an object in the visual band or 'V' band is called the apparent visual magnitude $m_V$ of the object. The apparent bolometric magnitude $m_\text{bol}$ is defined as the apparent magnitude of an object if all its radiation were collected and measured over all wavelengths. This would correspond to an ideal detector which is able to measure at all wavelengths with complete efficiency.

The absolute bolometric magnitude $M_\text{bol}$ is defined as the absolute magnitude of an object if all its radiation were collected and measured over all wavelengths.

The bolometric correction $BC$ is defined as the difference between the bolometric magnitude and the visual magnitude, given by

$$\tag{2.2.3} \boxed{BC = m_\text{bol} - m_V}$$

We also have that $BC = M_\text{bol} - M_V$ where $M_\text{bol}$ and $M_V$ are the absolute bolometric and absolute visual magnitudes, respectively.

The zero absolute bolometric magnitude $M_\text{bol} = 0$ corresponds to a luminosity of approximately $3.0128 \times 10^{28} \, \mathrm{W}$.

## Limiting Magnitude

For starlight, the limit of unaided eye detection is set at about $6^m$. This limit however can be increased by using a detector with a larger aperture size, such as a telescope. Consider a telescope with an aperture diameter D. Since the flux recieved is directly propotional to the recieving area,

$$ \frac{F_t}{F_e} = \frac{D^2}{d^2} $$

where $d$ is the size of the eye pupil, approximately $8 \, \mathrm{mm}$. The limiting magnitude of the telescope is defined as the magnitude of the faintest object that can be detected by the telescope. The limiting magnitude $m_t$ of a telescope with an aperture diameter D is given by

$$\tag{2.2.4} m_t - m_e = -2.5 \log \left( \frac{F_t}{F_e} \right) = -5 \log \frac{D}{d} $$

where $m_e = 6^m$ is the limiting magnitude of the eye.

100% of the light hitting the aperture is not collected by the telescope. The light is scattered, absorbed, and reflected by the telescope optics. The fraction of light that is actually collected is called the transmission efficiency $\eta$. The limiting magnitude of a telescope with an aperture diameter D and trasmission efficiency $\eta$ is given by

$$ m_t = m_e -2.5 \log \left( \eta \frac{D^2}{d^2} \right)$$

## Color Indices

Usually, filters are used to allow only certain wavelengths to enter the detector. One such is the UBV system.

- The ultraviolet filter (U) is centered at 365 nm with an effective bandwidth of 68 nm
- The blue filter (B) is centered at 440 nm with an effective bandwidth of 98 nm
- The visual filter (V) is centered at 550 nm with an effective bandwidth of 89 nm

The apparent magnitudes measured through these filters are denoted by $U$, $B$ and $V$, or by $m_U$, $m_B$, and $m_V$. The absolute magnitudes are denoted by $M_U$, $M_B$, and $M_V$. The color index is defined as the difference between the magnitudes measured through two different filters. For example, the $U-V$ color index is the difference between its $U$ and $V$ magnitudes

$$(U-V) = m_U - m_V = M_U - M_V = U - V$$

The smaller the $B-V$ index, the bluer the star is, hence the hotter it is. Color indices of a star are independent of its distance.

The sensitivity function $S(\lambda)$ is defined as the fraction of a star's flux detected by a filter at a given wavelength. It depends on the reflectivity of the mirrors, filter bandwidth and response of the photometer. For example, the apparent $U$ magnitude is given by

$$ U = -2.5 \log \int_0^\infty F_\lambda S_U(\lambda)\, d\lambda + C_U $$

where $C_U$ is a constant. The apparent $B$ and $V$ magnitudes are defined similarly.
For the bolometric magnitude, $S_\text{bol} (\lambda) = 1$.

$$ m_\text{bol} = -2.5 \log \int_0^\infty F_\lambda\, d\lambda + C_\text{bol} $$

where $C_\text{bol}$ is a constant. The $U-B$ color index is

$$ (U-B) = -2.5 \log \frac{\int_0^\infty F_\lambda S_U(\lambda)\, d\lambda}{\int_0^\infty F_\lambda S_B(\lambda)\, d\lambda} + C_{U-B} $$

where $C_{U-B} = C_U - C_B$.

## Extinction

If the space between the observer and the radiating source is not empty and is filled with some ISM (interstellar medium), some of the radiation will be absorbed or scattered. This is called extinction.

Suppose a star is radiating a flux $L_0$ into a solid angle $\omega$. The flux will decrease with distance because of extinction

$$\tag{2.2.5} dL = - \alpha L \, dr $$

The opacity $\alpha$ quantifies how effectively the medium can obsecure radiation. For vacuum, $\alpha = 0$. The dimensionless quanitity $\tau$, called the optical thickness or optical depth, is defined as

$$\tag{2.2.6} d\tau = \alpha \, {dr} $$

$$\tag{2.2.7} \therefore dL = -L \, d\tau \implies \boxed{L = L_0 e^{-\tau}} $$

Here $\tau = \int_0^r \alpha \, dr = \langle \alpha \rangle r$ is the optical thickness between the source and the observer.

If $F_0$ is the flux density at the star's surface and $F(r)$ is the flux density at a distance $r$,

$$ F(r) = F_0 \left( \frac{R}{r} \right)^2 e^{-\tau} $$

From this we get

$$
\tag{2.2.8} \begin{aligned}
    m - M &= -2.5 \log \left( \frac{F(r)}{F(10\,\mathrm{pc})} \right) \\
    &= 5 \log \frac{r}{10 \, \mathrm{pc}} + A \\
    &= 5 \log \frac{r}{10 \, \mathrm{pc}} + ar \\
\end{aligned}
$$

where $A = ar \ge 0$ is the extinction in magnitudes due to the medium, from $10 \mathrm{\,pc}$ from the star to the observer. Usually the star is far enough away so that $10 \mathrm{\, pc}$ can be ignored, and the extinction is due to the whole medium between the star and the observer. $a = 2.5 \langle \alpha \rangle \log e$ gives the extinction in magnitudes per unit distance.

Extinction also causes reddening of light; blue light is scattered and absorbed more than red light, hence the color index $B-V$ increases.

$$
\begin{aligned}
V &= M_V + 5 \log \frac{r}{10 \mathrm{\, pc}} + A_V \\
B &= M_B + 5 \log \frac{r}{10 \mathrm{\, pc}} + A_B \\
\end{aligned}
$$

$$\tag{2.2.9} \therefore \boxed{(B-V) = (B-V)_0 + E_{B-V}} $$

where $(B-V)_0 - M_B - M_V$ is the intrinsic color index of the star and the color excess is defined as $E_{B-V} = A_B - A_V$.

The ratio of the visual extinction $A_V$ to the $(B-V)$ color excess $E_{B-V}$ is almost constant for all stars

$$\tag{2.2.10} R = \frac{A_V}{E_{B-V}} \approx 3.1 $$

### Atmospheric Extinction

Earth's atmosphere also causes extinction. The observed magnitude $m$ depends on the location of the observer and the zenith distance of the object. If the zenith distance $z$ is not too large, the atmosphere can be modelled by a plane layer of constant thickness. The airmass is defined as

$$\tag{2.2.11} \boxed{X = \sec z} $$

The increase in magnitude is

$$\tag{2.2.12} m = m_0 + kX $$

where $k$ is the extinction coefficient, which depends on the wavelength of light and the atmospheric conditions. The extinction coefficient is defined as the increase in magnitude per unit airmass. $m_0$ is the true apparent magnitude, devoid of extinction effects.

## Extended Objects

The total magnitude of an extended object can be obtained by summing up the luminosity over the area of the object. The apparent magnitude is generally the integrated value. The total amount of light from a galaxy of $12^m$ would be the same as that from a star of $12^m$.

The total magnitude of a comet is the combined magnitude of the coma and the nucleus.

The surface brightness $S$ quantifies the apparent brightness of flux density per unit angular area of the spatially extended obejct. For an object with total magnitude $m$ extended over a visual area $A \mathrm{\: arcsec^2}$, its surface brightness is defined as

$$\tag{2.2.13} \boxed{S = m + 2.5 \log A} $$

Surface brightness is measured in units of $\mathrm{mag \,/\, arcsec^{2}}$.

## Albedo

The term albedo defines the ability of a body to reflect light.

Consider a planet or radius $R$ at a distance $r$ from the Sun. The total flux incident on the surface of the planet is

$$ L_\text{in} = \pi R^2 \frac{L_\odot}{4 \pi r^2} $$

The bond albedo $A$ is defined as the ratio of the emergent flux to the incident flux

$$ L_\text{out} = A L_\text{in} $$

The radiation is radiated anisotropically and depends on the phase angle $\alpha$. The flux density observed at Earth will be

$$ F = C \, \Phi (\alpha) \, \frac{L_\text{out}}{4\pi d^2} = \frac{CA}{4\pi} \, \Phi(\alpha) \, \frac{1}{d^2} \,L_\text{in} $$

where $d$ is the distance of the planet from Earth, $C$ is a constant and $\Phi(\alpha)$ is called the phase function. It is one when the phase angle is zero, $\Phi(\alpha = 0^\circ) = 1$. The total flux emittied is $L_\text{out}$, therefore

$$ \frac{C}{4 \pi d^2} \int_S \Phi(\alpha) \, dS = 1 $$
$$ \implies C = \frac{4 \pi d^2}{\int_S \Phi(\alpha) \, dS} = \frac{2}{\int_0^\pi \Phi(\alpha) \sin \alpha \, d\alpha} = \frac{4}{q} $$

The quantity $q = 2 \int_0^\pi \Phi(\alpha) \sin \alpha \, d \alpha$ is the phase integral. We define $\Gamma = \frac{CA}{4\pi}$. The geometric albedo is defined as

$$ p = \pi \Gamma $$

The bond albedo and geometric albedo are related by $A = pq$.

A Lambertian surface is an absolutely white diffuse surface which reflects all radiation. Hence $A = 1$ and

$$ \Phi(\alpha) = \begin{cases} \cos \alpha \qquad &0^\circ \le \alpha \le 90^\circ \\ 0 \qquad &\text{otherwise} \end{cases} $$

From this we get that for a lambertian surface, $p = q = 1$ and $C = 4$. The flux density radiated when $\alpha = 0^\circ$ is

$$ F_L = \frac{1}{\pi} \, \frac{1}{d^2} \, L_\text{in} $$

The flux density when $\alpha = 0^\circ$ for a non-lambertian surface is

$$ F = \frac{CA}{4\pi} \, \frac{1}{d^2} \, L_\text{in} $$

Hence we get that

$$ \frac{F}{F_L} = \frac{CA}{4} = p $$

We can therefore interpret the geometric albedo as the ratio of the flux densities at $\alpha = 0^\circ$ reflected by the planet and a lambertian surface of the same cross-section.

For some surfaces, $p > 1$. For a mirror $p$ is infinite.

The flux density of the reflected light is

$$ F = \frac{p}{\pi} \, \Phi(\alpha) \, \frac{1}{d^2} \, \frac{L_\odot R^2}{4 r^2} $$

The solar flux at Earth is $F_\odot = L_\odot / 4\pi a^2$. Therefore,

$$ m - m_\odot = -2.5 \log \frac{pR^2}{a^2} + 5 \log \frac{dr}{a^2} - 2.5 \log \Phi(\alpha) $$

The absolute magnitude $V(1, 0)$ of a planet is defined as the magnitude of the body if it is at a distance of $1 \, \mathrm{AU}$ from the Earth and Sun at a phase angle of $\alpha = 0^\circ$.

$$ V(1, 0) = m_\odot - 2.5 \log \frac{pR^2}{a^2} $$

Even though this situation is unphysical, it serves as a useful quanitity for computing the apparent magnitudes of planets. The absolute magnitude of a planet can never be observed, and is a property intrinsic to the planet.

$$ m = V(1, 0) + 5 \log \frac{dr}{a^2} - 2.5 \log \Phi(\alpha) $$

The absolute magnitude at a phase angle $\alpha$ is defined as

$$ V(1, \alpha) = V(1, 0) - 2.5 \log \Phi(\alpha) $$
$$ \implies m = V(1, \alpha) + 5 \log \frac{dr}{a^2} $$

At $\alpha = 0^\circ$, $p = \left( \frac{dr}{aR} \right)^2 10^{-0.4 (m - m_0)}$ where $m_0 = m(\alpha = 0^\circ)$ is the apparent magnitude.
