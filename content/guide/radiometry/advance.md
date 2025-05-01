---
title: Advanced Topics
weight: 4
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
