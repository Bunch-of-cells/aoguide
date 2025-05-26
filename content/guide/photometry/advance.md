---
title: Advanced Topics
weight: 6
---

## Synchrotron Radiation

An electron moving in a magnetic field $\mathbf{B}$ experiences a Lorentz force

$$ \mathbf{F} = e \left( \mathbf{v} \times \mathbf{B} \right) $$

where $q$ is the charge of the electron. If the electron is non-relativistic, its acceleration is

$$ \mathbf{a} = \frac{\mathbf{F}}{m} = \frac{e}{m} \left( \mathbf{v} \times \mathbf{B} \right) $$

where $m$ is the mass of the electron. The electron moves in a helical path having radius $r$ given by

$$ r_c = \frac{mv_\perp}{eB} $$

The pitch angle is given by $\tan \alpha_c = v_\perp / v_\parallel$, where $v_\perp$ is the velocity perpendicular to the magnetic field and $v_\parallel$ is the velocity parallel to the magnetic field.

The angular frequency of the motion, called the cyclotron frequency, is

$$ \omega = \frac{v_\perp}{r_c} = \frac{eB}{m} $$

The electron radiates energy, called cyclotron radiation, according to the Larmor formula

$$ P = \frac{2}{3} \frac{e^2}{4\pi \varepsilon_0 c^3} a^2 $$

It's spectrum is narrow in frequency and peaks at

$$ \nu_\text{max} \approx \frac{\omega_c}{2 \pi} \approx 280 \, \mathrm{GHz} \, \left( \frac{B}{1 \, \mathrm{T}} \right) $$

A relativistic electron will spiral around the magnetic field lines at the electron gyrofrequency

$$ \omega_s = \frac{eB}{\gamma m} = \frac{\omega_c}{\gamma} < \omega_c $$

Here $\gamma$ is the Lorentz factor. The radiation is called synchrotron radiation. The maximum frequency of the radiation is given by

$$ \nu_\text{max} \approx 12 \, \mathrm{GHz} \, \gamma^2 \left( \frac{B}{1 \, \mathrm{T}} \right) \sin \alpha_c $$

The magnetic field on the surface of Earth is $B_\oplus \approx 3.1 \times 10^{-5} \, \mathrm{T}$ and on the surface of Jupiter is $B_J \approx 5 \times 10^{-4} \, \mathrm{T}$.

## Radiative Energy Transfer

Consider a small cylinder of dimensions $dA \times dr$, with radiation of intensity $I_\nu$ propagating perpendiculat to the bottom surface into a solid angle $d\omega$. If the intensity changes by $d I_\nu$, the energy changes by

$$ dE = dI_\nu \, dA \, d\nu \, d\omega \, dt $$

in time $dt$. The absorbed energy is

$$ dE_\text{abs} = \alpha_\nu I_\nu \, dr \, dA \, d\nu \, d\omega \, dt $$

where $\alpha_\nu$ is the opacity of the medium at frequency $\nu$. Let the energy emittied into unit solid angle from unit volume per unit time in frequency interval $[\nu, \nu + d\nu]$ be $j_\nu$, called the emission coefficient of the medium.

$$ dE_\text{em} = j_\nu \, dr \, dA \, d\nu \, d\omega \, dt $$

The total change in energy is given by

$$ dE = dE_\text{abs} - dE_\text{em} $$
$$\tag{5.4.1} \implies \frac{1}{\alpha_\nu} \frac{dI_\nu}{dt} = -I_\nu + \frac{j_\nu}{\alpha_\nu} $$

We define the source function as

$$\tag{5.4.2} S_\nu = \frac{j_\nu}{\alpha_\nu} $$

In local thermodynamic equilibrium (LTE), the source function is given by the Planck function

$$ S_\nu = B_\nu (T)$$

and the optical thickness at frequency $\nu$ as $d \tau_\nu = \alpha_\nu \, dr$.

$$\tag{5.4.3} \therefore \boxed{\frac{dI_\nu}{d \tau_\nu} = -I_\nu + S_\nu} $$

This is the basic equation of radiative transfer. If $S_\nu > I_\nu$, the intensity increases in the direction of propagation, and if $S_\nu < I_\nu$, the intensity decreases in the direction of propagation. At equillibrium, $dE_\text{abs} = dE_\text{em}$ and $I_\nu = S_\nu = j_\nu / \alpha_\nu$.

A formal solution to the equation is

$$\tag{5.4.4} I_\nu (\tau_\nu) = I_\nu (0) \, e^{-\tau_\nu} + \int_0^{\tau_\nu} S_\nu (t) \, e^{-(\tau_\nu - t)} \, dt$$

where $I_\nu (0)$ is the intensity of the background radiation.

This equation can be used to model stellar and planetary atmospheres, and the radiation field in the interstellar medium.

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
