---
title: Geometry of the Universe
weight: 2
---

## Curvature of the Universe

The universe can have 3 basic geometries:

### Flat

In a flat universe, if a triangle is constructed, with vertices joined by geodesics, the angles at the vertices $\alpha$, $\beta$ and $\gamma$ must satisfy

$$ \alpha + \beta + \gamma = \pi $$

A plane has infinite area with no edges or boundaries.

### Positively Curved (Closed)

In a spherical or positively curved geometry, the geodesics are part of great circles. The angles of a triangle satisfy

$$ \alpha + \beta + \gamma = \pi + \frac{A}{R^2} $$

where $A$ is the area of the triangle and $R$ is the radius of the sphere. A sphere has finite area $4\pi R^2$, but no edge or boundary.

### Negatively Curved (Open)

A negatively curved geometry includes a hyperboloid. The angles of a triangle satisfy

$$ \alpha + \beta + \gamma = \pi - \frac{A}{R^2} $$

where $A$ is the area of the triangle and $R$ is the radius of curvature. A hyperboloid has infinite area and no edge or boundary.

We defined $\kappa$ as the curvature constant and $R$ as the radius of curvature, such that

$$ \kappa = \begin{cases} +1 &\text{positively curved} \\ 0 &\text{flat} \\ -1 &\text{negatively curved} \end{cases} $$

Hence the sum of the angles of a triangle can be expressed as

$$ \alpha + \beta + \gamma = \pi + \frac{\kappa A}{R^2} $$

Generally, $R (t)$ is a function of time. If $R_0$ is the radius of curvature at the present time, then the scale factor $a(t)$ is defined as

$$ a(t) = \frac{R(t)}{R_0} $$

The value of the scale factor at present time is $a(t_0) = 1$.

## FLRW Metric

The expanding universe can be described by the Friedmann-Lemaître-Robertson-Walker (FLRW) metric, which is a solution to the Einstein field equations of general relativity. The FLRW metric is

$$ ds^2 = -c^2 dt^2 + a(t)^2 \left[ \frac{dx^2}{1 - \kappa x^2 / R_0^2} + x^2 d \Omega^2 \right] $$

or

$$ ds^2 = -c^2 dt^2 + a(t)^2 \left[ dr^2 + S_\kappa (r)^2 d \Omega^2 \right] $$

where $d\Omega^2 = d\theta^2 + \sin^2 \theta d\phi^2$ is the differential solid angle, and $S_\kappa (r)$ is defined as

$$ S_\kappa (r) = \begin{cases} R \, \sin \left( \frac{r}{R} \right) &\kappa = +1\\ r &\kappa = 0\\ R \, \sinh \left( \frac{r}{R} \right) &\kappa = -1\end{cases} $$

and $x = S_\kappa (r)$.

The spatial component of the FLRW metric is scaled by the scale factor $a(t)$. The time variable $t$ is the cosmic time, which is the time measured by an observer who sees the univserse expanding uniformly around him/her. The spatrial variables ($r$, $\theta$, $\phi$) or ($x$, $\theta$, $\phi$) are the comoving coordinates of a point in space. If the expansion of the universe is perfectly homogeneous and isotropic, the comoving coordinates of a point remain constant with time.

### Proper Distance

The proper distance $d_\text{p}$ between two points in space is defined as the length of the geodesic between them when the cosmic time is fixed at a value $t$. It can be found using the FLRW metric that

$$ ds^2 = a(t)^2 \left[ dr^2 + S_\kappa (r)^2 d\Omega^2 \right] $$

Along the spatial geodesic between the observer and the object, ($\theta$, $\phi$) are constant, therefore

$$ ds = a(t) dr $$
$$ \implies d_\text{p}(t) = a(t) r $$

Or

$$ d_\text{p}(t) = \begin{cases} a(t) \, R \, \sin^{-1} \left( \frac{x}{R} \right) &\kappa = +1\\ a(t) \, x &\kappa = 0\\ a(t) \, R \, \sinh^{-1} \left( \frac{x}{R} \right) &\kappa = -1\end{cases} $$

Differentiating the proper distance with respect to time gives

$$ \dot{d_\text{p}(t)} = \frac{\dot{a}}{a} d_\text{p}(t) $$

or

$$ v_\text{p}(t) = H(t) d_\text{p} (t) $$

where $v_\text{p}(t) = \dot{d_\text{p}(t)}$ is the object's proper velocity and $H(t) = \frac{\dot{a}}{a}$ is the Hubble parameter at some time $t$.

Since light travels along null geodesics, $ds = 0$. Therefore by the FLRW metric, we have

$$ d_\text{p} (t_0) = \int_{t_\text{e}}^{t_0} dr = c \int_{t_\text{e}}^{t_0} \frac{dt}{a (t)} $$

If we observe a galaxy's emission line $\lambda_0$ at time $t_0$, and it was emitted with a shorter wavelength $\lambda_\text{e}$ at time $t_\text{e}$, then

$$ \frac{\lambda_0}{a(t_0)} = \frac{\lambda_\text{e}}{a(t_\text{e})} \implies \lambda(t) \propto a(t) $$

This change in wavelength is what leads to redshift. The redshift $z$ is given by

$$ 1 + z = \frac{\lambda_0}{\lambda_\text{e}} = \frac{a(t_0)}{a(t_\text{e})} = \frac{1}{a(t_\text{e})} $$

The Hubble time is defined as $t_\text{H} = H_0^{-1}$.

The Hubble distance is defined as

$$ d_\text{H} = \frac{c}{H_0} $$

beyond which $v_\text{p} > c$.

## Distance Measures

If the luminosity of an object is known to be $L$, and flux recieved from that body is $F$, its luminosity distance $d_\text{L}$ is given by

$$ d_\text{L} = \sqrt{\frac{L}{4 \pi F}} $$

Using the FLRW metric, we get $d_\text{L} = S_\kappa (r) (1+z)$. If $\kappa = 0$, $d_\text{L} = d_\text{p} (t_0) (1+z)$.

The angular diameter distance is defined as

$$ d_A = \frac{l}{\theta} $$

where $l$ is the length of the object and $\theta \ll 1$ is the angle subtended by the object at the observer.

Using FLRW metric, we get $d_A = \frac{d_\text{p} (t_0)}{1+z}$. The angular diameter distance is related to the luminosity distance by

$$ d_\text{L} = (1+z)^2 \, d_A$$

In an expanding universe, $d_\text{L} > d_A$.

In a flat universe, the flux recieved from a source with redshift $z$ is

$$ F = \frac{L}{4 \pi d_\text{p}^2} \cdot \frac{1}{1+z} \cdot \frac{1}{1+z}$$

The first factor of $1+z$ comes from the fact that as the photons are redshifted, their energy decreases. The second factor of $1+z$ comes from the fact that the interval of time between the emission and reception of the photons is $dt_\text{e} = dt_0 (1+z)$.

The reason why a factor of $1+z$ comes in the angular diameter distance is because the object which we are viewing is that what it looked like when the light was emitted. The object is not at the same distance as it was when the light was emitted. The object is at a distance $d_\text{p} (t_0)$, but the light was emitted at a distance $d_\text{p} (t_\text{e}) = \frac{d_\text{p}(t_0)}{1+z}$.

### Cosmic Horizons

The cosmic event horizon is the maximum comoving distance a light beam emitted now can travel

$$ d_\text{EH} = \int_{t_0}^{\infty} \frac{c}{a(t)} dt$$

The most distant objects one can see are those for which light emitted at $t = 0$ is just reaching us now at $t = t_0$. The proper distance to such an object is called the particle horizon distance

$$ d_\text{hor} = \int_{0}^{t_0} \frac{c}{a(t)} dt$$

The portion of the universe lying within the horizon, called the visible universe, is causally coneected to the observer.

At present time, $d_\text{H}(t_0) \: (\approx 4.3 \, \mathrm{Gpc}) < d_\text{EH}(t_0) \: (\approx 5 \, \mathrm{Gpc} ) < d_\text{hor}(t_0) \: (\approx 14.4 \, \mathrm{Gpc})$.
