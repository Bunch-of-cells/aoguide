---
title: Kepler's Laws
prev: /guide/celestial/
next: /guide/celestial/bound
---

Newton's law of universal gravitation describes gravity as a force by stating that every particle attracts every other particle in the universe with a force that is proportional to the product of their masses and inversely proportional to the square of the distance between their centers of mass. Consider two bodies of masses $m_1$ and $m_2$, with position vectors $\vec{r_1}$ and $\vec{r_2}$. The force exerted on body 2 due to body 1 is

$$ \vec{F} = -\frac{G m_1 m_2}{r^3} \vec{r} $$

We define the following:

- Separation vector: $ \vec{r} = \vec{r_2} - \vec{r_1} $
- Total mass: $M = m_1 + m_2$
- Reduced mass: $m_\mu = \frac{m_1 m_2}{m_1 + m_2}$
- Gravitational parameter: $\mu = GM$

Here G is the gravitational constant, equal to $6.67430 \times 10^{-11} \: \mathrm{m^3\,kg^{-1}\,s^{-2}}$
. Using Newton's second law $\vec{F} = m \vec{a}$, we can write

$$ \ddot{\vec{r}} = -\mu \frac{\vec{r}}{r^3} $$

Working in the center of mass frame, we have

$$ m_1 \vec{r_1} + m_2 \vec{r_2} = \vec{0} $$

Hence the individual position vectors can be expressed as

$$ \vec{r_1} = \frac{-m_2}{M} \vec{r} \,, \qquad \qquad \vec{r_2} = \frac{m_1}{M} \vec{r} $$

The total orbital angular momentum is given by

$$
\begin{align*}
\vec{L} &= m_1 \vec{r_1} \times \vec{v_1} + m_2 \vec{r_2} \times \vec{v_2}\\
        &= m_\mu \vec{r} \times \vec{v}
\end{align*}
$$

where $\vec{v} = \dot{\vec{r}}$. The total energy of the system is given by

$$
\begin{align*}
E &= \frac{1}{2} m_1 v_1^2 + \frac{1}{2} m_2 v_2^2 - \frac{G m_1 m_2}{|\vec{r_1} - \vec{r_2}|^2} \\
  &= \frac{1}{2} m_\mu v^2 - \mu \frac{m_\mu}{r^2}
\end{align*}
$$

We define the specific angular momentum and specific energy as

$$
\begin{align*}
\vec{h} &= \frac{\vec{L}}{m_\mu} = \vec{r} \times \dot{\vec{r}}\\
\varepsilon &= \frac{E}{m_\mu} = \frac{1}{2} v^2 - \frac{\mu}{r}
\end{align*}
$$

Since gravitation is a central force, the angular momentum is conserved. Moreover since it is conservative, the total energy is also conserved. Hence $\vec{h}$ and $\varepsilon$ are constants of motion.

Since $\vec{h} \cdot \vec{r} = 0$, $\vec{h}$ lies perpendicular to the plane of motion, and hence defines the plane of motion. We have

$$
\begin{align*}
\frac{d}{dt} (\vec{h} \times \dot{\vec{r}}) = \vec{h} \times \ddot{\vec{r}} &= (\vec{r} \times \dot{\vec{r}}) \times \left( -\mu \frac{\vec{r}}{r^3} \right) \\
&= -\mu \frac{1}{r^3} \left[(\vec{r} \cdot \vec{r}) \dot{\vec{r}} - (\vec{r} \cdot \dot{\vec{r}}) \times \vec{r} \right] \\
&= -\mu (\frac{\dot{\vec{r}}}{r} - \vec{r} \frac{\dot{r}}{r^2}) = \frac{d}{dt} \left(-\mu \frac{\vec{r}}{r} \right)
\end{align*}
$$

$$ \implies \frac{d}{dt} \left( \vec{h} \times \dot{\vec{r}} + \mu \frac{\vec{r}}{r} \right) = \vec{0} $$

Hence we define the eccentricity vector as

$$ \vec{e} = -\frac{\vec{h} \times \dot{\vec{r}}}{\mu} - \frac{\vec{r}}{r} $$

This is another constant of motion. It lies in the plane of motion, hence $\vec{h} \cdot \vec{e} = 0$. It points in the direction of the periapsis. The mangnitude of the eccentricity vector is

$$ e = \sqrt{1 + \frac{2 \varepsilon h^2}{\mu^2}} $$

The angle between the eccentricity vector and the position vector is called the mean anamoly

$$ \vec{r} \cdot \vec{e} = r e \cos f = \vec{r} \cdot \left( -\frac{\vec{h} \times \dot{\vec{r}}}{\mu} - \frac{\vec{r}}{r} \right) = \frac{h^2}{\mu} - r$$

$$ \implies \boxed{r = \frac{h^2 / \mu}{1 + e \cos f}} $$

This, if one may recognize, is the equation of a conic section in polar coordinates, with the focus being at origin, and length of the semi latus rectum being $p = \frac{h^2}{\mu}$. The magnitude of $\vec{e}$ determines the shape of the trajectory:

- $e = 0$: Circle
- $0 \leq e < 1$: Ellipse
- $e = 1$: Parabola
- $e > 1$: Hyperbola

where the focus of the conic section lies at the center of mass of the system.

Another trajectory is possible, which is a straight line. This is the case where $\vec{h} = \vec{0}$, and the bodies are moving directly towards each other. The eccentricity of such a trajectory is $1$. However, depending on the total energy of the system, the trajectory can be classified as:

- $\varepsilon < 0$: radial elliptic trajectory
- $\varepsilon = 0$: radial parabolic trajectory
- $\varepsilon > 0$: radial hyperbolic trajectory

The energy of the system can thus be determined by just the eccentricity $e$ and length of semi latus rectum $p$ of the trajectory. The total energy of the system is given by

$$e^2 = 1 + \frac{2h \varepsilon}{mu^2} \implies \varepsilon = \frac{1}{2} \left( e^2 - 1 \right) \frac{\mu^2}{h^2}$$

$$\boxed{\varepsilon = \frac{1}{2} \frac{\mu (1 - e^2)}{p}}$$

We see that the sign of the total energy depends on the eccentricity of the trajectory

- $0 \leq e < 1$: An elliptical trajectory gives a negative total energy, and hence a bound orbit
- $e = 1$: A parabolic trajectory gives a zero total energy, and hence an unbound orbit
- $e > 1$: A hyperbolic trajectory gives a positive total energy, and hence an unbound orbit

We see that all bound orbits are ellipses, and all unbound orbits are hyperbolae or parabolae.

For our solar system, the sun is much more massive than any of the planets, hence is nearly at the center of mass, or the focus of the elliptical orbits of all planets. This proves Kepler's first law of planetary motion, which states that the orbit of a planet is an ellipse with the sun at one of the foci.

The cross product of two vectors gives the area of a parallelogram possessing sides of those vectors, hence the triangular area $dA$ swept out in a short period of time is given by half the cross product of the $\vec{r}$ and $\vec{dx}$ vectors, for some short piece of the orbit, $dx$.

$$ dA = \frac{1}{2}|\vec{r} \times \vec{dx}| = \frac{1}{2}|\vec{r} \times \vec{v} dt| = \frac{h}{2} dt $$

$$ \implies \boxed{\frac{dA}{dt} = \frac{h}{2}} $$

which is constan. This proves Kepler's second law of planetary motion, which states that a line segment joining a planet and the sun sweeps out equal areas during equal intervals of time.

Consider two bodies moving in bound elliptical orbits, with the semi-major axis of the orbit being $a$, and the semi-minor axis being $b$. The lengths of the two axes are related by the eccentricity of the orbit, $e$, as

$$ e^2 = 1 - \frac{b^2}{a^2} $$

The area of an ellipse is $\pi a b = \pi a^2 \sqrt{1 - e^2}$. Moreover, the length of semi latus rectum is $p = \frac{b^2}{a} = a (1 - e^2)$, hence $h^2 = \mu a (1 - e^2)$

Integrating the equation of areal velocity, we have

$$
\begin{align*}
dA &= \frac{h}{2} dt\\
\int dA &= \frac{h}{2} \int dt\\
\pi a^2 \sqrt{1 - e^2} &= \frac{1}{2} \mu a (1 - e^2) P\\
\end{align*}
$$

Rearranging, we get

$$ \boxed{P^2 = \frac{4 \pi^2}{\mu} a^3} $$

If we work in the units of AU, sidereal years, and solar masses, we have $G = 4 \pi$. Hence the equation simplifies to

$$ \boxed{a^3 = M P^2} $$

In our solar system, $M = M_\odot + m_{planet} \approx M_\odot = 1$, hence we have the relation $P^2 = a^3$. This proves Kepler's third law of planetary motion, which states that the square of the period of revolution of a planet is directly proportional to the cube of the semi-major axis of its orbit.
