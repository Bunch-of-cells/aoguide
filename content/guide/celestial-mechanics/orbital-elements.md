---
title: Orbital Elements
weight: 4
---

{{< svg "images/orbital-elements.svg" "Orbital elements illustration" "Orbital Elements (source: Wikipedia)" >}}

First of all, we define the following

- Reference plane: plane used as a reference to define orbital elements. The reference plane is typically taken to be the ecliptic or the equator.
- Reference direction (♈︎): direction in the reference plane used to define the orbital elements. The reference direction is typically taken to be the vernal equinox.
- Node: intersection of the orbiting body's orbital plane with the reference plane.
- Ascending node (☊): point at which the orbiting body crosses the reference plane from below to above.
- Descending node (☋): point at which the orbiting body crosses the reference plane from above to below.
- Periapsis (☉): point at which the orbiting body is closest to the focus of the ellipse. If the primary body is the Sun, this point is called perihelion (☉). If the primary body is Earth, this point is called perigee (☉). If the primary body is the Moon, this point is called perilune (☉).
- Apoapsis (☽): point at which the orbiting body is farthest from the focus of the ellipse. If the primary body is the Sun, this point is called aphelion (☽). If the primary body is Earth, this point is called apogee (☽). If the primary body is the Moon, this point is called apolune (☽).

Orbital elements are the parameters required to uniquely identify a specific orbit. When viewed from an inertial frame, two orbiting bodies trace out distinct trajectories. Each of these trajectories has its focus at the common center of mass. When viewed from a non-inertial frame centered on one of the bodies, only the trajectory of the opposite body is apparent; Keplerian elements describe these non-inertial trajectories. In general, six parameters are used to describe the orbit.

Two parameter are required to describe the size and shape of the orbit. These are:

- Semi-major axis $a$: half the distance between the apoapsis and periapsis (long axis of the ellipse). This value is positive for elliptical orbits, infinity for parabolic trajectories, and negative for hyperbolic trajectories, which can hinder its usability when working with different types of trajectories.
- Eccentricity $e$: shape of the ellipse, describing how much it deviates from a perfect a circle. An eccentricity of zero describes a perfect circle, values less than 1 describe an ellipse, values greater than 1 describe a hyperbolic trajectory, and a value of exactly 1 describes a parabola.

Three parameters are required to descrive the orientation of the orbit. These are:

- Inclination $i$: vertical tilt of the ellipse with respect to the reference plane, measured at the ascending node. Inclinations from $90^\circ$ to $180^\circ$ are typically used to denote retrograde orbits.
- Longitude of the ascending node $\Omega$: describes the angle from the ascending node of the orbit (☊ in the diagram) to the reference frame's reference direction (♈︎ in the diagram). This is measured in the reference plane. This quantity is undefined for perfectly coplanar orbits, but is often set to zero instead by convention.
- Argument of periapsis $\omega$: defines the orientation of the ellipse in the orbital plane, as an angle measured from the ascending node to the periapsis. This quantity is undefined for circular orbits, but is often set to zero instead by convention.

Another parameter commonly used is

- Longitude of periapsis $\varpi$: describes the angle between the reference direction (♈︎) and the periapsis, measured partly in the reference plane and partly in the orbital plane. It is defined as $\varpi =\Omega +\omega$. Unlike the longitude of the ascending node, this value is defined for orbits where the inclination is zero.

One parameter are needed to describe the position of the body around its orbit, and the time at which this occurs. These are:

- Time of periapsis $\tau$:  time at which the orbiting body is at periapsis. This value is not defined for circular orbits, as they do not have a uniquely defined point of periapsis.

Another parameter commonly used is

- Mean Longitude $\bar{\lambda}$: Mean longitude is similar to mean anomaly, in that it increases linearly with time and does not represent the real angular displacement. Unlike with mean anomaly, mean longitude is defined relative to the vernal point, which means it is defined for circular orbits. $\bar{\lambda} = \varpi + M$

## Eulerian Angles

{{< svg "images/euler-angles.svg" "Euler angle illustration" "Euler Angles" >}}

The Euler angles are three angles used to describe the orientation of a coordinate system with respect to another fixed coordinate system. The angles $\Omega$, $i$, $\omega$ are the Euler angles characterizing the orientation of the coordinate system. Let ${\hat{\mathbf{X}}}$, $\hat{\mathbf{Y}}$ and $\hat{\mathbf{Z}}$ define the coordinate system of the reference plane, and ${\hat{\mathbf{x}}}$, $\hat{\mathbf{y}}$ and $\hat{\mathbf{z}}$ define the coordinate system of the orbital plane. N in the figure denotes the direction of the ascending node, while X is the reference direction.

The transformation between the two coordinate systems is given by the following equations:

$$
\begin{bmatrix} X \\ Y \\ Z \end{bmatrix} =
\begin{bmatrix}
\cos\Omega & -\sin\Omega & 0 \\
\sin\Omega & \cos\Omega & 0 \\
0 & 0 & 1
\end{bmatrix}
\begin{bmatrix}
1 & 0 & 0 \\
0 & \cos i & -\sin i \\
0 & \sin i & \cos i
\end{bmatrix}
\begin{bmatrix}
\cos\omega & -\sin\omega & 0 \\
\sin\omega & \cos\omega & 0 \\
0 & 0 & 1
\end{bmatrix}
\begin{bmatrix} x \\ y \\ z \end{bmatrix}
$$

$$\tag{3.4.1}$$ <br />

and

$$
\begin{bmatrix} x \\ y \\ z \end{bmatrix} =
\begin{bmatrix}
\cos\Omega & \sin\Omega & 0 \\
-\sin\Omega & \cos\Omega & 0 \\
0 & 0 & 1
\end{bmatrix}
\begin{bmatrix}
1 & 0 & 0 \\
0 & \cos i & \sin i \\
0 & -\sin i & \cos i
\end{bmatrix}
\begin{bmatrix}
\cos\omega & \sin\omega & 0 \\
-\sin\omega & \cos\omega & 0 \\
0 & 0 & 1
\end{bmatrix}
\begin{bmatrix} X \\ Y \\ Z \end{bmatrix}
$$

$$\tag{3.4.2}$$  <br />

If the orbiting body is at a distance $r$, having true anamoly $\theta$, its coordinates are $x = r \cos \theta$, $y = r \sin \theta$ and $z = 0$. Therefore, the coordinates of the orbiting body in the reference frame are given by

$$
\begin{align}
\tag{3.4.3} X &= r \left( \cos\Omega \cos(\omega + \theta) - \sin\Omega \sin(\omega + \theta) \cos i \right) \\
\tag{3.4.4} Y &= r \left( \sin\Omega \cos(\omega + \theta) + \cos\Omega \sin(\omega + \theta) \cos i \right) \\
\tag{3.4.5} Z &= r \sin(\omega + \theta) \sin i
\end{align}
$$

If the reference frame is the ecliplic, the (heliocentric) ecliptic coordinates of the orbiting body are given by

$$\tag{3.4.6} \tan \lambda = \frac{Y}{X}\,, \qquad \qquad \sin \beta = \frac{Z}{\sqrt{X^2 + Y^2}} $$

## Problems

{{< tabs items="Problem,Solution" >}}
    {{< tab >}}
    [NAC 2023, Long Questions, 2](https://usaaao.org/wp-content/uploads/2023/09/second_exam_2023-1.pdf)
    {{< /tab >}}

    {{< tab >}} 
    [Solution](https://usaaao.org/wp-content/uploads/2023/09/second_exam_2023_sols-1.pdf)
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="Problem,Hint,Solution" >}}
    {{< tab >}}
    Assume that at this exact moment a satellite in circular heliocentric orbit is in a solar transit.
    1. Find the distance of the satellite from earth 65 days later.
    2. Find the equatorial coordinates of this satellite 140 days later.

    You are given that the orbital inclination of the satellite is $20^\circ$, orbital radius is $0.6 \mathrm{\, AU}$, longitude of ascending node is $130^\circ$ and inclination of the ecliptic relative to the equator is $23.5^\circ$. Assume the orbit of Earth to be circular.
    {{< /tab >}}

    {{< tab >}} 
    Use equations 3.4.3 to 3.4.5 to find the cartesian coordinates of the satellite at a later time. Use the 3D distance formula to find the distance from Earth, and eq 3.4.6 to find the ecliptic coordinates, which can be converted to equatorial coordinates.
    {{< /tab >}}

    {{< tab >}}
    We are given that

    - $a = 0.6 \mathrm{\, AU}$
    - $i = 20^\circ$
    - $\Omega = 130^\circ$

    Note that since there is no periapsis (the orbit is circular), we can't determine $\omega$. Instead, we use the ascending node as a reference point, and set $\omega = M = \tau = 0$ there. The orbital period of the satellite is $P = a^{3/2} = 0.465 \mathrm{\,yr}$, which gives the mean motion $n = 0.03701 \mathrm{\,day^{-1}}$. Writing eqn 3.4.3 to 3.4.5 at a later time when the mean anamoly (which is equal to the true anamoly) is $M$,

    $$
    \begin{aligned}
    X &= r \left( \cos\Omega \cos M - \sin\Omega \sin M \cos i \right) \\
    Y &= r \left( \sin\Omega \cos M + \cos\Omega \sin M \cos i \right) \\
    Z &= r \sin M \sin i
    \end{aligned}
    $$

    1. The position of Earth at the same time is given by

    $$
    \begin{aligned}
    X_\oplus &= a \cos (M + \Omega) \\
    Y_\oplus &= a \sin (M + \Omega) \\
    Z_\oplus &= 0
    \end{aligned}
    $$

    where a = $1 \mathrm{\,AU}$.

    At $t = 65 \mathrm{\,days}$, $M = nt = 2.406 = 137.8^\circ$. Putting this into the equations, we get

    $$
    \begin{aligned}
    X &= -0.004 \mathrm{\, AU} \\
    Y &= -0.584 \mathrm{\, AU} \\
    Z &= 0.138 \mathrm{\, AU}
    \end{aligned}
    $$

    $$
    \begin{aligned}
    X_\oplus &= -0.038 \mathrm{\, AU} \\
    Y_\oplus &= -0.999 \mathrm{\, AU} \\
    Z_\oplus &= 0
    \end{aligned}
    $$

    The distance between Earth and the satellite is, therefore,

    $$d = \sqrt{(X - X_\oplus)^2 + (Y - Y_\oplus)^2 + (Z - Z_\oplus)^2} = \boxed{0.439 \mathrm{\, AU}}$$

    2. The mean anamoly after 140 days is $M = nt = 5.182 = 296.9^\circ$. The position of the satellite at this time is given by

    $$
    \begin{aligned}
    X &= 0.211 \mathrm{\, AU} \\
    Y &= 0.531 \mathrm{\, AU} \\
    Z &= -0.183 \mathrm{\, AU}
    \end{aligned}
    $$

    Now, using eq 3.4.6, we can find the ecliptic coordinates of the satellite.

    $$
    \begin{aligned}
    \tan \lambda &= \frac{Y}{X} = 2.517 \implies \lambda = 68.3^\circ \\
    \sin \beta &= \frac{Z}{\sqrt{X^2 + Y^2}} = -0.320 \implies \beta = -18.7^\circ
    \end{aligned}
    $$

    To get the equatorial coordinates from this, we use the following equations

    $$
    \begin{aligned}
    \sin \alpha \cos \delta &= -\sin \beta \sin \epsilon + \cos \beta \cos \epsilon \sin \lambda \\
    \cos \alpha \cos \delta &= \cos \lambda \cos \beta \\
    \sin \delta &= \sin \beta \cos \epsilon + \cos \beta \sin \epsilon \sin \lambda
    \end{aligned}
    $$

    Substituing the values for $\beta$, $\lambda$ and $\epsilon$, we get

    $$\boxed{ \alpha = 69.46^\circ\,, \quad \delta = 3.26^\circ }$$

    {{< /tab >}}
{{< /tabs >}}
