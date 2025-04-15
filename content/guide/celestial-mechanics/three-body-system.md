---
title: Three Body Systems
weight: 5
---

The three-body problem is to take the initial positions and velocities of three point masses that orbit each other in space and calculate their subsequent trajectories using Newton's laws of motion and Newton's law of universal gravitation. There exists no general closed form solution to the three body problem. When three bodies orbit each other, the resulting dynamical system is chaotic for most initial conditions. Because there are no solvable equations for most three-body systems, the only way to predict the motions of the bodies is to estimate them using numerical methods.

A class of three body problems, called the restricted three body problem is as follows: two massive bodies, called primaries, orbit each other in a circular orbit, and a third body of negligible mass moves under the influence of the two massive bodies. The third body does not affect the motion of the two massive bodies. The restricted three-body problem is easier to analyze theoretically than the full problem.

There do exist some special configurations, for which solutions to the three body problem are known:

- Lagrange points: This is a solution to the restricted three body problem. Five points exist in the orbital plane of two massive bodies, where a third body can be placed and remain in a stable position relative to the two massive bodies. The Lagrange points are denoted $L_1$, $L_2$, $L_3$, $L_4$, and $L_5$. The $L_4$ and $L_5$ points are stable, while the others are unstable.
- 8 shaped orbit: This is a solution to the full three body problem. Three bodies of equal masses can orbit each other in a figure-eight pattern. This solution is known as the Chenciner–Montgomery orbit. The total angular momentum of such a system is zero, and the three bodies lie in a plane.

## Virial Theorem

Suppose we have a system of $n$ point masses $m_i$ with position vectors $\mathbf{r}_i$ and velocities $\mathbf{v}_i$. We define the virial of the system as

$$\tag{3.5.1} A = \sum_{i=1}^n m_i \mathbf{v_i} \cdot \mathbf{r_i} $$
$$\implies \dot{A} = 2\,K + \sum_{i=1}^n \mathbf{F_i} \cdot \mathbf{r_i} $$

where $K$ is the total kinetic energy of the system. Let $\lang x \rang$ denote the time average of $x$ in the interval $[0, \tau]$

$$ \lang \dot{A} \rang = \frac{1}{\tau} \int_0^\tau \dot{A} dt = \frac{A(\tau)}{\tau} = 2\, \lang K \rang + \lang \sum_{i=1}^n \mathbf{F_i} \cdot \mathbf{r_i} \rang  $$

If the system remains bound, $A$ remains finite. As $\tau \rightarrow \infty$, $\frac{A}{\tau} \rightarrow 0$, hence we get that $2 \lang K \rang + \lang \sum_{i=1}^n \mathbf{F_i} \cdot \mathbf{r_i} \rang = 0 $. If the forces are due to mutual gravity only, $\sum_{i=1}^n \mathbf{F_i} \cdot \mathbf{r_i} = U$ is the total potential energy of the system. Hence we get that

$$\tag{3.5.2} \boxed{2 \, \lang K \rang + \lang U \rang = 0 }$$

This is the virial theorem, and is very useful.

## Tidal Forces

Tidal force is the difference in gravitational attraction between different points on a body, causing the body to be pulled unevenly and as a result are being stretched towards the attraction. Tidal forces are a secondary effect of gravity, making the closer near-side more attracted than the more distant far-side. Phenomenon caused by tidal forces include:

- Ocean tides and solid-earth tides
- Tidal locking
- breaking apart of celestial bodies and formation of ring systems within the Roche limit
- spaghettification of objects near black holes
- tidal heating of moons and planets

Tidal acceleration does not require rotation or orbiting bodies; for example, the body may be freefalling in a straight line under the influence of a gravitational field while still being influenced by (changing) tidal acceleration.

Consider a body of mass $M$, kept at a distance $r$ from a spherical body of radius $R$. Define

- $\mathbf{s}$ as the position vector of mass $m$ on the surface of the sphere relative to the massive body $M$
- $\mathbf{R}$ as the position vector of mass $m$ relative to the center of mass of the sphere
- $\mathbf{r}$ as the position vector of the sphere relative to the massive body $M$

Since the sphere accelerates towards the massive body $M$ with $\mathbf{a} = -\frac{GM}{r^2} \hat{\mathbf{r}}$, the force on mass $m$ is given by

$$\mathbf{F}_\text{net} = -\frac{GMm}{s^2} \hat{\mathbf{s}} + \frac{GMm}{r^2} \hat{\mathbf{r}} + \sum \mathbf{F}_\text{other} $$

The last term persists in the absence of M while the first two terms arise from the presence of M — the combination of these two additional terms is known as the tidal force $\mathbf{F}_\text{tidal}$, and the acceleration caused is called the tidal acceleration $\mathbf{a}_\text{tidal}$

$$\tag{3.5.3} \mathbf{a}_\text{tidal} = -GM \left( \frac{\hat{\mathbf{s}}}{s^2} - \frac{\hat{\mathbf{r}}}{r^2} \right) $$

Since $\mathbf{s} = \mathbf{r} + \mathbf{R}$,

$$ \mathbf{a}_\text{tidal} = -GM \left( \frac{\mathbf{r} + \mathbf{R}}{|\mathbf{r} + \mathbf{R}|^3} - \frac{\mathbf{r}}{r^3} \right) $$

Usually $r \gg R$, so we can take few approximations, which finally give

$$\tag{3.5.4} \boxed{ \mathbf{a}_\text{tidal} \approx -\frac{GM}{r^3} \left[ \mathbf{R} - 3\, ( \hat{\mathbf{r}} \cdot \mathbf{R} )\, \hat{\mathbf{r}} \right] } $$

Consider a cartesian coordinate system with its origin at the center of the sphere, the $x$-axis pointing towards the massive body, and $y$-axis oriented such that $\mathbf{R}$ lies in the $xy$-plane. If the angle $\theta$ is the angle between the $x$-axis and the vector $\mathbf{R}$, the tidal acceleration experienced by $m$ is

$$\tag{3.5.5} \boxed{\mathbf{a}_\text{tidal} = \frac{GMR}{r^3} (2\cos \theta \, \hat{\mathbf{i}} - \sin \theta \, \hat{\mathbf{j}}) }$$

We see that when $R$ and $r$ are parallel, i.e. $m$ lies on the line joining $M$ and the center of the sphere, the tidal acceleration is

$$\mathbf{a}_\text{tidal} = -2\frac{GM \mathbf{R}}{r^3}$$

When $R$ and $r$ are perpendicular, i.e. $m$ lies on the line perpendicular to the line joining $M$ and the center of the sphere, the tidal acceleration is

$$\mathbf{a}_\text{tidal} = -\frac{GM \mathbf{R}}{r^3}$$

The tidal acceleration is maximum when $R$ and $r$ are parallel, and minimum when they are perpendicular.

## Roche Limit

The Roche limit or Roche radius is the distance from a massive primary body within which a second body held together only by its own gravity, will disintegrate due to tidal forces. The Roche limit typically applies to a satellite's disintegrating due to tidal forces induced by its primary, the body around which it orbits.

Let $R_M$, $\rho_M$ and $M_M$ be the radius, density and mass of the primary (larger) body and $R_m$, $\rho_m$ and $M_m$ be the radius, density and mass of the satellite. The satellite is at a distance $d$ from the primary. For the satellite to be held together by its own gravity, the tidal force must be less than the gravitational force acting on the satellite. We get the Roche limit when these two interactions are equal.

$$ 2 \frac{GM_M R_m m'}{d^3} = \frac{GM_m m'}{R_m^2} $$

where $m'$ is a mass closest to the primary body, on the satellite's surface. This gives

$$\tag{3.5.6} \boxed{ d = R_m \left( \frac{2M_m}{M_m} \right)^{1/3} = R_M \left( \frac{2 \rho_m}{\rho_m} \right)^{1/3}} $$

The above expression is for a rigid satellite. For a fluid satellite,

$$ d \approx 2.44\, R_M \left( \frac{\rho_m}{\rho_m} \right)^{1/3} $$

## Hill Sphere

The Hill sphere is the region around a celestial body where its own gravity (compared to other nearby bodies) is the dominant force in attracting satellites. It is also known as the Roche sphere. If a less massive body $m$ orbits a more mass body $M$ ($M \ll m$), and has an instantaneous distance $a$ from $M$, then its hill radius (at that instant) is

$$\tag{3.5.7} \boxed{ R_H \approx a \left( \frac{m}{3(M + m)} \right)^{1/3} } $$

For Earth, this is approximately $0.01 \mathrm{\,AU}$. The derivation of the hill radius is similar to that of the $L_1$ and $L_2$ Lagrange points.

## Lagrange Points

In the restricted three body problem, the third body can remain at rest relative to the primaries at certain points. There are five such points, called Lagrange points. The Lagrange points are denoted $L_1$, $L_2$, $L_3$, $L_4$, and $L_5$. The points $L_1$, $L_2$ and $L_3$ are unstable, and lie on the line joining the two primaries. The points $L_4$ and $L_5$ are stable, and lie at the vertices of an equilateral triangle with the two primaries. When seen in a rotating reference frame, a body kept at one of the Lagrange points matches the angular velocity of the two co-orbiting primaries, allowing it to remain stationary relative to them. At the Lagrange points, the net gravitational force acting on the third body is equal to the centrifugal force acting on it. The barycenter is defined to be center of mass of the three-body system, which is also the center of rotation of the three-body system.

Asteroids and comets are often found at the Lagrange points of the Sun and Jupiter. The Lagrange points are also used for placing satellites in orbit. Asteroids found around Jupiter's $L_4$ and $L_5$ points are called Trojan asteroids.

Let the masses of the two primaries be $M$ and $m$ ($M > m$), separated at a distance $R$, Their angular velocity is given by

$$ \omega = \sqrt{ \frac{G(M + m)}{R^3} } $$

### L <sub>1</sub>

The $L_1$ point lies between the two primaries, and its distance $r$ from the small primary is given by

$$ \frac{GM}{(R-r)^2} - \frac{Gm}{r^2} = \left( \frac{m}{M + m} R - r \right) \omega^2 $$

If $M \gg m$, then $L_1$ and $L_2$ are approximately at the same distance $r$ from the smaller primary, equal to the hill radius, given by

$$\tag{3.5.8} r \approx R \sqrt[3]{\frac{m}{M+m}} $$

### L <sub>2</sub>

The $L_2$ point lies on the opposite side of the larger primary, and its distance $r$ from the smaller primary is given by

$$ \frac{GM}{(R+r)^2} + \frac{Gm}{r^2} = \left( \frac{m}{M + m} R + r \right) \omega^2 $$

Again, if $M \gg m$, then $L_1$ and $L_2$ are approximately at the same distance $r$ from the smaller primary, equal to the hill radius, given by

$$ r \approx R \sqrt[3]{\frac{m}{M+m}} $$

<br>

We can also write this relation as

$$ \frac{m}{r^3} \approx \frac{M}{R^3} $$

Now, since $F_\text{tidal} \propto \frac{M}{R^3}$, we find that the tidal effect of the smaller body at the $L_1$ or at the $L_2$ point is about three times of that body. We can also write the relation as

$$ \rho_2 \alpha_2^3 \approx 3 \rho_1 \alpha_1^3 $$

where $\rho$ is the density of the primary and $\alpha$ is its angular size, as seen from $L_1$ or $L_2$. This shows that viewed from these two Lagrange points, the apparent sizes of the two bodies will be similar, especially if the density of the smaller one is about thrice that of the larger, as in the case of the earth and the sun. Looking toward the sun from $L_2$ one sees an annular eclipse. Therefore it is necessary for a spacecraft parked at $L_2$, to follow a Lissajous orbit or a halo orbit around $L_2$ in order for its solar panels to get full sun.

### L <sub>3</sub>

The $L_3$ point lies on the opposite side of the smaller primary, and its distance $r$ from the orbit of the smaller primary is given by

$$ \frac{GM}{(R-r)^2} + \frac{Gm}{(2R-r)^2} = \left( \frac{m}{M + m} R + R - r \right) \omega^2 $$

If $M \gg m$, then

$$\tag{3.5.9} r \approx \frac{7}{12}\frac{m}{M+m}R $$

### L <sub>4</sub> and L <sub>5</sub>

The reason these points are in balance is that at $L_4$ and $L_5$ the distances to the two primaries are equal. Accordingly, the gravitational forces from the two primary bodies are in the same ratio as the masses of the two bodies, and so the resultant force acts through the barycenter of the system. Additionally, the geometry of the triangle ensures that the resultant acceleration is to the distance from the barycenter in the same ratio as for the two primaries. This resultant force is exactly that required to keep the smaller body at the Lagrange point in orbital equilibrium with the primaries.

## Orbital Resonance

Orbital resonance occurs when orbiting bodies exert regular, periodic gravitational influence on each other, usually because their orbital periods are related by a ratio of small integers. Examples are the 1:2:4 resonance of Jupiter's moons Ganymede, Europa and Io, and the 2:3 resonance between Neptune and Pluto. Unstable resonances with Saturn's inner moons give rise to gaps in the rings of Saturn. The special case of 1:1 resonance between bodies with similar orbital radii causes large planetary system bodies to eject most other bodies sharing their orbits; this is part of the much more extensive process of clearing the neighbourhood around planets.

A binary resonance ratio should be interpreted as the ratio of number of orbits completed in the same time interval, rather than as the ratio of orbital periods, which would be the inverse ratio. Thus, the 2:3 ratio above means that Pluto completes two orbits in the time it takes Neptune to complete three.

A mean-motion orbital resonance occurs when two bodies have periods of revolution that are a simple integer ratio of each other.

A spin orbit resonance is where the spin period of the planet is connected to the orbital period by a simple ratio. For circular orbits, only such resonance possible is 1:1, where the planet is tidally locked to the star. For elliptical orbits, other resonances are possible. Mercury has a spin orbit resonance or 3:2 with the sun, where it rotates three times on its axis for every two revolutions around the sun.

## n-body problem

The n-body problem is the problem of predicting the individual motions of a group of celestial objects interacting with each other gravitationally. It consists of n point mass $m_i$, with position vectors $\mathbf{r}_i$ and velocities $\mathbf{v}_i$. The equations of motion are given by

$$ \ddot{\mathbf{r}_i} = \sum_{\substack{j=0 \\ j \neq i}}^{n} \frac{G m_i m_j}{|\mathbf{r}_j - \mathbf{r}_j|^3} (\mathbf{r}_j - \mathbf{r}_i) $$

There is no general closed form solution for $n >2$.

## Problems

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    Find the first cosmic velocity, which is the least velocity of a satellite launched from the surface of Earth required to put a satellite into orbit around the earth.
    {{< /tab >}}

    {{< tab >}}
    The first cosmic velocity is given by

    $$\tag{3.5.11} v_1 = \sqrt{\frac{GM_\oplus}{R_\oplus}} \approx \boxed{7.91 \mathrm{\,km/s}}$$

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    Find the second cosmic velocity, which is the least velocity of a satellite launched from the surface of Earth required to escape from the gravitational field of the earth.
    {{< /tab >}}

    {{< tab >}}
    The second cosmic velocity is given by

    $$\tag{3.5.12} v_2 = \sqrt{\frac{2GM_\oplus}{R_\oplus}} \approx \boxed{11.2 \mathrm{\,km/s}}$$

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    Find the third cosmic velocity, which is the least velocity of a satellite launched from the surface of Earth required to escape from the gravitational field of the solar system.
    {{< /tab >}}

    {{< tab >}}
    In heliocentric frame, the escape velocity is

    $$v_{2,\odot} = \sqrt{\frac{2GM_\odot}{a_\odot}} \approx 42.1 \mathrm{\,km/s}$$

    From Earth's frame,

    $$ v' = v_{2,\odot} - v_\oplus = \sqrt{\frac{2GM_\odot}{a_\odot}} - \sqrt{\frac{GM_\odot}{a_\odot}} \approx 12.3 \mathrm{\,km/s}$$

    Therefore, we can get the third cosmic velocity by

    $$ \frac{1}{2} v_3^2 - \frac{GM_\oplus}{R_\oplus} = \frac{1}{2}v'^3 $$

    $$\tag{3.5.13} \implies v_3 = \sqrt{\frac{2GM_\oplus}{R_\oplus} + v'^2} \approx \boxed{16.7 \mathrm{\,km/s}}$$

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    $\text{(IOAA 2011)}$ Estimate the number of stars in a globular cluster of diameter 40 pc, if the escape velocity at the edge of the cluster is 6 km/s and most of the stars are similar to the Sun.
    {{< /tab >}}

    {{< tab >}}
    The escape velocity of object on the edge of the cluster is given by

    $$ v_e = \sqrt{ \frac{2GM}{R} } \implies M = \frac{Rv_e^2}{2G} $$
    $$ N = \frac{M}{M_\odot} = \frac{Rv_e^2}{2GM_\odot} \approx \boxed{ 8.4 \times 10^4 } $$
    {{< /tab >}}
{{< /tabs >}}
