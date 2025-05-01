---
title: Advanced Topics
weight: 5
---

## Lane-Emden equation

The Lane–Emden equation is a dimensionless equation that describes a Newtonian self-gravitating, spherically symmetric, polytropic fluid. It is named after astrophysicists Jonathan Homer Lane and Robert Emden. The equation reads:

$$\boxed{ \frac{1}{\xi^2} \frac{d}{d\xi^2} \left( \xi^2 \frac{d \theta}{d \xi} \right) + \theta^n = 0 }$$

where $\xi$ is a dimensionless radius and $\theta$ is related to the density, and thus the pressure, by $\rho = \rho_c \theta^n$, where  $\rho_c$ is the central density. The index $n$ is the polytropic index that appears in the polytropic equation of state,

$$P = K \rho^{1 + \frac{1}{n}}$$

where $P$ and $\rho$ are the pressure and density, respectively, and $K$ is a constant of proportionality. The standard boundary conditions are $\theta(0) = 1$ and $\theta'(0) = 0$. Solutions thus describe the pressure and density profile with radius and are known as polytropes of index $n$. These are commonly used to model stars.

### Derivation

Consider a self-gravitating, spherically symmetric fluid in hydrostatic equilibrium. Mass is conserved and thus described by the continuity equation

$$\frac{dm}{dr} = 4 \pi r^2 \rho$$

where $\rho$ is a function of $r$. The equation of hydrostatic equillibrium is

$$ \frac{1}{\rho} \frac{dP}{dr} = - \frac{Gm}{r^2} $$

where $m$ is also a function of $r$. Differentiating again gives

$$
\begin{align}
\frac{d}{dr} \left( \frac{1}{\rho} \frac{dP}{dr} \right) &= \frac{2Gm}{r^3} - \frac{G}{r^2} \frac{dm}{dr} \nonumber \\&= - \frac{2}{\rho r} \frac{dP}{dr} - 4\pi G \rho \nonumber
\end{align}
$$

Rearranging gives

$$ \frac{1}{r^2} \frac{d}{dr} \left( \frac{r^2}{\rho} \frac{dP}{dr} \right) = -4 \pi G \rho $$

If we substitue the polytropic equation of state with $P = K \rho_c^{1 + \frac{1}{n}} \theta^{n+1}$ and $\rho = \rho_c \theta^n$, we have

$$ \frac{1}{r^2} \frac{d}{dr} \left( r^2 K \rho_c^\frac{1}{n} (n+1) \frac{d\theta}{dr} \right) = -4 \pi G \rho_c \theta^n $$

Gathering the constants and substituting $r = \alpha \xi$, where

$$ \alpha^2 = (n+1) K \rho_c^{\frac{1}{n} - 1} / 4\pi G, $$

we have the Lane-Emden equation

$$ \frac{1}{\xi^2} \frac{d}{d\xi^2} \left( \xi^2 \frac{d \theta}{d \xi} \right) + \theta^n = 0 $$

The boundary conditions are:

- $\theta(0) = 1$: The density at the center of the star is $\rho_c$.
- $\theta'(0) = 0$: The density gradient at the center is zero, avoiding any discontinuity.

The surface of the fluid is defined by the condition $\theta(\xi_R) = 0$, where $\xi_R$ is the radius of the fluid. Only solutions with $n < 5$ have a surface. All polytropes with $n \geq 5$ have infinite radii.

### Solutions

- $n = 0$

The Lane-Emden equation becomes $\frac{1}{\xi^2} \frac{d}{d\xi^2} \left( \xi^2 \frac{d \theta}{d \xi} \right) = 0$. Integrating, we find that the solution is

$$ \theta(\xi) = 1 - \frac{\xi^2}{6} $$

This gives the surface to be at $\xi_R = \sqrt{6}$. This solution corresponds to an incompressible fluid star, which has the same density everywhere.

- $n = 1$

The solution for $n = 1$ is

$$ \theta(\xi) = \frac{\sin(\xi)}{\xi} $$

This extends to infinity, hence has infinite radius, unless truncated artificially. We truncate the star at the first root, where $\xi_R = \pi$.

- $n = 5$

The solution for $n = 5$ is

$$ \theta(\xi) = \left( 1 + \frac{\xi^2}{3} \right)^{-1/2} $$

This solution has no surface, as it extends to infinity.

- $n = 1.5,\, 3$

The solution corresponding to $n = 1.5$ is of an adiabatic star supported by pressure of non relativistic gas, or a white dwarf.

The solution corresponding to $n = 3$ is of an adiabatic star supported by pressure of ultra-relativistic gas, or a neutron star.

### Physical Properties

The stellar radius is

$$ R = \alpha \xi_R = \left[ \frac{K}{G} \frac{n + 1}{4 \pi} \right]^{1/2} \rho_c^\frac{1-n}{2n} \xi_R $$

The stellar mass is

$$
\begin{align}
M &= \int_0^R 4 \pi r^2 \rho dr \nonumber \\&= 4 \pi \left( \frac{K}{G} \frac{n + 1}{4 \pi} \right)^{3/2} \rho_c^\frac{3-n}{2n} \left[ -\xi^2 \frac{d \theta}{d \xi} \right]_{\xi_R} \nonumber
\end{align}
$$

From this we get that

$$ M \propto R^\frac{n-1}{3n-1} $$

The average density of the star is

$$ \rho_{av} = \frac{3M}{4 \pi R^3} = \frac{3}{\xi_R^3} \left[ -\xi^2 \frac{d \theta}{d \xi} \right]_{\xi_R} \rho_c$$

The gravitational potential energy is

$$ \Omega = - \int_0^M \frac{GM_r dM_r}{r^2} = \frac{3}{5-n} \frac{GM^2}{R} $$

## Limb Darkening

Limb darkening is the phenomenon where the center of a star appears brighter than the edges (limbs). This is due to the fact that light from the center of the star has to pass through less material than light from the edges, which has to pass through more material.

The intensity seen at some point P is only a function of the incident angle $\psi$.

$$ \frac{I(\psi)}{I(0)} = \sum_{k=0}^N a_k \cos^k \psi $$

It can also be written as

$$ \frac{I(\psi)}{I(0)} = 1 + \sum_{k=1}^N A_k (1 - \cos \psi)^k $$

For a lambertian surface, $I(\psi) = I(0) \cos \psi$, hence no limb darkening is observed (the projected area also scales as $\cos \psi$).

We have that

$$ \cos \psi = \frac{\sqrt{\cos^2 \theta - \cos^2 \Omega}}{\sin \Omega} = \sqrt{1 - \left( \frac{\sin \theta}{\sin \Omega} \right)^2} $$

For small $\theta$,

$$ \cos \psi \approx \sqrt{1 - \left( \frac{\theta}{\sin \Omega} \right)^2}$$

The mean intensity is given by

$$ \bar{I} = \frac{\int I(\psi) \, d\omega}{\int d\omega} $$

where $d\omega = \sin \theta \, d\theta \, d\phi$. We get that

$$ \bar{I} = 2I(0) \sum_{k=0}^N \frac{a_k}{k+2} $$

The radiative transfer equation is

$$ \frac{dI_\nu}{d\tau_\nu} = I_\nu - S_\nu $$

where $\tau_\nu = - \alpha_\nu \, ds$ and $ds = dr \, \cos \theta$. Defining $\mu = \cos \theta$, the equation for radial direction is therefore

$$ \mu \frac{dI}{d\tau} (\tau, \mu) = I (\tau, \mu) - S (\tau) $$

A solution upto linear terms is $I (\tau, \mu) = I_0 + I_1 \mu$. The mean intensity is

$$ J(\tau) = \frac{1}{2} \int_{-1}^{1} (I_0 + I_1 \mu) d\mu = I_0$$

The net flux is

$$ F(\tau) = \int I(\tau, \mu) \cos \theta \, d\Omega = \frac{4\pi}{3} I_1$$
$$ \implies I_1 = \frac{3 F(0)}{4\pi} $$

In radiative equilibrium, $S(\tau) = J(\tau)$. Thus the equation for radiative transfer becomes

$$ \mu \frac{dI_0}{d\tau} = I_1 \mu \implies I = I_1 (\tau + \mu) + C $$

Setting the inward flux to be zero, we get that $C = 2/3$. Hence the intensity is

$$ I = \frac{3 F(0)}{4\pi} \left( \tau + \mu + \frac{2}{3} \right) $$

At the surface of the star, $\tau = 0$, therefore we get that

$$ \frac{I(0, \theta)}{I(0, 0)} = 0.4 + 0.6 \cos \theta = 1 - u (1 - \mu) $$

where $u = 0.6$ is the limb darkening coefficient.

## Compact Stars
