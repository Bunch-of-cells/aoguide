---
title: Stellar Evolution
weight: 4
---

## Stellar Time Scales

### Nuclear Time Scale

The nuclear time scale is the time in which a star radiates away all the energy that can be released by nuclear reactions. Around $10$% of the total Hydrogen present in stars is consumable, and $0.7$% of the rest mass is turned into energy in hydrogen burning. Hence the nuclear time scale is

$$ t_\text{nuc} \backsim 0.1 \cdot 0.007 \cdot \frac{Mc^2}{L} $$

For Sun, $t_\text{nuc} \approx 10^{10}$ years.

### Thermal Time Scale

The thermal time scale is the time in which a star would radiate all its thermal energy if its nuclear energy production were suddenly cutoff. This is also known as the Kelvin-Helmholtz time scale.

$$ t_\text{th} \backsim \frac{GM^2 / 2R}{L} $$

For Sun, $t_\text{th} \approx 2 \times 10^{7}$ years.

### Dynamical Time Scale

The dynamical time scale is the time it would take for a star to collapse if the pressure supporting it against gravity were suddenly removed.

$$ t_\text{dyn} \backsim \sqrt{\frac{R^3}{GM}} $$

For Sun, $t_\text{dyn} \approx 0.5$ hr.

Hence we see that $t_\text{nuc} \gg t_\text{th} \gg t_\text{dyn}$.

## Main Sequence Phase

The main sequence phase is that evolutionary stage in which the energy released by the burning of hydrogen in the core is the only source of stellar energy. During this stage, the star is in stable equilibrium, and its structure changes only because its chemical composition is gradually altered by the nuclear reactions. Thus the evolution takes place on a nuclear time scale, which means that the main sequence phase is the longest part of the life of a star. Main Sequence stars follow a mass-luminosity relationship

$$ L \propto M^{3.8} $$

## Jeans Limit

The Jeans instability describes an instability that leads to the gravitational collapse of a cloud of gas or dust. It causes the collapse of interstellar gas clouds and subsequent star formation. It occurs when the internal gas pressure is not strong enough to prevent the gravitational collapse of a region filled with matter.

Consider a gas cloud of mass $M$, radius $R$, uniform density $\rho$, mean molecular mass $\mu$ and temperature $T$. Jean's length is the critical radius of a gas cloud, below which the cloud will collapse under its own gravity. The gravitational force acting on the cloud is counteracted by the thermal pressure of the gas. The kinetic energy $K$ and potential energy $U$ of the cloud is

$$ K = \frac{3}{2} N k T = 2kT \frac{\pi R^3 \rho}{\mu m_H} $$

$$ U = -\frac{3}{5} \frac{GM^2}{R} = -\frac{16}{15} G \pi^2 R^5 \rho^2 $$

Using virial theorem,

$$\tag{5.4.1} R = \lambda_J = \left( \frac{15}{4 \pi} \frac{k}{Gm_H} \frac{T}{\mu \rho} \right)^{1/2} $$

The critical mass, called Jean's mass is given by

$$\tag{5.4.2} M_J = \frac{4}{3} \pi \lambda_J^3 \rho = \sqrt{ \frac{375}{4 \pi} \left( \frac{k}{Gm_H} \right)^3 \frac{T^3}{\mu^3 \rho} } $$

## Strömgren Sphere

If a hot star is embedded in a region of uniform density gas, then it will be surrounded by a sphere of almost completely ionized hydrogen. At the surface of the sphere (~1 photon mean free path thick), th ionized fraction of hydrogen frops from nearly 1 to nearly 0. Let the rate of ionization be $Q$. This is the rate at which the central stat is producing photons with $h \nu > 13.6 \, \mathrm{eV}$.

$$\tag{5.4.3} Q_* = \int_{\nu_0}^{\infty} \frac{L_\nu}{h \nu}\, d\nu$$

where $L_\nu$ is the spectral luminosity of the star. The mean free path of an electron is

$$\tag{5.4.4} l_\text{rec} = \frac{1}{n_p \sigma_\text{rec}}$$

where $n_p$ is the number density of protons (ionized H) and $\sigma_\text{rec}$ is the cross section for recombination. Let the velocity of electron be $v_e$, then the initial recombinations per unit volume will be

$$\tag{5.4.5} t_\text{rec} = \frac{l_\text{rec}}{v_e} = \frac{1}{n_p \sigma_\text{rec} v_e}$$
$$\tag{5.4.6} N_\text{rec} = \frac{n_e}{t_\text{rec}} = n_e n_p \sigma_\text{rec} v_e$$

where $n_e$ is the number density of electrons. The recombination coefficient is defined as

$$\tag{5.4.7} \alpha(T_e) = \langle \sigma_\text{rec} v_e \rangle \propto T_e^{-1/2}$$

$T_e$ is the temperature of the electrons (may or may not be equal to $T_*$). For overall charge neutrality, $n_e = n_p$.

$$ \therefore N_\text{rec} = n_e^2 \alpha (T_e) $$

For ionization fraction of H to be in equillibrium,

$$\tag{5.4.8} Q_* = N_\text{rec} V$$

where $V = \frac{4}{3} \pi R_S^3$ is the volume of the sphere, and $R_S$ is the radius of the Strömgren sphere, called the Strömgren radius. We can solve for $R_S$ as

$$\tag{5.4.9} R_S = \left( \frac{3}{4 \pi} \frac{Q_*}{n_e^2 \, \alpha (T_e)} \right)^{1/3} \propto T_e^{-1/6}$$
