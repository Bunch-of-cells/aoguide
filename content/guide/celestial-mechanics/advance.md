---
title: Advance Topics
weight: 7
---

## Laplace-Runge-Lenz Vector

For an inverse square law force of the form

$$\mathbf{F} = -\frac{k}{r^2} \hat{\mathbf{r}}$$

and the corresponding potential energy $V(r) = -k/r$, the **super** useful Laplace-Runge-Lenz vector, or LRL vector is defined as

$$\tag{3.7.1} \boxed{ \mathbf{A} = \mathbf{p} \times \mathbf{L} - m k \hat{\mathbf{r}} } $$

$\mathbf{p}$ and $\mathbf{L}$ are the linear and angular momentum of the particle at any instant, and $\hat{\mathbf{r}}$ is the unit vector pointing from the center of mass to the particle. The constant parameter k describes the strength of the central force; it is equal to $GMm$ for gravitational forces. The LRL vector is a scaled version of the eccentricity vector, $\mathbf{A} = mk \mathbf{e}$, and hence is a constant of motion. The magntidue of the LRL vector is

$$\tag{3.7.2} A^2 = m^2 k^2 + 2mEL^2 $$

where E is the total energy of the system.

### Trajectory of the momentum vector

The conservation of the LRL vector $\mathbf{A}$ and angular momentum vector $\mathbf{L}$ is useful in showing that the momentum vector $\mathbf{p}$ moves on a circle under an inverse-square central force.

$$ mk \hat{\mathbf{r}} = \mathbf{p} \times \mathbf{L} - \mathbf{A} $$

$$\implies (mk)^2 = A^2 + p^2L^2 + 2\mathbf{A} \cdot (\mathbf{p} \times \mathbf{A}) $$

Choosing $\mathbf{L}$ along the $z$-axis, and the major semiaxis as the $x$-axis, yields the locus equation for $\mathbf{p}$

$$\tag{3.7.3} p_x^2 + \left( p_y - \frac{A}{L} \right)^2 = \left( \frac{mk}{L} \right)^2 $$

Thus, the momentum vector $\mathbf{p}$ is confined to a circle of radius $mk/L = L/p$ centered on $(0,\, A/L)$. For unbounded orbits, $A > mk$ and hence the circle does not intersect the $p_x$-axis.

### Precession of LRL vector under a perturbed potential

Consider a small perturbation $h(r)$ to the potential energy $V(r)$, such that

$$ V(r) = -\frac{k}{r} + h(r) $$

Since the force is no longer inverse-square, the LRL vector is no longer conserved, and precesses, leading to precessiong of apsis.

$$ \frac{d\mathbf{A}}{dt} = - \frac{d h(r)}{dt} \, \hat{\mathbf{r}} \times \mathbf{L} = L \frac{d}{dt} h(r) \: \hat{\mathbf{\varphi}} $$

Since $\mathbf{L}$ and $E$ are still conserved, the magnitude of $\mathbf{A}$ remains constant. Writing $L = mr^2 \dot{\theta}$,

$$ \frac{d \mathbf{A}}{d \theta} = -m \frac{d}{du} h(u) \hat{\mathbf{\varphi}} $$

where $u = 1/r$. The average precession of the apsis

$$ \Delta \varphi \approx \frac{|\Delta \mathbf{A}|}{A} = \frac{m}{A} \int_0^{2 \pi} \frac{d}{du} h(u) d \theta $$

The rate of precession is therefore given by

$$\tag{3.7.4} \dot{\varphi} = \frac{m}{AT} \int_0^{2 \pi} \frac{d}{du} h(u) d \theta $$

If the perturbation is small, the orbit during one revolution can be approximated as keplerian

$$ u = \frac{mk}{L^2} \left[ 1 + \frac{A}{mk} \cos \theta \right] $$

and hence the integral can be evaluated.

For example, the potential due to a point mass in general relativity is given by

$$\tag{3.7.5} V(r) = - \frac{GMm}{r} - \frac{GML^2}{mc^2r^3}$$

Evaluating the integral gives

$$\tag{3.7.6} \Delta \varphi = \frac{6 \pi G^2M^2m^2}{c^2L^2}$$

## Orbit Equation

<!-- gravitational radiation (GW), effective V, u'' + u = k (+GR) -->
