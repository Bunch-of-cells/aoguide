---
title: Advanced Topics
weight: 6
---

## Radiative Energy Transfer

Understanding how energy moves through space and matter is essential in astrophysics. Radiative transfer describes how light travels through a medium, such as a star's atmosphere or interstellar gas.

Imagine a small cylinder with cross-sectional area $dA$ and length $dr$. Radiation of intensity $I_\nu$ travels perpendicular to the bottom surface into a small solid angle $d\omega$. If the intensity changes by $dI_\nu$, the energy change over a time $dt$ is

$$ dE = dI_\nu \, dA \, d\nu \, d\omega \, dt $$

Some of this energy is absorbed by the medium

$$ dE_\text{abs} = \alpha_\nu I_\nu \, dr \, dA \, d\nu \, d\omega \, dt $$

Here, $\alpha_\nu$ is the opacity (how much the medium absorbs) at frequency $\nu$. The medium can also emit energy, described by the emission coefficient $j_\nu$

$$ dE_\text{em} = j_\nu \, dr \, dA \, d\nu \, d\omega \, dt $$

The total change in energy is the absorbed minus the emitted energy

$$ dE = dE_\text{abs} - dE_\text{em} $$
$$\tag{5.4.1} \implies \frac{1}{\alpha_\nu} \frac{dI_\nu}{dt} = -I_\nu + \frac{j_\nu}{\alpha_\nu} $$

We define the source function, which describes how much energy is emitted compared to how much is absorbed

$$\tag{5.4.2} S_\nu = \frac{j_\nu}{\alpha_\nu} $$

In local thermodynamic equilibrium (LTE), the source function equals the Planck function

$$ S_\nu = B_\nu (T)$$

We also define the optical thickness as $d \tau_\nu = \alpha_\nu \, dr$. It is a measure of how opaque the medium is to radiation at frequency $\nu$.

$$\tag{5.4.3} \therefore \: \boxed{\frac{dI_\nu}{d \tau_\nu} = -I_\nu + S_\nu} $$

This is the fundamental equation of radiative transfer. If $S_\nu > I_\nu$, the intensity increases as radiation travels; if $S_\nu < I_\nu$, it decreases. At equilibrium, absorption equals emission: $dE_\text{abs} = dE_\text{em}$ and $I_\nu = S_\nu = j_\nu / \alpha_\nu$.

A general solution to this equation is

$$\tag{5.4.4} I_\nu (\tau_\nu) = I_\nu (0) \, e^{-\tau_\nu} + \int_0^{\tau_\nu} S_\nu (t) \, e^{-(\tau_\nu - t)} \, dt$$

where $I_\nu (0)$ is the background intensity. This equation is widely used to model the atmospheres of stars and planets, as well as the interstellar medium.

## Albedo

Albedo measures how well a surface reflects light. Suppose a planet of radius $R$ is at a distance $r$ from the Sun. The total energy flux hitting the planet is

$$ L_\text{in} = \pi R^2 \frac{L_\odot}{4 \pi r^2} $$

The Bond albedo $A$ is the fraction of incoming energy that is reflected.

$$ L_\text{out} = A L_\text{in} $$

The reflected light is not always spread evenly in all directions; it depends on the phase angle $\alpha$ (the angle between the Sun, planet, and observer). The observed flux at Earth is

$$ F = C \, \Phi (\alpha) \, \frac{L_\text{out}}{4\pi d^2} = \frac{CA}{4\pi} \, \Phi(\alpha) \, \frac{1}{d^2} \,L_\text{in} $$

Here, $d$ is the distance from the planet to Earth, $C$ is a constant, and $\Phi(\alpha)$ is the phase function (how brightness changes with phase angle). When $\alpha = 0^\circ$, $\Phi(0) = 1$. The total reflected flux is $L_\text{out}$, so

$$ \frac{C}{4 \pi d^2} \int_S \Phi(\alpha) \, dS = 1 $$
$$ \implies C = \frac{4 \pi d^2}{\int_S \Phi(\alpha) \, dS} = \frac{2}{\int_0^\pi \Phi(\alpha) \sin \alpha \, d\alpha} = \frac{4}{q} $$

The phase integral is defined as $q = 2 \int_0^\pi \Phi(\alpha) \sin \alpha \, d \alpha$. We define $\Gamma = \frac{CA}{4\pi}$. The geometric albedo of the planet is

$$ p = \pi \Gamma $$

Bond albedo and geometric albedo are related by $A = pq$.

{{< callout type="remark" >}}
A Lambertian surface is a perfect diffuser that reflects all incoming light equally in all directions, so $A = 1$ and

$$ \Phi(\alpha) = \begin{cases} \cos \alpha \qquad &0^\circ \le \alpha \le 90^\circ \\ 0 \qquad &\text{otherwise} \end{cases} $$

For a Lambertian surface, $p = q = 1$ and $C = 4$. The flux density at $\alpha = 0^\circ$ is

$$ F_L = \frac{1}{\pi} \, \frac{1}{d^2} \, L_\text{in} $$

For a non-Lambertian surface, the flux density at $\alpha = 0^\circ$ is

$$ F = \frac{CA}{4\pi} \, \frac{1}{d^2} \, L_\text{in} $$

So,

$$ \frac{F}{F_L} = \frac{CA}{4} = p $$

Thus, geometric albedo $p$ is the ratio of the flux at $\alpha = 0^\circ$ reflected by the planet to that reflected by a Lambertian disk of the same size.

Some surfaces can have $p > 1$ (for example, a mirror, where $p$ is infinite).
{{< /callout >}}

The flux density of reflected light is

$$ F = \frac{p}{\pi} \, \Phi(\alpha) \, \frac{1}{d^2} \, \frac{L_\odot R^2}{4 r^2} $$

The solar flux at Earth is $F_\odot = L_\odot / 4\pi a^2$. Therefore,

$$ m - m_\odot = -2.5 \log \frac{pR^2}{a^2} + 5 \log \frac{dr}{a^2} - 2.5 \log \Phi(\alpha) $$

The absolute magnitude $V(1, 0)$ of a planet is the magnitude it would have if it were 1 AU from both the Earth and Sun, at phase angle $\alpha = 0^\circ$

$$ V(1, 0) = m_\odot - 2.5 \log \frac{pR^2}{a^2} $$

Although this situation is not physically possible, it is a useful reference for comparing relative brightness of planets.

$$\therefore m = V(1, 0) + 5 \log \frac{dr}{a^2} - 2.5 \log \Phi(\alpha) $$

The absolute magnitude at phase angle $\alpha$ is:

$$ V(1, \alpha) = V(1, 0) - 2.5 \log \Phi(\alpha) $$
$$ \implies m = V(1, \alpha) + 5 \log \frac{dr}{a^2} $$

At $\alpha = 0^\circ$, $p = \left( \frac{dr}{aR} \right)^2 10^{-0.4 (m - m_0)}$ where $m_0 = m(\alpha = 0^\circ)$ is the apparent magnitude.

## Cyclotron and Synchrotron Radiation

When charged particles like electrons move through a magnetic field, they experience a force that causes them to spiral. This motion causes them to emit radiation, which is important in many astrophysical environments.

An electron in a magnetic field $\mathbf{B}$ feels a Lorentz force:

$$ \mathbf{F} = e \left( \mathbf{v} \times \mathbf{B} \right) $$

where $e$ is the electron charge. For a non-relativistic electron, the acceleration is:

$$ \mathbf{a} = \frac{\mathbf{F}}{m} = \frac{e}{m} \left( \mathbf{v} \times \mathbf{B} \right) $$

where $m$ is the electron mass. The electron moves in a helical path with radius:

$$ r_c = \frac{mv_\perp}{eB} $$

The pitch angle is $\tan \alpha_c = v_\perp / v_\parallel$, where $v_\perp$ is the velocity perpendicular to the field and $v_\parallel$ is parallel to the field.

The angular frequency of this motion (cyclotron frequency) is:

$$ \omega = \frac{v_\perp}{r_c} = \frac{eB}{m} $$

The electron emits energy (cyclotron radiation) according to the Larmor formula:

$$ P = \frac{2}{3} \frac{e^2}{4\pi \varepsilon_0 c^3} a^2 $$

The spectrum is narrow and peaks at:

$$ \nu_\text{max} \approx \frac{\omega_c}{2 \pi} \approx 280 \, \mathrm{GHz} \, \left( \frac{B}{1 \, \mathrm{T}} \right) $$

{{< callout type="remark" >}}
If the electron is moving close to the speed of light (relativistic), it spirals at the electron gyrofrequency:

$$ \omega_s = \frac{eB}{\gamma m} = \frac{\omega_c}{\gamma} < \omega_c $$

Here, $\gamma$ is the Lorentz factor. The radiation emitted is called synchrotron radiation. The maximum frequency is:

$$ \nu_\text{max} \approx 12 \, \mathrm{GHz} \, \gamma^2 \left( \frac{B}{1 \, \mathrm{T}} \right) \sin \alpha_c $$
{{< /callout >}}

For reference, the magnetic field at Earth's surface is $B_\oplus \approx 3.1 \times 10^{-5} \, \mathrm{T}$ and at Jupiter's surface is $B_J \approx 5 \times 10^{-4} \, \mathrm{T}$.
