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

Thus, the momentum vector $\mathbf{p}$ is confined to a circle of radius $mk/L$ centered on $(0,\, A/L)$. For unbounded orbits, $A > mk$ and hence the circle does not intersect the $p_x$-axis.

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

The energy of a particle of mass $m$ moving in a central potential $V(r)$ is

$$E = \frac{1}{2}mv^2 + V(r) = \frac{1}{2}m(\dot{r}^2 + r^2 \dot{\theta}^2) + V(r)$$

Differentiating with respect to time, and substituting the $L = mr^2 \dot{\theta}$, we get the equaiton of motion of the particle

$$ m\ddot{r} - \frac{L^2}{m r^3} = - \frac{dV}{dr} $$

Substituting $u = 1/r$ and simplifying, we get

$$\tag{3.7.7} \frac{d^2 u}{d \theta^2} + u = -\frac{m}{L^2} \frac{d}{du} V(u) $$

This is the orbit equation. For an inverse square force having potential $V(r) = -k/r = -ku$, the orbit equation $u(\theta)$ is given by

$$\tag{3.7.8} \frac{d^2 u}{d \theta^2} + u = -\frac{km}{L^2} $$

This is, again, the equation of a conic section. The solution $u(\theta)$ is

$$ u = \frac{mk}{L^2} \left( 1 + e \cos (\theta - \theta_0) \right) $$

where $e$ (the eccentricity) and $\theta_0$ (the phase offset) are constants of integration.

### Precession of apasis in General Relativity

The orbit equation in general relativity is given by

$$ \frac{d^2 u}{d \theta^2} + u = \frac{GMm^2}{L^2} + \frac{3GM}{c^2} u^2 $$

Defining a dimensionless $w = \frac{L^2}{GMm^2} u$ and $\alpha = \frac{2G^2M^2m^2}{c^2L^2} \:\: (\ll 1)$,

$$ \frac{d^2 w}{d \theta^2} + w = 1 + \alpha w^2 $$

Since $\alpha$ is very small, we can use perturbation methods to find an approximate solution for $w$. In the first order, $w (\alpha)$ can be expanded in terms of a power series as

$$ w = w_0 + \alpha w_1 $$

$w_0$ just gives the newtonian solution

$$ \frac{d^2 w_0}{d \theta^2} + w_0 = 1 \implies w_0 = 1 + e \cos \theta $$

For $w_1$, we get

$$ \frac{d^2 w_1}{d \theta^2} + w_1 \approx w_0^2  = 1 + \frac{e^2}{2} + 2 e \cos \theta +\frac{e^2}{2} \cos 2 \theta $$

This gives the solution for $w_1$ as

$$ w_1 = 1 + \frac{e^2}{2} + e \theta \sin \theta - \frac{e^2}{6} \cos 2 \theta $$

Putting everything together and neglecting the small terms, we get

$$ w \approx 1 + e \cos \left[ (1 - \alpha) \, \theta \right] $$

The period of the ellipse is not $2 \pi$, and hence precesses at a rate of

$$ \Delta \varphi = \frac{2 \pi}{1 - \alpha} \approx 2\pi (1 + \alpha) = \frac{2\pi G^2 M^2 m^2}{c^2L^2} $$

which matches the result which we obtained via the precession of the LRL vector. This apsidal precession is prominent in the orbit of Mercury.

## Orbits in General Relativity

As shown earlier, elliptical orbits in general relativity tend to precess. The energy conservation equation is given by

$$ \frac{1}{2} \dot{r}^2 + \frac{h^2}{2r^2} - \frac{GM}{r} - \frac{GMh^2}{c^2 r^3} = \epsilon $$

where the central body of mass $M$ is much more massive than the orbiting body of mass $m$ and is essentially at rest. Here $\epsilon$ is a term related to the energy of the system, and $h$ is the specific angular momentum of the orbiting body. For a circular orbit, $\dot{r} = 0$, which gives the radius of the orbit as

$$\tag{3.7.9} r = \frac{h^2}{2GM} \left[ 1 \pm \sqrt{1 -\frac{12G^2M^2}{c^2h^2}} \right] $$

We see that for a given angular momentum $h$, two circular orbits are possible. Introducing $a = h/c$ and the schwarschild radius $r_s = \frac{2GM}{c^2}$,

$$ r = \frac{a^2}{r_s} \left( 1 \pm \sqrt{1 - \frac{3r_s^2}{a^2}} \right) $$

Therefore for a circular orbit, $a > \sqrt{3} r_s$. This puts a limit on the minimum angular momentum of the body.

The inner orbit

$$ r_\text{inner} = \frac{a^2}{r_s} \left( 1 - \sqrt{1 - \frac{3r_s^2}{a^2}} \right) $$

is unstable, while the outer orbit

$$ r_\text{outer} = \frac{a^2}{r_s} \left( 1 + \sqrt{1 - \frac{3r_s^2}{a^2}} \right) $$

is stable. Therefore the minimum radius of a stable circular orbit is when $a^2 = 3r_s^2$

$$\tag{3.7.10} r = \frac{a^2}{r_s} = 3r_s = \frac{6GM}{c^2} $$

In the limit $a \gg r_s$,

$$\tag{3.7.11} r_\text{outer} = \frac{2a^2}{r_s} = \frac{h^2}{GM}\,,\qquad\qquad r_\text{inner} = \frac{3}{2} r_s = \frac{3GM}{c^2} $$

Circular orbits with radius smaller than $\frac{3}{2} r_s$ are not possible. For massless particles (photons), the only circular orbit possible is at $r = \frac{3}{2} r_s$.

## Gravitational Waves

Consider two massive bodies $M_1$ and $M_2$ orbiting each other, with position vectors $\mathbf{r_1}$ and $\mathbf{r_2}$ relative to the center of mass. We define $M = M_1 + M_2$ and $m = \frac{M_1 M_2}{M_1 + M_2}$.

According to general theory of relativity, accelerated masses with non zero quadrouple moments radiate gravitataional waves (GWs) and lose energy. For small enough velocities, the emitted GWs

- have a frequency twice as large as the orbital frequency
- can be characterized by a luminosity, which is dominated by the expression

$$ P = \frac{32}{5} \frac{G}{c^5}m^2 a^4 \Omega^6 $$

where $a$ is the orbital separation and $\Omega$ is the angular velocity of each mass.

The energy of the system is $E = - \frac{GMm}{2a}$. Differentiating, we get

$$ \left( \frac{d \Omega}{dt} \right)^3 = \left( \frac{96}{5} \right)^3 \frac{\Omega^{11}}{c^5} (GM_c)^5 $$

where we define the chirp mass $M_c = m^{3/5} M^{2/5}$.

Now, $f_\text{GW} = 2f = \frac{\Omega}{\pi}$ gives

$$ f_\text{GW}^{-8/3} (t) = \frac{(8 \pi)^{8/3}}{5} \left( \frac{GM_c}{c^3} \right)^{5/3} (t_0 - t) $$

where $t_0$ is a constant of integration.
