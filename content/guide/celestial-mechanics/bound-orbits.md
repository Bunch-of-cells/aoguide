---
title: Bound Orbits
weight: 2
---

As proved in section 3.1, all bound orbits are elliptical. Consider an ellipse with semi-major axis $a$, semi-minor axis $b$, and eccentricity $e$. The semi-major axis is half the length of longest radii of the ellipse, while the semi-minor axis is half the length of the shortest radii. The semi-minor and semi-major axis are related by

$$ b^2 = a^2 (1 - e^2) $$

The eccentricity of an ellipse is always less than 1, being 0 for a circle. The length of the periapsis, which is the point closest to the foci, and apoapsis, the point farthest from the foci, are given by

$$
\begin{align*}
r_p &= a (1 - e)\\
r_a &= a (1 + e)
\end{align*}
$$

From this we get the relations

$$ a = \frac{r_p + r_a}{2}\,, \qquad \qquad e = \frac{r_a - r_p}{r_a + r_p} $$

The semi-latus rectum $p$ of an ellipse is defined as the distance from the focus to the ellipse along a line perpendicular to the major axis. It is given by

$$ p = \frac{b^2}{a} = a (1 - e^2) $$

From this we get that the total energy and angular momentum of the orbit is

$$
\begin{align*}
\tag{3.2.1} \varepsilon &= -\frac{\mu}{2a}\\
\tag{3.2.2} h &= \sqrt{\mu a (1 - e^2)}
\end{align*}
$$

From hereon for all subsections except the last one, we consider the case when $m_2 \gg m_1$.

## Orbital Velocity

From eq 3.1.1, we have

$$ \frac{1}{2} v^2 - \frac{\mu}{r} = \varepsilon = -\frac{\mu}{2a} $$

$$\tag{3.2.3} \implies \boxed{v^2 = \mu \left( \frac{2}{r} - \frac{1}{a} \right)} $$

This is called the vis-viva equation. It gives the velocity of the smaller body at a distance $r$ from the larger body. The velocity is maximum at periapsis and minimum at apoapsis. The velocity at periapsis is given by

$$v_p = \sqrt{\mu \left( \frac{2}{r_p} - \frac{1}{a} \right)} = \sqrt{\frac{\mu}{a} \left( \frac{1+e}{1-e} \right)} $$

The velocity at apoapsis is given by

$$v_a = \sqrt{\mu \left( \frac{2}{r_a} - \frac{1}{a} \right)} = \sqrt{\frac{\mu}{a} \left( \frac{1-e}{1+e} \right)} $$

From this we get two relations:

$$ v_p v_a = \frac{\mu}{a}\,, \qquad \qquad \frac{v_p}{v_a} = \frac{1+e}{1-e} $$

In the case of a circular orbit, we have $e = 0$. The body therefore moves with a constant speed $v_c$, called the circular velocity, given by

$$\tag{3.2.4} v_c = \sqrt{\frac{\mu}{a}} $$

For the body to escape the gravitational influence of the larger body and become unbound, the total energy of the system must become more than or equal to 0. This can be achieved by increasing the velocity of the smaller body to a value equal to the escape velocity $v_e$, given by

$$\tag{3.2.5} v_e = \sqrt{\frac{2\mu}{r}} = \sqrt{2} v_c$$

From eq 3.1.8, the time period of the orbit is

$$ P = 2 \pi \sqrt{\frac{a^3}{\mu}} $$

## Kepler's Equation

Let the instant in time when the body was at periapsis be $t = \tau$. The mean motion $n$ is defined as

$$n = \frac{2 \pi}{P}$$

We define the mean anamoly $M$ as the angular distance from the periapsis which a fictitious body would have if it moved in a circular orbit, with constant speed, with the same orbital period as the actual body in its elliptical orbit. At any instant in time $t$, it is given by

$$\tag{3.2.6} M = n (t - \tau) $$

We defined the eccentric anamoly $E$ as the eccentric angle of the smaller body in its elliptical orbit. In cartesian coordinates with the center of the ellipse being at origin, the equation of the ellipse becomes

$$ \frac{x^2}{a^2} + \frac{y^2}{b^2} = 1 $$

The eccentric anamoly $E$ in terms of these coordinates is given by

$$ \cos E = \frac{x}{a}\,, \qquad \qquad \sin E = \frac{y}{b} $$

Moreover, we get that the distance of the smaller body from the larger body (foci of the ellipse) is given by

$$ r = a (1 - \cos E) $$

With this result, we can show that the true anomaly $\theta$ and the eccentric anamoly $E$ are related by

$$\tag{3.2.7} \tan \frac{\theta}{2} = \sqrt{\frac{1+e}{1-e}} \tan \frac{E}{2} $$

and

$$ \cos \theta = \frac{a}{r} (\cos E - e) \qquad \qquad \sin \theta = \frac{b}{r} \sin E $$

Using Kepler's second law, by finding the total area covered by the smaller body, presently at the eccentric angle $E$. Thus one obtains the relation between the mean anamoly $M$ and the eccentric anamoly $E$ as

$$\tag{3.2.8} M = E - e \sin E $$

This is called Kepler's equation. It is a transcendental equation, and can be solved using numerical methods.

It can be solved exactly in terms of an infinite series expansion, given by

$$ E = M + e \sin M + \frac{e^2}{2} \sin 2M + \frac{e^3}{6} \sin 3M + \ldots $$

The true anamoly and distance from focus too can be obtained in terms of infinite series expansion, given by

$$
\begin{align*}
\theta &= M + {2e \sin M} + \frac{5e^2}{4} \sin 2M + \frac{e^3}{12} (12 \sin 3M - 3 \sin M) + \ldots\\
\frac{r}{a} &= 1 - e\cos M + \frac{e^2}{2} (1 - \cos 2M) + \frac{3e^3}{8} (\cos M - \cos 3M) + \ldots
\end{align*}
$$

## Radial Elliptic trajectory

A radial elliptic trajectory is a degenerate case of an elliptical trajectory, where the eccentricity $e$ is equal to 1 and the angular momentum of the system is zero. The trajectory is a straight line, and the two bodies collide with each other at some point in the trajectory. It is still classified as an elliptic trajectory since the total energy of the system is negative.

## Binary Systems

Consider a binary system having two bodies of masses $m_1$ and $m_2$ moving in bound orbits. Both the bodies move in ellipses of equal eccentricities but oriented opposite to each other. Properties of orbits of individual bodies will be labelled with a subscript (e.g. $x_1$ and $x_2$), and properties of the trajectory of the separation vector, or the orbit of one of the bodies relative to the other will be written without a subscript (e.g. $x$).

The semi-major axes $a$ are related by the center of mass relation,

$$\tag{3.2.9} m_1 a_1 = m_2 a_2 = ma \implies a = a_1 + a_2 $$

Similarily, in the center of mass frame, the speeds $v$ are related by

$$\tag{3.2.10} m_1 v_1 = m_2 v_2 = m v \implies v = v_1 + v_2$$

When an elliptical orbit is projected onto a plane, it produces another ellipse. However, the foci of the original ellipse does not project onto the foci of the observed ellipse.

Consider a binary system at a distance $r$ from us, inclined at an angle $i$, which is the angle between the plane of the orbit and plane of the sky. $\alpha$ and $\tilde{\alpha}$ be the true and observed angular semi-major axes. They are related by the equations

$$ m_1 \alpha_1 = m_2 \alpha_2 = m \alpha \implies \alpha = \alpha_1 + \alpha_2$$
$$ m_1 \tilde{\alpha}_1 = m_2 \tilde{\alpha}_2 = m \tilde{\alpha} \implies \tilde{\alpha} = \tilde{\alpha_1} + \tilde{\alpha_2} $$
$$\tag{3.2.11} \tilde{\alpha} = \alpha \cos i $$

The true semi-major axis $a$ is given by

$$a = r \alpha = r \tilde{\alpha} \cos i$$

Hence Kepler's third law can be written as

$$\tag{3.2.12} m_1 + m_2 = \frac{4\pi^2}{G} \frac{a^3}{P^2} = \frac{4\pi^2}{G} \left( \frac{r}{\cos i} \right)^3 \frac{\tilde{\alpha}^3}{P^2}$$

Usually, for a binary system, only the radial velocity of the bodies can be measured. If the trajectory of the binary system is circular, the radial velocity is given by $v = \frac{2 \pi a}{T}$. The maximum radial velocity observed is $v_r = v \sin i$

$$ a = a_1 + a_2 = \frac{P}{2 \pi} (v_1 + v_2) = \frac{P}{2 \pi \sin i} (v_{1r} + v_{2r}) $$
$$\tag{3.2.13} \implies m_1 + m_2 = \frac{P}{2 \pi G} \frac{(v_{1r} + v_{2r})^3}{\sin^3 i} $$

If only one velocity ($v_{1r}$) is observable, $v_{2r}$ can be obtained using $m_1 v_{1r} = m_2 v_{2r}$. Putting this into the equation above, we get

$$\tag{3.2.14} \boxed{ \frac{m_2^3}{(m_1 + m_2)^2} \sin^3 i = \frac{P}{2 \pi G} v_{1r}^3 } $$

This is the mass function of the binary system. The mass function can be used to determine the mass of the secondary body if the mass of the primary body is known. The mass function can also be used to determine the inclination of the orbit if the masses of both bodies are known. It also sets a lower limit on the mass of $m_2$:

$$\tag{3.2.15} m_2 \geq \frac{P}{2 \pi G} v_{1r}^3 $$

## Problems

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    $\text{(IOAA 2007)}$ A Sun-orbiting periodic comet is the farthest at $31.5 \mathrm{\,AU}$ and the closest at $0.5 \mathrm{\,AU}$. What is the orbital period of this comet? What is the area (in $\mathrm{AU^2/yr}$) swept by the line joining the comet and the Sun?
    {{< /tab >}}

    {{< tab >}}
    The semi-major axis of the orbit is

    $$a = \frac{r_p + r_a}{2} = 16 \mathrm{\,AU}$$

    Using Kepler's third law, we have

    $$P^2 = a^3 = 16^3 = 4096 \implies \boxed{P = 64 \mathrm{\,years}}$$

    The eccentricity and semi-latus rectum can be found using

    $$e = \frac{r_a - r_p}{r_a + r_p} = \frac{31.5 - 0.5}{31.5 + 0.5} = \frac{31}{32}$$

    $$p = a(1 - e^2) = 16 \left( 1 - \frac{31^2}{32^2} \right) = 16 \left( \frac{63}{1024} \right) = 0.98 \mathrm{\,AU}$$

    Therefore the rate of area swept is

    $$\frac{dA}{dt} = \frac{h}{2} = \frac{\sqrt{\mu p}}{2} = \frac{\sqrt{4 \pi^2 p}}{2} = \pi \sqrt{p} = \pi \cdot \sqrt{0.98} = \boxed{3.1 \mathrm{\, AU^2/yr}}$$
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    $\text{(IOAA 2009)}$ Estimate the radius of a planet that a man can escape its gravitation by jumping vertically. Assume density of the planet and the Earth are the same.
    {{< /tab >}}

    {{< tab >}}
    A man can jump to a height $h \approx 50 \mathrm{\,cm}$ on Earth. This gives the man's jump velocity to be $v_\text{jump} = \sqrt{2g_\oplus h}$. Equating it to the escape velocity of the planet, we get

    $$\sqrt{2g_\oplus h} = \sqrt{\frac{2GM}{R}} \implies \sqrt{2\frac{G}{R_\oplus^2} \frac{4 \pi \rho_\oplus R_\oplus^3}{3} h} = \sqrt{\frac{2G}{R} \frac{4 \pi \rho R^3}{3}}$$

    Since $\rho = \rho_\oplus$, we have

    $$ R = \sqrt{R_\oplus h} \approx \boxed{1.79 \times 10^3 \mathrm{\,m}}  $$
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    A projectile which starts from the surface of the Earth at the sea level is launched with the initial speed of $v_0 < \sqrt{\frac{2GM_\oplus}{R_\oplus}}$ and the projecting angle (with respect to the local horizon) of $\theta$. Ignore the air resistance.
    1. The orbit of the projectile is an ellipse. Find its semi-major axis $a$ in units of $R_\oplus$.
    2. Calculate the highest altitude of the projectile with respect to the Earth surface (in units of $R_\oplus$)
    3. Find the time of filght for the projectile.
    4. What is the range of the projectile (surface distance between launching point and falling point) in the units of $R_\oplus$?
    5. What is the eccentricity $e$ of this elliptical orbit?
    {{< /tab >}}

    {{< tab >}}
    Coming Soon
    {{< /tab >}}
{{< /tabs >}}
