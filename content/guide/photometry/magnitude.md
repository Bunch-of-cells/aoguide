---
title: Magnitude Systems
weight: 2
---

Magnitude is a measure of the brightness of a star, astronomical object or other celestial objects like artificial satellites. We would like to be able to communicate and express how bright an object. For this one could use the luminosity of the object, or the flux recieved by that object. However, these numbers can get very large or very small. As a result, a magnitude scale is used.

Magnitudes are denoted by the unit 'mag', or with a superscript $^m$, although they have no dimensions. The scale is reverse logarithmic: the brighter an object is, the lower its magnitude number. A difference of 1.0 mag in magnitude corresponds to the brightness ratio of $\sqrt[5]{100}$, or about 2.512. For example, a magnitude 2.0 star is 2.512 times brighter than a magnitude 3.0 star, 6.31 times brighter than a magnitude 4.0, and 100 times brighter than a magnitude 7.0 star.

Apparent magnitude is a measure of the brightness of an object as seen from Earth. It is related to how much flux is recieved from that object to the observer. It is usually denoted by $m$.

Absolute magnitude on the other hand is a measure of the intrinsic brightness of an object, defined as the apparent magnitude it would have if it were located at a distance of 10 parsecs from the observer, without any extinction. The absolute magnitude of a star is directly related to its luminosity. It is usually denoted by $M$.

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

{{< callout type="remark" >}}
The difference in absolute magnitudes of two objects gives the ratio of their luminosities. If $M_1$ and $M_2$ are the absolute magnitudes of two objects, then

$$M_1 - M_2 = -2.5 \log \frac{L_1}{L_2} $$

where $L_1$ and $L_2$ are the luminosities of the two objects.

If the two objects have radii $R_1$ and $R_2$, and temperatures $T_1$ and $T_2$, then we can find luminosity using the Stefan-Boltzmann law

$$L = 4 \pi R^2 \sigma T^4$$

From this we get

$$M_1 - M_2 = -5 \log \frac{R_1}{R_2} - 10 \log \frac{T_1}{T_2}$$
{{< /callout >}}

{{< tabs items="P1,Solution" >}}
    {{< tab >}}
    What is the absolute magnitude of the Sun? Apparent magnitude of the sun as seen from Earth is $m_\odot = -26.8^m$.
    {{< /tab >}}

    {{< tab >}}
    Using Pogson's equation,

    $$M_\odot = m_\odot + 5 \log \frac{1 \, \mathrm{AU}}{10 \, \mathrm{pc}} = \boxed{4.8^m}$$
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P2,Solution" >}}
    {{< tab >}}
    Albireo is a star in the constellation of Cygnus. It is a double and the system has a total magnitude of $3.0^m$. The fainter companion (Albireo B) has a magnitude of $5.1^m$. Find out the apparent magnitude of the brighter component of the double, Albireo A.
    {{< /tab >}}

    {{< tab >}}
    The light which we see coming from a double is the sum of the light from both components. Let $F_0$ be the flux which corresponds to a magnitude of 0. Let $L_A$ and $L_B$ be the luminosities of Albireo A and B, respectively. The total luminosity of the system is thus $L_A + L_B$.

    The luminosity of Albireo B can be found using

    $$m_B = -2.5 \log \frac{L_B}{F_0} \implies L_B = F_0 \cdot 10^{-0.4 m_B}$$

    The total luminosity of the system can be found using

    $$m_\text{tot} = -2.5 \log \frac{L_A + L_B}{F_0} \implies L_A + L_B = F_0 \cdot 10^{-0.4 m_\text{tot}}$$

    Hence the luminosity of Albireo A is

    $$L_A = F_0 \cdot 10^{-0.4 m_\text{tot}} - F_0 \cdot 10^{-0.4 m_B}$$

    The apparent magnitude of Albireo A is given by Pogson's equation as

    $$m_A = -2.5 \log \frac{L_A}{F_0} = -2.5 \log \left(10^{-0.4 m_\text{tot}} - 10^{-0.4 m_B} \right)$$

    Therefore we get that $\boxed{m_A = 3.2^m}$
    {{< /tab >}}
{{< /tabs >}}

## Color Indices

Usually, filters are used to allow only certain wavelengths to enter the detector. This gives more information about the object than measuring the flux through all wavelengths at once. One such system of filters used commonly is the UBV system. It consists of three filters:

- The ultraviolet filter (U) is centered at 365 nm with an effective bandwidth of 66 nm
- The blue filter (B) is centered at 445 nm with an effective bandwidth of 94 nm
- The visual filter (V) is centered at 551 nm with an effective bandwidth of 88 nm

The apparent magnitudes measured through these filters are denoted by $U$, $B$ and $V$, or by $m_U$, $m_B$, and $m_V$. The absolute magnitudes are denoted by $M_U$, $M_B$, and $M_V$.

{{< callout type="remark" >}}
Aside from the UBV system, there are other systems of filters used in astronomy, such as the Johnson-Cousins system, which includes additional filters like R (red), I (infrared) and J, H, K, L and M bands (which also lie in the infrared), and the SDSS system, which includes filters u, g, r, i, and z.
{{< /callout >}}

The color index is defined as the difference between the magnitudes measured through two different filters. For example, the $U-V$ color index is the difference between its $U$ and $V$ magnitudes

$$(U-V) = m_U - m_V = M_U - M_V = U - V$$

This gives the color of the star, which can be used to determine its temperature. The smaller the $B-V$ index, the bluer the star is, hence the hotter it is. Color indices of a star are independent of its distance.

The sensitivity function $S(\lambda)$ is defined as the fraction of a star's flux detected by a filter at a given wavelength. It depends on the optics of the system, filter bandwidth and response of the photometer. For example, the apparent $U$ magnitude is given by

$$ U = -2.5 \log \int_0^\infty F_\lambda S_U(\lambda)\, d\lambda + C_U $$

where $C_U$ is a constant. The apparent $B$ and $V$ magnitudes are defined similarly.

The $U-B$ color index is thus

$$ (U-B) = -2.5 \log \frac{\int_0^\infty F_\lambda S_U(\lambda)\, d\lambda}{\int_0^\infty F_\lambda S_B(\lambda)\, d\lambda} + C_{U-B} $$

where $C_{U-B} = C_U - C_B$.

## Bolometric Magnitude

Apparent magnitude is defined in a specific bandpass, such as the visual band, and depends on the sensitivity of the detectors used. The apparent magnitude of an object in the visual band or 'V' band is called the apparent visual magnitude $m_V$ of the object. The apparent bolometric magnitude $m_\text{bol}$ is defined as the apparent magnitude of an object if all its radiation were collected and measured over all wavelengths. This would correspond to an ideal detector which is able to measure at all wavelengths with complete efficiency.

The absolute bolometric magnitude $M_\text{bol}$ is defined as the absolute magnitude of an object if all its radiation were collected and measured over all wavelengths.

The bolometric correction $BC$ is defined as the difference between the bolometric magnitude and the visual magnitude, given by

$$\tag{2.2.3} \boxed{BC = m_\text{bol} - m_V}$$

We also have that $BC = M_\text{bol} - M_V$ where $M_\text{bol}$ and $M_V$ are the absolute bolometric and absolute visual magnitudes, respectively.

For the bolometric magnitude, the sensitivity function is unity everywhere: $S_\text{bol} (\lambda) = 1$.

$$\therefore m_\text{bol} = -2.5 \log \int_0^\infty F_\lambda\, d\lambda + C_\text{bol} $$

where $C_\text{bol}$ is a constant.

By definition, bolometric correction is zero for F5 spectral type stars.

{{< tabs items="P3,Solution" >}}
    {{< tab >}}
    Find an expression for the bolometric correction, assuming the visual sensitivity function is given by

    $$S_V(\lambda) = \begin{cases} 1 & \text{if } \lambda_1 < \lambda < \lambda_2 \\ 0 & \text{otherwise} \end{cases}$$

    Where $\lambda_1 = 551 - 44$ nm and $\lambda_2 = 551 + 44$ nm.

    Consider the zero point of both the visual and bolometric magnitudes to be the same, i.e. $C_V = C_\text{bol}$. Assume the emitting body emits like a perfect blackbody of temperature $5800 \, \mathrm{K}$.
    {{< /tab >}}

    {{< tab >}}
    The visual magnitude is given by

    $$ m_V = -2.5 \log \int_0^\infty F_\lambda S_V(\lambda)\, d\lambda + C_V $$

    The bolometric magnitude is given by

    $$ m_\text{bol} = -2.5 \log \int_0^\infty F_\lambda\, d\lambda + C_\text{bol} $$

    Thus the bolometric correction is given by

    $$ BC = m_\text{bol} - m_V = -2.5 \log \left( \frac{\int_0^\infty F_\lambda\, d\lambda}{\int_0^\infty F_\lambda S_V(\lambda)\, d\lambda} \right) $$

    Since $F_\lambda$ follows a blackbody spectrum, we can write

    $$ F_\lambda = \pi \frac{R^2}{D^2} \cdot \frac{2 \pi h c^2}{\lambda^5} \frac{1}{e^{\frac{hc}{\lambda k T}} - 1} $$

    Where $T$ is the temperature of the object, $R$ is the radius of the object and $D$ is the distance to the object. Defining $x = \frac{hc}{\lambda kT}$, and doing some algebra, we get that the expression for the bolometric correction simplifies to

    $$ BC = 2.5 \log \left( \frac{15}{\pi^4} \int_{x_2}^{x_1} \frac{x^3}{e^x - 1} \,dx \right) $$

    where $x_1 = \frac{hc}{\lambda_1 k T} \approx 4.901$ and $x_2 = \frac{hc}{\lambda_2 k T} \approx 4.176$. Numerical integration gives

    $$ \boxed{BC \approx -2.37^m} $$

    The bolometric correction of the sun, which too has a temperature of about $5800 \, \mathrm{K}$, is about $-0.7^m$. This large difference is due to the assumptions we made: Sun does not emit like a perfect blackbody, the zero points of the visual and bolometric magnitudes are not the same, and the sensitivity function is not a perfect rectangle, but rather shaped like a bell curve.
    {{< /tab >}}
{{< /tabs >}}

## Extended Objects

For extended objects (which are not point-like), the total magnitude can be obtained by summing up the luminosity over the area of the object. The apparent magnitude of an extended object is defined as the magnitude of a point source that would produce the same total flux as the extended object.

Thus the total amount of light from a galaxy of $12^m$ would be the same as that from a star of $12^m$. However, since the light from the galaxy is spread over a larger area, it will appear dimmer than the star.

For a comet, the total magnitude is the combined magnitude of the coma and the nucleus.

The surface brightness $S$ quantifies the apparent brightness of flux density per unit angular area of the spatially extended obejct. For an object with total magnitude $m$ extended over a visual area $A \mathrm{\: arcsec^2}$, its surface brightness is defined as

$$\tag{2.2.4} \boxed{S = m + 2.5 \log A} $$

Surface brightness is measured in units of $\mathrm{mag \,/\, arcsec^{2}}$. This is a much more useful quantity when comparing brightness of extended objects.

## Extinction

### ISM

If the space between the observer and the radiating source is not empty and is filled with interstellar medium (ISM), which consists of gas and dust. As light passes through the ISM, some of the it will be absorbed or scattered. This reduction of intensity of light in the direction of propagation is called extinction.

Suppose a star is radiating a flux $L_0$ into a solid angle $\omega$. The flux will decrease with distance because of extinction

$$\tag{2.2.5} dL = - \alpha L \, dr $$

The opacity $\alpha$ quantifies how effectively the medium can obsecure radiation. For vacuum, $\alpha = 0$. The dimensionless quanitity $\tau$, called the optical thickness or optical depth, is defined as

$$\tag{2.2.6} d\tau = \alpha \, {dr} $$

$$\tag{2.2.7} \therefore dL = -L \, d\tau \implies \boxed{L = L_0 e^{-\tau}} $$

Here $\tau = \int_0^r \alpha \, dr = \langle \alpha \rangle r$ is the optical thickness between the source and the observer. This exponential decay is known as the Beer-Lambert law.

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

where $A = ar \ge 0$ is the extinction in magnitudes due to the interstellar medium, as light goes from the star to the observer. $a = 2.5 \langle \alpha \rangle \log e \approx 1.1 \langle \alpha \rangle$ gives the extinction in magnitudes per unit distance.

Extinction also causes reddening of light; blue light is scattered and absorbed more than red light, hence the color index $B-V$ increases.

$$
\begin{aligned}
V &= M_V + 5 \log \frac{r}{10 \mathrm{\, pc}} + A_V \\
B &= M_B + 5 \log \frac{r}{10 \mathrm{\, pc}} + A_B \\
\end{aligned}
$$

$$\tag{2.2.9} \therefore \boxed{(B-V) = (B-V)_0 + E_{B-V}} $$

where $(B-V)_0 = M_B - M_V$ is the intrinsic color index of the star and the color excess is defined as $E_{B-V} = A_B - A_V$.

Studies show that the ratio of the visual extinction $A_V$ to the $(B-V)$ color excess $E_{B-V}$ is almost constant for all stars

$$\tag{2.2.10} R = \frac{A_V}{E_{B-V}} \approx 3.1 $$

{{< tabs items="P4,Solution" >}}
    {{< tab >}}
    A star's apparent magnitude in the V band is $15.1^m$ and absolute magnitude is equal to $1.3^m$. Extinction of the interstellar medium per kpc is $1^m$.

    a) Find the distance to the star. <br>
    b) If the star's observed color index is $(B-V) = 1.6^m$, find its intrinsic color. <br>
    c) If $BC = -0.6^m$ for the star, find its luminosity.
    {{< /tab >}}

    {{< tab >}}
    **a)** The distance modulus is given by

    $$m - M = 5 \log \frac{r}{10 \times 10^{-3}} + ar$$

    Where $r$ is measured in kpc, and $a = 1^m \, \mathrm{kpc^{-1}}$. Substituting the values, we get

    $$3.8 = \log r + r$$

    Solving it numerically, we get $\boxed{r \approx 3.28 \, \mathrm{kpc}}$.

    **b)** The intrinsic color index is given by

    $$(B-V)_0 = (B-V) - E_{B-V}$$

    We can use the relation between $A_V$ and $E_{B-V}$ to find the color excess. The extinction in visual band is

    $$A_V = ar = 3.28^m$$

    Hence the color excess is

    $$E_{B-V} = \frac{A_V}{R} \approx 1.06^m$$

    Thus the intrinsic color index of the star is

    $$\boxed{(B-V)_0 = 1.6^m - 1.06^m = 0.54^m}$$

    **c)** The bolometric magnitude of the star is

    $$M_\text{bol} = M_V + BC = 1.3^m - 0.6^m = 0.7^m$$

    Comparing with the bolometric magnitude of the sun gives the luminosity of the star

    $$M_\text{bol} - M_{\odot, \text{bol}} = -2.5 \log \frac{L}{L_\odot}$$
    $$\implies L = L_\odot \cdot 10^{-0.4(M_\text{bol} - M_{\odot, \text{bol}})}$$

    The absolute bolometric magnitude of the Sun is $4.75^m$. Thus we get that the luminosity of the star is

    $$\boxed{L \approx 41.7 L_\odot}$$

    {{< /tab >}}
{{< /tabs >}}

### Atmospheric Extinction

Earth's atmosphere also causes extinction. The observed magnitude $m$ depends on the location of the observer and the zenith distance of the object. If the zenith distance $z$ is not too large, the atmosphere can be modelled by a plane layer of constant thickness. The airmass is defined as

$$\tag{2.2.11} \boxed{X = \sec z} $$

This approximation holds good for $z \lesssim 70^\circ$.

The increase in magnitude is

$$\tag{2.2.12} m = m_0 + kX $$

where $k$ is the extinction coefficient, which depends on the wavelength of light and the atmospheric conditions. The extinction coefficient is defined as the increase in magnitude per unit airmass. $m_0$ is the true apparent magnitude, devoid of extinction effects.

Atmospheric extinction is usually negligible for objects at zenith, but can be significant for objects near the horizon.

Since $k$ depends on the wavelength, the color index is also affected by atmospheric extinction.

## Problems

{{< tabs items="P5,Solution" >}}
    {{< tab >}}
    Vega is known to have an apparent magnitude of about $0$ (in reality it is about $0.03$ and fluctuates). Given that it has an absolute magnitude of about $0.58$, find its distance.
    {{< /tab >}}

    {{< tab >}}
    Using Pogson's equation, we have

    $$m - M = 5 \log \frac{r}{10 \, \mathrm{pc}}$$

    Substituting the values, we get

    $$0 - 0.58 = 5 \log \frac{r}{10}$$
    $$\implies r = 10 \cdot 10^{-0.116} \approx 7.7 \, \mathrm{pc}$$

    Hence the distance to Vega is approximately $\boxed{7.7 \, \mathrm{pc}}$.

    Note that since Vega is so close to us, the extinction effects are negligible, and we can ignore them in this case.
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P6,Solution" >}}
    {{< tab >}}
    What is the optical thickness of a layer of fog, if the Sun seen through the fog seems as bright as a full moon in a cloudless sky?
    {{< /tab >}}

    {{< tab >}}
    The apparent magnitudes of the Sun and the Moon are $−26.8$ and $−12.5$, respectively. Thus the total extinction in the cloud must be $A = 14.3$. Since

    $$ A = (2.5 \log e) \tau $$

    where $\tau$ is the optical thickness of the fog, we can rearrange to get

    $$ \tau = \frac{A}{2.5 \log e} = \frac{14.3}{1.086} \approx \boxed{13.2}$$
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P7,Solution" >}}
    {{< tab >}}
    Assume that all stars have the same absolute magnitude and stars are evenly distributed in space. Let $N(m)$ be the number of stars brighter than m magnitudes. Find the ratio $N(m + 1)/N(m)$.
    {{< /tab >}}

    {{< tab >}}
    Let the number density of stars be $n$, and their absolute magnitude be $M$. Let the apparent magnitude of the star at a distance $r$ pc from the observer be $m$. $m$ and $r$ are related by the equation

    $$ m - M = 5 \log r - 5 $$

    Rearranging gives

    $$ r = 10^{0.2(m - M) + 1} $$

    All the stars brighter than magnitude $m$ will lies within $r$ pc distance to the observer. Thus the volume of the sphere upto radius $r$ is

    $$ V = \frac{4}{3} \pi r^3 = \frac{4}{3} \pi \left( 10^{0.2(m - M) + 1} \right)^3 $$

    The number of stars brighter than magnitude $m$ is given by

    $$ N(m) = n V = n \frac{4}{3} \pi \left( 10^{0.2(m - M) + 1} \right)^3 $$

    The number of stars brighter than magnitude $m + 1$ is given by

    $$ N(m + 1) = n \frac{4}{3} \pi \left( 10^{0.2(m + 1 - M) + 1} \right)^3 $$

    The ratio of the two is given by

    $$ \frac{N(m + 1)}{N(m)} = \left( \frac{10^{0.2(m + 1 - M) + 1}}{10^{0.2(m - M) + 1}} \right)^3 = 10^{0.6} \approx \boxed{3.98}$$
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P8,Solution,IOAA 2012" >}}
    {{< tab >}}
    An old planetary nebula, with a white dwarf (WD) in its center, is located 50 pc away from Earth. Exactly in the same direction, but behind the nebula, lies another WD, identical to the frist, but located at 150 pc from the Earth. Consider that the two WDs have absolute bolometric magnitude +14.2 and intrinsic color indexes $B - V = 0.300$ and $U - V = 0.330$. Extinction occurs in the interstellar medium and in the planetary nebula.

    When we measure the color indices for the closer WD (the one who lies at the center of the nebula), we find the values $B - V = 0.327$ and $U - B = 0.038$. In this part of the Galaxy, the interstellar extinction rates are 1.50, 1.23 and 1.00 magnitudes per kiloparsec for the filters U, B and V, respectively. Calculate the color indices as they would be measured for the second star.
    {{< /tab >}}

    {{< tab >}}
    Let $B_0$, $V_0$, $U_0$ be the intrinsic absolute magnitudes of the white dwarf. Let $a_B$, $a_V$, $a_U$ be the interstellar extinction coefficients per kpc. Let $A_{neb,B}$, $A_{neb,V}$, $A_{neb,U}$ be the total extinction for the planetary nebula around the first WD, for light travelling from the centre of the nebula to the edge.

    $$(U-B)_0 = (U-V)_0 - (B-V)_0 = 0.330 - 0.300 = 0.030$$

    For the closer WD,

    $$(U-V)_1 = (U-B)_1 + (B_V)_1 = 0.038 + 0.327 = 0.365$$
    $$(B-V)_1 = (B-V)_0 + (a_B - a_V) r + (A_{neb,B} - A_{neb,V})$$
    $$\begin{align*}
    \therefore (A_{neb,B} - A_{neb,V}) &= (B-V)_1 - (B-V)_0 - (a_B - a_V) r \\ &= 0.0155
    \end{align*}$$

    Similarily,

    $$\begin{align*}
    (A_{neb,U} - A_{neb,V}) &= (U-V)_1 - (U-V)_0 - (a_U - a_V) r \\ &= 0.0100
    \end{align*}$$
    $$\begin{align*}
    (A_{neb,U} - A_{neb,B}) &= (U-B)_1 - (U-B)_0 - (a_U - a_B) r \\ &= -0.0055
    \end{align*}$$

    For second white dwarf, the extinction in planetary nebula will be doubled as extinction the light from this pulsar has to cross the entire diameter of the nebula. Overall distance of this pulsar is 3 times larger.

    $$(B-V)_2 = (B-V)_0 + 3(a_B-a_V)r + 2(A_{neb,B} - A_{neb,V})$$
    $$\implies \boxed{(B-V)_2 \approx 0.366}$$
    $$(U-V)_2 = (U-V)_0 + 3(a_U-a_V)r + 2(A_{neb,U} - A_{neb,V})$$
    $$\implies \boxed{(U-V)_2 \approx 0.425}$$
    $$(U-B)_2 = (U-B)_0 + 3(a_U-a_B)r + 2(A_{neb,U} - A_{neb,B})$$
    $$\implies \boxed{(U-B)_2 \approx 0.060}$$

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P9,Solution,IOAA 2008" >}}
    {{< tab >}}
    A UBV photometric observation of a star gives $U = 8.15$, $B = 8.50$, and $V = 8.14$. Based on the spectral class, one gets the intrinsic colour $(U − B)_0 = −0.45$. If the star is known to have radius of $2.3R_\odot$, absolute bolometric magnitude of $−0.25$, and bolometric correction (BC) of $−0.15$, determine:

    a) the intrinsic magnitudes U, B, and V of the star <br>
    b) the effective temperature of the star <br>
    c) the distance to the star

    Note: Take, for the typical interstellar matters, the ratio of total to selective extinction $R_V = 3.2$ and the colour excess in $(B − V)$ to be about 72% of the colour excess in $(U − B)$. 
    {{< /tab >}}

    {{< tab >}}
    **a)** Let intrinsic magnitudes of the star be $U_0$, $B_0$, and $V_0$ respectively.

    $$E_{U-B} = (U-B) - (U - B)_0 = (3.15 - 8.50) - (-0.45) = 0.1$$

    Since $E_{U-B} = 0.72 \, E_{B-V}$, $E_{B-V} = \frac{0.1}{0.72} = 0.14$.

    Using the relation $A_V = R_V \, E_{B-V}$, we get

    $$A_V = 3.2 \cdot 0.14 = 0.45$$
    $$\therefore \boxed{V_0 = V + A_V = 7.69}$$

    The intrinsic $B_0$ and $U_0$ color can be found using

    $$(B-V)_0 = (B-V) - E_{B-V} = (8.50 - 8.14) - 0.14 = 0.22$$
    $$\begin{align*}
    \implies &\boxed{B_0 = V_0 + (B-V)_0 = 7.91}
    \\ &\boxed{U_0 = B_0 + (U-B)_0 = 7.46}
    \end{align*}$$

    **b)** Comparing the star's bolometric magnitude to that of the Sun,

    $$\begin{align*}
    &M_\text{bol} - M_{\odot, \text{bol}} = -2.5 \log \frac{L}{L_\odot}
    \\ \implies &M_{\odot, \text{bol}} - M_\text{bol} = 5 \log \frac{R}{R_\odot} + 10 \log \frac{T}{T_\odot}
    \end{align*}$$

    Substituting the values, we get

    $$\boxed{T = 2.07 T_\odot = 12000 \, \mathrm{K}}$$

    **c)** The absolute visual magnitude can be found using the bolometric correction

    $$M_V = M_\text{bol} + BC = -0.25 + (-0.15) = -0.40$$

    Hence the distance can be found

    $$m_V - M_V = 5 \log \frac{r}{10 \, \mathrm{pc}}$$
    $$\implies 7.69 - (-0.40) = 5 \log \frac{r}{10}$$
    $$\implies \boxed{r \approx 415 \, \mathrm{pc}}$$

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P10,Solution,IOAA 2012" >}}
    {{< tab >}}
    A pulsar, located 1000 pc far from Earth and 10,000 times more luminous than our Sun, emits radiation only from its two opposite poles, creating a homogeneous emission beam shaped as double cone with opening angle $\alpha = 4^\circ$. Assuming the angle between the rotation axis and the emission axis is $\theta = 30^\circ$, and assuming a random orientation of the pulsar beams in relation to an observer on Earth, what is the probability of detecting the pulses? In case we can see it, what is the apparent bolometric magnitude of the pulsar?
    {{< /tab >}}

    {{< tab >}}
    As the pulsar rotates, its beam sweeps out a conical surface. The solid angle into which radiation is emitted (by both poles) in one rotation is

    $$\begin{align*}
    \Omega &= 2 \cdot \left[ 2 \pi (1 - \cos (\theta + \frac{\alpha}{2})) - 2 \pi (1 - \cos (\theta - \frac{\alpha}{2})) \right]
    \\ &= 8 \pi \sin \theta \sin \frac{\alpha}{2}
    \end{align*}$$

    To detect the pulsar, Earth must lie inside this solid angle. Hence the probability is

    $$p = \frac{\Omega}{4 \pi} = 2 \sin \theta \sin \frac{\alpha}{4} \approx \boxed{0.035}$$

    The pulsar emits radiation into a cone having solid angle

    $$\Omega = 2 \cdot 4 \pi \sin^2 \frac{\alpha}{4}$$

    Thus the flux recieved on Earth is

    $$F = \frac{L}{A} = \frac{L}{\omega r^2} = \frac{L}{8 \pi r^2} \frac{1}{\sin^2 \frac{\alpha}{4}}$$

    Comparing the flux with the solar flux gives the apparent magnitude of the pulsar

    $$\begin{align*}
    m &= M_\odot - 2.5 \log \frac{F}{F_\odot}
    \\ &= M_\odot - 2.5 \log \frac{L}{8 \pi r^2 \sin^2 \frac{\alpha}{4}} \frac{4 \pi r_0^2}{L_\odot}
    \\ &= M_\odot -2.5 \log \frac{L}{L_\odot} + 5 \log \frac{r}{10 \, \mathrm{pc}} + 5 \log (\sqrt{2} \sin \frac{\alpha}{4})
    \\ &= 4.72 - 8.04 = \boxed{-3.32}
    \end{align*}$$
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P11,Solution,IOAA 2018" >}}
    {{< tab >}}
    A star has an apparent magnitude $m_U = 15.0$ in the U-band. The U-band filter is ideal, i.e., it has perfect (100%) transmission within the band and is completely opaque (0% transmission) outside the band. The  filter is centered at 360 nm, and has a width of 80 nm. It is assumed that the star also has a flat energy spectrum with respect to frequency. The conversion between magnitude, $m$, in any band and flux density, $f$, of a star in Jansky is given by

    $$f = 3631 \times 10^{-0.4m} \, \mathrm{Jy}$$

    a) Approximately how many U-band photons, $N_0$, from this star will be incident normally on a  $1 \, \mathrm{m^2}$  area at the top of the Earth's atmosphere every second?

    This star is being observed in the U-band using a ground based telescope, whose primary mirror has a  diameter of $2.0 \, \mathrm{m}$. Atmospheric extinction in U-band during the observation is 50%. You may assume that the seeing is diffraction limited. Average surface brightness of night sky in U-band was measured to be $22.0 \, \mathrm{mag/arcsec^2}$.

    b) What is the ratio, $R$, of number of photons received per second from the star to that received from the sky, when measured over a circular aperture of diameter $2''$? <br>
    c) In practice, only 20% of U-band photons falling on the primary mirror are detected. How many photons, $N_t$, from the star are detected per second?
    {{< /tab >}}

    {{< tab >}}
    ****a)**** The U-band is defined as ($360 \pm 40$) nm. Thus, the minimum, maximum and average frequencies of the band are

    $$\begin{align*}
    \nu_\text{min} &= \frac{c}{\lambda_\text{max}} = 7.495 \times 10^{14} \, \mathrm{Hz} \\
    \nu_\text{max} &= \frac{c}{\lambda_\text{min}} = 9.369 \times 10^{14} \, \mathrm{Hz} \\
    \nu_\text{avg} &= \frac{\nu_\text{min} + \nu_\text{max}}{2} = 8.432 \times 10^{14} \, \mathrm{Hz} \\
    \Delta \nu &= \nu_\text{max} - \nu_\text{min} = 1.874 \times 10^{14} \, \mathrm{Hz}
    \end{align*}$$

    $$\therefore f = 3631 \times 10^{-0.4 \cdot 15.0} \, \mathrm{Jy} = 3.631 \times 10^{-29} \, \mathrm{W \, Hz^{-1} \, m^{-2}}$$

    Now, $N_0 \times h \nu_\text{avg} = \Delta \nu \cdot f \cdot A \cdot \Delta t$, where $A = 1 \, \mathrm{m^2}$ and $\Delta t = 1 \, \mathrm{s}$.

    $$ \therefore N_0 = \frac{f A \Delta \nu \Delta t}{h \nu_\text{avg}} \approx \boxed{12180}$$

    **b)** Let us call sky flux per square arcsec as $\Phi$ and total sky flux for the given aperture as $\phi_\text{sky}$. Let total star flux be $\phi_\text{st}$.

    $$\phi_\text{sky} = \Phi A = \pi (1'')^2 \Phi$$

    Using the formula for surface brightness, we get that the magnitude corresponding to this flux is

    $$m_{sky} = 22.0 + 2.5 \log \frac{\Phi}{\phi_\text{sky}} = 20.76^m$$

    As extinction is 50%,

    $$R = \frac{0.5 \phi_\text{st}}{\phi_\text{sky}} = 0.5 \times 10^{-0.4(15 - 20.76)} \approx \boxed{100}$$

    **c)** Equating the number of photons,
    
    $$N_T \times 1 \, \mathrm{m} = N_0 \times 0.5 \times 0.2 \times A_t$$
    $$\implies N_T = 12180 \times 0.5 \times 0.2 \times \left( \frac{2.0}{2} \right)^2 \approx \boxed{3813}$$

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P12,Solution,IOAA 2018" >}}
    {{< tab >}}
    The star $\beta$-Doradus is a Cepheid variable star with a pulsation period of 9.84 days. We make a simplifying assumption that the star is brightest when it is most contracted (radius being $R_1$) and it is faintest when it is most expanded (radius being $R_2$). For simplicity, assume that the star maintains its spherical shape and behaves as a perfect black body at every instant during the entire cycle. The bolometric magnitude of the star varies from $3.46$ to $4.08$. From Doppler measurements, we know that during pulsation the stellar surface expands or contracts at an average radial speed of $12.8 \, \mathrm{km \, s^{-1}}$. Over the period of pulsation, the peak of thermal radiation (intrinsic) of the star varies from 531.0 nm to 649.1 nm.

    a) Find the ratio of radii of the star in its most contracted and most expanded states ($R_1/R_2$). <br>
    b) Find the radii of the star (in metres) in its most contracted and most expanded states ($R_1$ and $R_2$). <br>
    c) Calculate the flux of the star, $F_2$, when it is in its most expanded state. <br>
    d) Find the distance to the star, $D_\text{star}$, in parsecs.
    {{< /tab >}}

    {{< tab >}}
    **a)** The ratio of the fluxes is

    $$m_1 - m_2 = -2.5 \log \frac{F_1}{F_2} \implies \frac{F_1}{F_2} = 10^{-0.4(m_1 - m_2)} = 1.77$$

    The flux is given by $F = \frac{4 \pi R^2 \sigma T^4}{4 \pi D^2}$, if the star is at a distance $D$ from the observer.
    
    Hence we get that

    $$\frac{F_1}{F_2} = \frac{R_1^2 T_1^4}{R_2^2 T_2^4} = 1.77$$

    Using Wien's displacement law, $\frac{T_1}{T_2} = \frac{\lambda_2}{\lambda_1}$.

    $$\implies \frac{R_1}{R_2} = \sqrt{\frac{F_1}{F_2}} \left( \frac{\lambda_1}{\lambda_2} \right)^2 = \boxed{0.890}$$

    **b)** The radial velocity causes the change in radius of the star

    $$R_2 - R_1 = v \cdot \frac{P}{2} = 5.441 \times 10^9 \, \mathrm{m}$$
    $$(1-0.890)R_2 = 5.441 \times 10^9 \, \mathrm{m}$$
    $$\begin{align*}
    \therefore \: &\boxed{R_2 = 4.95 \times 10^10 \, \mathrm{m}} \\
    &\boxed{R_1 = 4.40 \times 10^{10} \, \mathrm{m}}
    \end{align*}$$

    **c)** To get the absolute value of flux ($F_2$) we must compare it with observed flux of the Sun.

    $$m_2 - m_\odot = -2.5 \log \frac{F_2}{F_\odot}$$
    $$\implies F_2 = F_\odot \cdot 10^{-0.4(m_2 - m_\odot)}$$

    $$F_2 = 1361 \, \mathrm{W \, m^{-2}} \cdot 10^{-0.4(4.08 + 26.72)} = \boxed{6.51 \times 10^{-10} \, \mathrm{W \, m^{-2}}}$$

    **d)** The temperature of the star when it is fully expanded is

    $$T_2 = \frac{b}{\lambda_2} = 4465 \, \mathrm{K}$$

    The distance can be found using the observed flux

    $$F_2 = \frac{4 \pi R_2^2 \sigma T_2^4}{4 \pi D_\text{star}^2}$$
    $$\implies D_\text{star} = R_2 T_2^2 \sqrt{\frac{\sigma}{F_2}} = \boxed{298 \, \mathrm{pc}}$$

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P13,Solution" >}}
    {{< tab >}}
    Given the intrinsic $(B-V)$ color index of a star, find its color temperature $T_c$.
    {{< /tab >}}

    {{< tab >}}
    Assuming the star to be a blackbody, the spectral flux density in the Wien approximation of the star is propotional to

    $$ F_\lambda \propto \lambda^{-5} e^{-hc/\lambda kT_c} $$

    The color index is defined as

    $$ (B-V) = -2.5 \log \left( \frac{F_B}{F_V} \right) $$
    $$\implies (B-V) = -2.5 \log \left( \frac{\lambda_B^{-5} e^{-hc/\lambda_B kT_c}}{\lambda_V^{-5} e^{-hc/\lambda_V kT_c}} \right) $$
    $$\implies (B-V) = 12.5 \log \left( \frac{\lambda_B^5}{\lambda_V^5} \right) + 2.5 \frac{hc}{kT_c} \left( \frac{1}{\lambda_B} - \frac{1}{\lambda_V} \right) $$
    $$\implies T_c = \frac{hc}{k} \cdot \frac{2.5 \left( \frac{1}{\lambda_B} - \frac{1}{\lambda_V} \right)}{(B-V) + 2.5 \log \left( \frac{\lambda_B^5}{\lambda_V^5} \right)}$$

    Substituting the values $\lambda_B = 440 \, \mathrm{nm}$ and $\lambda_V = 550 \, \mathrm{nm}$, we get

    $$\boxed{T_c \approx \frac{7000 \mathrm{K}}{(B-V) + 0.47}}$$
    {{< /tab >}}
{{< /tabs >}}
