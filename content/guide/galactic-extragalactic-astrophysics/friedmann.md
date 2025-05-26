---
title: The Friedmann Equations
weight: 4
---

## The Friedmann Equation

The equation which links together the scale factor $a(t)$, the curvature $\kappa$, the current radius of curvature $R_0$, and the energy density $\varepsilon(t)$ is the Friedmann equation:

$$\tag{7.3.1} \boxed{\left( \frac{\dot{a}}{a} \right)^2 = \frac{8\pi G}{3 c^2} \varepsilon (t) - \frac{\kappa c^2}{R_0^2} \frac{1}{a(t)^2}}$$

The Friedmann equation is derived from the Einstein field equations of general relativity, which describe how matter and energy in the universe influence its geometry. However, it can be approximately derived from Newtonian physics by considering a homogeneous and isotropic universe.

The Hubble parameter $H(t)$ is defined as

$$\tag{7.3.2} H(t) = \frac{\dot{a}}{a}$$

The present value of the Hubble parameter (at $t = t_0$) is called the Hubble constant $H_0$, and is approximately equal to $70 \, \text{km/s/Mpc}$.

We define the critical energy density $\varepsilon_\text{c}$ as the energy density of a flat universe, which is given by

$$\tag{7.3.3} \varepsilon_\text{c}(t) = \frac{3 H(t)^2}{8 \pi G}$$

The current value of the critical energy density is $\varepsilon_{\text{c},0} \approx 5.2 \mathrm{\,GeV\,m^{-3}}$. At any time, if $\kappa = +1$, $\varepsilon(t) > \varepsilon_\text{c}(t)$; if $\kappa = 0$, $\varepsilon(t) = \varepsilon_\text{c}(t)$; and if $\kappa = -1$, $\varepsilon(t) < \varepsilon_\text{c}(t)$.

The density parameter $\Omega(t)$ is defined as

$$\tag{7.3.4} \Omega(t) = \frac{\varepsilon(t)}{\varepsilon_\text{c}(t)}$$

$$ \therefore 1 - \Omega(t) = -\frac{\kappa c^2}{R_0^2 a(t)^2 H(t)^2} $$

The RHS can't change its sign, hence if $\omega$ was less than 1 at some time, it will always be less than 1. From this relation we also get that by measuring $H_0$ and $\Omega_0$, we can find $\kappa$ and $R \: (= a(t)\, R_0)$.

Define the density parameter related to the curvature $\Omega_\kappa(t)$ as

$$\tag{7.3.2} \Omega_\kappa(t) = -\frac{\kappa c^2}{R_0^2 \, a(t)^2 \, H(t)^2}$$

Then we can rewrite the Friedmann equation as

$$\tag{7.3.1} \Omega(t) + \Omega_\kappa(t) = 1$$

The sum of all the density parameters in the universe is equal to 1, at all times.

## Fluid and Acceleration Equation

The universe can be modelled as a perfect fluid, one which is incompressible and has no viscosity. The fluid equation is

$$\tag{7.3.5} \boxed{\dot{\varepsilon} + 3 \frac{\dot{a}}{a} (\varepsilon + P) = 0}$$

where $P$ is the pressure of the fluid, associated with the material filling the universe. This can be derived from thermodynamics, and is a consequence of the conservation of energy and momentum in a homogeneous and isotropic universe.

The acceleration equation is

$$\tag{7.3.6} \boxed{\frac{\ddot{a}}{a} = -\frac{4 \pi G}{3c^2} (\varepsilon + 3P)}$$

All matter has positive pressure and hence causes the rate of expansion to slow down. However, if the pressure is negative, it can cause the expansion to accelerate. This is the case for dark energy, which has a negative pressure and is responsible for the observed acceleration of the universe's expansion. One of the models of dark energy is the cosmological constant $\Lambda$, which is a constant energy density filling space homogeneously.

## Equation of State

An equation of state is a mathematical relation between the pressure and the energy density of the 'stuff' that fills up the universe. It can be expressed in a simple linear form as

$$\tag{7.3.7} \boxed{P = w \varepsilon}$$

where $w$ is a dimensionless number.

- For non-relativistic matter, $w = 0$.
- For radiation and relativistic matter, $w = \frac{1}{3}$.
- $w < -\frac{1}{3}$ will provide a positive acceleration to the universe ($\ddot{a} > 0$). Such a component is called 'dark energy'.
- The cosmological constant $\Lambda$ is a special case of dark energy, where $w = -1$.

For adiabatic perturbations in a gas with pressure $P$ and energy density $\varepsilon$, the speed of sound $c_s$ is

$$\tag{7.3.8} c_s^2 = c^2 \, \frac{\partial P}{\partial \varepsilon} = w c^2$$

Since the speed of sound is always less than the speed of light, for all components of the universe we have $w < 1$.

## Cosmological Constant

Adding $\Lambda$ into our equations gives

$$\tag{7.3.9} \boxed{ \left( \frac{\dot{a}}{a} \right)^2 = \frac{8\pi G}{3 c^2} \varepsilon (t) - \frac{\kappa c^2}{R_0^2 \, a(t)^2} + \frac{\Lambda}{3}}$$
$$\tag{7.3.10} \boxed{\dot{\varepsilon} + 3 \frac{\dot{a}}{a} (\varepsilon + P) = 0}$$
$$\tag{7.3.11} \boxed{\frac{\ddot{a}}{a} = -\frac{4 \pi G}{3c^2} (\varepsilon + 3P) + \frac{\Lambda}{3}}$$

We see that the cosmological constant acts like a fluid with $w = -1$, and has its own associated energy density and pressure, both of which are constant over space and time.

$$\tag{7.3.12} \varepsilon_\Lambda = \frac{\Lambda c^2}{8 \pi G}$$
$$\tag{7.3.13} P_\Lambda = -\varepsilon_\Lambda = -\frac{\Lambda c^2}{8 \pi G}$$

The total pressure and energy density of the universe can be expressed as

$$\tag{7.3.14} \varepsilon = \sum_w \varepsilon_w$$
$$\tag{7.3.15} P = \sum_w P_w = \sum_w w \varepsilon_w$$

From the fluid equation, we get

$$\tag{7.3.16} \varepsilon_w (t) = \varepsilon_{w,0} \, a(t)^{-3(1+w)}$$

where $\varepsilon_{w,0}$ is the energy density of the component at the present time.

- For matter ($w = 0$), $\varepsilon_\text{m} \propto a^{-3}$.
- For radiation ($w = \frac{1}{3}$), $\varepsilon_\text{r} \propto a^{-4}$.
- For cosmological constant $\Lambda$ ($w = -1$), $\varepsilon_\Lambda \propto a^0$.

Since the energy density of radiation is propotional to $T^4$, and also depends on the scale factor as $a^{-4}$, we can relate the temperature of the universe to the scale factor as

$$\tag{7.3.17}  T(t) \propto \frac{1}{a(t)} \implies T(t) = T_0 \, a(t)^{-1}$$

where $T_0$ is the present temperature of the universe.

Let $\Omega_\text{m}$, $\Omega_\text{r}$ and $\Omega_\Lambda$ be the density parameters for matter, radiation and dark energy respectively. Then the Friedmann equation can be rewritten as

$$\tag{7.3.18} \boxed{\Omega_\text{m} + \Omega_\text{r} + \Omega_\Lambda + \Omega_\kappa = 1}$$

The present time values of the density parameters are

Component | $\bold{\Omega_0}$ |
--- | --- |
Matter | $\Omega_{\text{m}, 0} \approx 0.3$|
Radiation | $\Omega_{\text{r}, 0} \approx 8.4 \times 10^{-5}$|
Dark Energy | $\Omega_{\Lambda, 0} \approx 0.7$|
Curvature | $\Omega_{\kappa, 0} \approx 0$ |

## Single Component Universes

### Empty Curved Universe

For an empty curved universe, the Friedmann equation becomes

$$\tag{7.3.18} \dot{a}^2 = -\frac{\kappa c^2}{R_0^2}$$

The solutions to this equation are $\dot{a} = 0$ and $\kappa = 0$, corresponding to a static, empty and spatially flat universe, and $\kappa = -1$ and $\dot{a} = \pm \frac{c}{R_0}$.

For an expanding universe,

- $a(t) = \frac{t}{t_0} = H_0 t$, where $t_0$ is the age of the universe.
- The Hubble parameter is $H(t) = t^{-1}$, and the Hubble constant is $H_0 = t_0^{-1}$.
- The age of the universe is $t_0 = H_0^{-1} = \frac{R_0}{c}$.
- $1 + z = \frac{1}{a(t_e)} = (H_0 t_e)^{-1} \implies t_e = \frac{1}{H_0 (1+z)}$.
- $d_p (t_0) = c \int_{t_e}^{t_0} \frac{dt}{a(t)} = \frac{c}{H_0} \ln (1+z) $
- $d_p (t_e) = \frac{c}{H_0} \frac{\ln (1+z)}{1+z}$ was the proper distance at the time of emission (maximum for $z \approx 1.7$).

### Flat Universe

For a flat universe ($\kappa = 0$) containing only a single component with equation of state coefficient of $w$, the Friedmann equation becomes

$$\tag{7.3.19} \dot{a}^2 = \frac{8 \pi G \varepsilon_0}{3 c^2} a^{-(1+3w)}$$

This gives the scale factor as

$$\tag{7.3.20} \boxed{a(t) = \left( \frac{t}{t_0} \right)^{\frac{2}{3(1+w)}}}$$

where $t_0 = \frac{1}{1+w} \left( \frac{c^2}{6 \pi G \varepsilon_0} \right)^{\frac{1}{2}}$ is the age of the universe. The Hubble parameter is given by

$$\tag{7.3.21} H(t) = \frac{2}{3(1+w)} \frac{1}{t}$$

Hence $t_0 = \frac{2}{3(1+w)} H_0^{-1}$. The energy density is given by

$$\tag{7.3.22} \varepsilon(t) = \varepsilon_0 \, a(t)^{-3(1+w)} = \varepsilon_0 \, \left( \frac{t}{t_0} \right)^{-2}$$

Moreover since the universe is flat, $\varepsilon(t) = \varepsilon_\text{c}(t) = \frac{3c^2}{8 \pi G} H(t)^2$. From this we get

$$\tag{7.3.23} \varepsilon(t) = \frac{1}{6\pi (1+w)^2} \frac{c^2}{G} \frac{1}{t^2} = \frac{1}{6\pi (1+w)^2} \frac{E_\text{p}}{l_\text{p}^3} \left( \frac{t}{t_\text{p}} \right)^{-2}$$

where $E_\text{p} = \frac{c^5}{\hbar G} \approx 1.2 \times 10^{28} \, \text{J}$ is the Planck energy, $l_\text{p} = \sqrt{\frac{\hbar G}{c^3}} \approx 1.6 \times 10^{-35} \, \text{m}$ is the Planck length and $t_\text{p} = \sqrt{\frac{\hbar G}{c^5}} \approx 5.4 \times 10^{-44} \, \text{s}$ is the Planck time.

The time of emission of light which is observed to have a redshift of $z$ at the present time is given by

$$\tag{7.3.24} t_e = \frac{2}{3H_0(1+w)}(1+z)^{-\frac{3}{2}(1+w)}$$

This can be rearranged for the redshift as

$$\tag{7.3.25} 1 + z = \left( \frac{t_e}{t_0} \right)^{-\frac{2}{3(1+w)}}$$

The proper distance to the object at the present time is given by

$$\tag{7.3.26} d_p (t_0) = \frac{c}{H_0} \frac{2}{3(1+w)} \left[ 1 - \left(\frac{t_e}{t_0}\right)^{\frac{1+3w}{3+3w}} \right]$$

The proper distance to the object at the time of emission is $d_p(t_e) =\frac{ d_p(t_0) }{(1+z)}$.

The particle horizon distance is given by

$$\tag{7.3.27} d_\text{hor} = \frac{c}{H_0} \frac{2}{1+3w}$$

For a matter dominated universe,

- $a_\text{m}(t) = (t/t_0)^{2/3} \implies a \propto t^{2/3}$
- $t_0 = \frac{2}{3H_0}$
- $d_\text{hor}(t_0) = 3ct_0 = \frac{2c}{H_0}$
- $d_p(t_0) = \frac{2c}{H_0} \left[ 1 - (1+z)^{-1/2} \right]$
- $d_p(t_e)$ is maxiumum for $z = 1.25$.

Such a universe is also called an Einstein-de Sitter universe.

For a radiation dominated universe,

- $a_\text{r}(t) = (t/t_0)^{1/2} \implies a \propto t^{1/2}$
- $t_0 = \frac{1}{2H_0}$
- $d_\text{hor}(t_0) = 2ct_0 = \frac{c}{H_0}$
- $d_p(t_0) = \frac{c}{H_0} \left[ 1 - (1+z)^{-1} \right]$
- $d_p(t_e)$ is maximum for $z = 1$.
- $\varepsilon_r(t) = \frac{3}{32} \frac{E_\text{p}}{l_\text{p}^3} \left( \frac{t}{t_\text{p}} \right)^{-2} $
- $T(t) = \left( \frac{45}{32 \pi^2} \right)^{1/4} T_\text{p} \left( \frac{t}{t_\text{p}} \right)^{-1/2}$
- $N(t) = n(t) V_\text{hor}(t) \approx 1.9 \left( \frac{t}{t_\text{p}} \right)^{3/2}$

where $T_\text{p} = \left( \frac{c^5}{\hbar G} \right)^{1/4} \approx 1.4 \times 10^{32} \, \text{K}$ is the Planck temperature, and $N(t)$ is the number of particles within the particle horizon.

For a cosmological constant dominated universe,

- $H_0 = \sqrt{\frac{\Lambda}{3}}$
- $a_\Lambda(t) = e^{H_0 (t-t_0)} \propto e^{H_0 t}$
- $d_p(t_0) = \frac{c}{H_0} z$
- $d_p(t_e) = \frac{c}{H_0} \frac{z}{1 + z}$. As $z$ tends to $\infty$, $d_p(t_e)$ approaches $\frac{c}{H_0}$.

Such a universe is infinitely old, and has an infinite event horizon distance.

A universe with $\Lambda > 0$ is called a de Sitter universe. The de Sitter universe is a solution to Einstein's field equations with a positive cosmological constant, and describes a universe that is expanding exponentially.

A universe with $\Lambda < 0$ is called an anti-de Sitter universe. The anti-de Sitter universe is a solution to Einstein's field equations with a negative cosmological constant, and describes a universe that is contracting exponentially.

A universe with $\Lambda = 0$ is called a Minkowski or flat universe. The Minkowski universe is a solution to Einstein's field equations with zero cosmological constant, and describes a universe that is flat and static. This is the first case we discussed.

## Deceleration Parameter

Taylor expanding the scale factor gives

$$
\begin{align*}
\tag{7.3.28} a(t) &= a_0 + \dot{a}_0 (t - t_0) + \frac{1}{2} \ddot{a}_0 (t - t_0)^2 + \ldots \\
&= 1 + H_0 (t - t_0) - \frac{1}{2} q_0 H_0^2 (t - t_0)^2 + \ldots
\end{align*}
$$

Here $q_0$ is the deceleration parameter, defined as

$$\tag{7.3.29} q_0 = - \left( \frac{\ddot{a}}{a \, H^2} \right)_{t=t_0} = \frac{1}{2} \sum_w \Omega_{w,0} (1+3w)$$
