---
title: Orbital Elements
weight: 4
---

<figure class="ma0 w-75">
  <img src="/images/orbital-elements.svg" alt="Orbital Elements" />
  <figcaption>Orbital Elements (source: Wikipedia)</figcaption>
</figure>

Orbital elements are the parameters required to uniquely identify a specific orbit. When viewed from an inertial frame, two orbiting bodies trace out distinct trajectories. Each of these trajectories has its focus at the common center of mass. When viewed from a non-inertial frame centered on one of the bodies, only the trajectory of the opposite body is apparent; Keplerian elements describe these non-inertial trajectories. In general, six parameters are used to describe the orbit.

Two parameter are required to describe the size and shape of the orbit. These are:

- Semi-major axis $a$: half the distance between the apoapsis and periapsis (long axis of the ellipse). This value is positive for elliptical orbits, infinity for parabolic trajectories, and negative for hyperbolic trajectories, which can hinder its usability when working with different types of trajectories.
- Eccentricity $e$: shape of the ellipse, describing how much it deviates from a perfect a circle. An eccentricity of zero describes a perfect circle, values less than 1 describe an ellipse, values greater than 1 describe a hyperbolic trajectory, and a value of exactly 1 describes a parabola.

Three parameters are required to descrive the orientation of the orbit. These are:

- Inclination $i$: vertical tilt of the ellipse with respect to the reference plane, measured at the ascending node. Inclinations from $90^\circ$ to $180^\circ$ are typically used to denote retrograde orbits.
- Longitude of the ascending node $\Omega$: describes the angle from the ascending node of the orbit (☊ in the diagram) to the reference frame's reference direction (♈︎ in the diagram). This is measured in the reference plane. This quantity is undefined for perfectly coplanar orbits, but is often set to zero instead by convention.
- Argument of periapsis $\omega$: defines the orientation of the ellipse in the orbital plane, as an angle measured from the ascending node to the periapsis. This quantity is undefined for circular orbits, but is often set to zero instead by convention.

Another element commonly used is

- Longitude of periapsis $\varpi$: describes the angle between the reference direction (♈︎) and the periapsis, measured partly in the reference plane and partly in the orbital plane. It is defined as $\varpi =\Omega +\omega$. Unlike the longitude of the ascending node, this value is defined for orbits where the inclination is zero.

One elements are needed to describe the position of the body around its orbit, and the time at which this occurs. These are:

- Time of periapsis $\tau$:  time at which the orbiting body is at periapsis. This value is not defined for circular orbits, as they do not have a uniquely defined point of periapsis.

Another element commonly used is

- Mean Longitude $\bar{\lambda}$: Mean longitude is similar to mean anomaly, in that it increases linearly with time and does not represent the real angular displacement. Unlike with mean anomaly, mean longitude is defined relative to the vernal point, which means it is defined for circular orbits. $\bar{\lambda} = \varpi + M$

## Eulerian Angles

<figure class="ma0 w-75">
  <img src="/images/euler-angles.svg" alt="Euler angles" />
  <figcaption>Euler Angles</figcaption>
</figure>

The Euler angles are three angles used to describe the orientation of a coordinate system with respect to another fixed coordinate system. The angles $\Omega$, $i$, $\omega$ are the Euler angles characterizing the orientation of the coordinate system. Let ${\mathbf{\hat{X}}}$, $\mathbf{\hat{Y}}$ and $\mathbf{\hat{Z}}$ define the coordinate system of the reference plane, and ${\mathbf{\hat{x}}}$, $\mathbf{\hat{y}}$ and $\mathbf{\hat{z}}$ define the coordinate system of the orbital plane. N in the figure denotes the direction of the ascending node.

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
0 & \cos I & -\sin I \\
0 & \sin I & \cos I
\end{bmatrix}
\begin{bmatrix}
\cos\omega & -\sin\omega & 0 \\
\sin\omega & \cos\omega & 0 \\
0 & 0 & 1
\end{bmatrix}
\begin{bmatrix} x \\ y \\ z \end{bmatrix}
$$

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
0 & \cos I & \sin I \\
0 & -\sin I & \cos I
\end{bmatrix}
\begin{bmatrix}
\cos\omega & \sin\omega & 0 \\
-\sin\omega & \cos\omega & 0 \\
0 & 0 & 1
\end{bmatrix}
\begin{bmatrix} X \\ Y \\ Z \end{bmatrix}
$$

If the orbiting body is at a distance $r$, having true anamoly $\theta$, its coordinates are $x = r \cos \theta$, $y = r \sin \theta$ and $z = 0$. Therefore, the coordinates of the orbiting body in the reference frame are given by

$$
\begin{align*}
X &= r \left( \cos\Omega \cos(\omega + \theta) - \sin\Omega \sin(\omega + \theta) \cos I \right) \\
Y &= r \left( \sin\Omega \cos(\omega + \theta) + \cos\Omega \sin(\omega + \theta) \cos I \right) \\
Z &= r \sin(\omega + \theta) \sin I
\end{align*}
$$

If the reference frame is the ecliplic, the (heliocentric) ecliptic coordinates of the orbiting body are given by

$$ \tan \lambda = \frac{Y}{X}\,, \qquad \qquad \sin \beta = \frac{Z}{\sqrt{X^2 + Y^2}} $$

## Problems

- [NAC 2023, Long Questions, 2](https://usaaao.org/wp-content/uploads/2023/09/second_exam_2023-1.pdf)

{{< tabs items="Problem,Hint,Solution" >}}
    {{< tab >}}
    Assume that at this exact moment a satellite in circular heliocentric orbit is in a solar transit.
    1. Find the distance of the satellite from earth 65 days later.
    2. Find the equatorial coordinates of this satellite 140 days later.

    You are given that the orbital inclination of the satellite is $20^\circ$, orbital radius is $0.6 \mathrm{\, AU}$, longitude of ascending node is $130^\circ$ and inclination of the ecliptic relative to the equator is $23.5^\circ$. Assume the orbit of Earth to be circular.
    {{< /tab >}}

    {{< tab >}} 
    Coming Soon!
    {{< /tab >}}

    {{< tab >}}
    Coming Soon!
    {{< /tab >}}
{{< /tabs >}}
