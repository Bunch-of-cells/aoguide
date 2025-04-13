---
title: Orbital Maneuvers
weight: 6
---

## Delta-v

Delta-v ($\Delta v$) is a measure of the impulse per unit of spacecraft mass that is needed to perform a maneuver. It is a scalar that has the units of speed. In the abscence of external forces, the Delta-v is equal to the change in velocity of the spacecraft.

$$\tag{3.6.1} \Delta v = \int_{t_0}^{t_1} |\dot{v}| dt $$

where $\dot{v}$ is the acceleration. When the thrust force is applied in a constant direction, Delta-v is given by $\Delta v = |v_1 - v_0|$ is simply the magnitude of the change in velocity. For multiple maneuvers, Delta-v sums linearly.

Orbit maneuvers are made by firing a thruster to produce a reaction force acting on the spacecraft. The size of this force will be

$$\tag{3.6.2} T = v_\text{exh} \, \rho $$

where

- $v_\text{exh}$ s the velocity of the exhaust gas in rocket frame
- $\rho$ is the mass flow rate of the propellant

If the mass of the satellite at $t=t_0$ before the maneuver is $m_0$, and at $t=t_1$ after the maneuver is $m_1$, then the Delta-v is given by the Tsiolkovsky rocket equation

$$\tag{3.6.3} \boxed{\Delta v = v_\text{exh} \ln \left( \frac{m_0}{m_1} \right)} $$

Thus the amount of propellant required for the maneuver is $m_1 - m_0$.

When applying Delta-v in the direction of the velocity the specific orbital energy gained per unit Delta-v is equal to the instantaneous speed. This is called the Oberth effect. For example, a satellite in an elliptical orbit is boosted more efficiently at high speed (at perigee) than at low speed (at apogee). Another example is that when a vehicle is making a pass of a planet, burning the propellant at closest approach rather than further out gives significantly higher final speed, and this is even more so when the planet is a large one with a deep gravity field, such as Jupiter.

## Hohmann Tranfer Orbital Maneuver

The Hohmann transfer orbit is an orbital maneuver used to transfer a spacecraft between two orbits of different altitudes around a central body. The initial and target orbits are both circular and coplanar. The maneuver is accomplished by placing the craft into an elliptical transfer orbit that is tangential to both the initial and target orbits. The maneuver uses two impulsive engine burns: the first establishes the transfer orbit, and the second adjusts the orbit to match the target. The Hohmann maneuver often uses the lowest possible amount of impulse (which consumes a proportional amount of delta-v, and hence propellant).

### Transfer between circular coplanar orbits

Consider an orbital transfer from orbit 1, having radius $a_1$ to orbit 2, having radius $a_2$, via an elliptical orbit whose periapsis is in orbit 1 and apoapsis in orbit 2. Such transfer orbits are known as Hohmann least energy two-impulse cotangential orbits. The first impulse is applied at periapsis, and the second at apoapsis.

The semi-major axis of the transfer orbit is

$$\tag{3.6.4} a_t = \frac{a_1 + a_2}{2} $$

The eccentricity of the transfer orbit is

$$\tag{3.6.5} e_t = \frac{a_2 - a_1}{a_2 + a_1} $$

The transfer time is half the period of the transfer orbit, which is given by

$$\tag{3.6.6} T_t = \pi \sqrt{\frac{a_t^3}{\mu}} $$

If we work in the units of AU, years and solar masses, $T_t = \sqrt{\frac{(a_1 + a_2)^3}{32M}}$.

The velocity at periapsis of the transfer orbit is greater than the velocity of the initial orbit, and the velocity at apoapsis of the transfer orbit is less than the velocity of the final orbit. The change in velocity at periapsis is given by

$$\tag{3.6.7} \Delta v_1 = v_\text{p,t} - v_1 = \sqrt{\frac{\mu}{a_t} \left( \frac{1 + e}{1 - e} \right) } - \sqrt{\frac{\mu}{a_1}} $$

The change in velocity at apoapsis is given by

$$\tag{3.6.8} \Delta v_2 = v_2 - v_\text{a,t} = \sqrt{\frac{\mu}{a_2}} - \sqrt{\frac{\mu}{a_t} \left( \frac{1 - e}{1 + e} \right) } $$

The total Delta-v for the maneuver is

$$\tag{3.6.9} \Delta v = \sqrt{\frac{\mu}{a_t (1 - e_t^2)}} \, (2e_t + \sqrt{1 - e_t} - \sqrt{1 + e_t})$$

### Coplanar rendezvous transfer

The Hohmann transfer orbit can be used to rendezvous with another spacecraft in a co-planar orbit. Let's say we have a interceptor satellite which has to be maneuvered to rendezvous with a target satellite. The interceptor is in a circular orbit of radius $a_1$, and the target is in a circular orbit of radius $a_2$. Both orbit in the same direction. The interceptor will perform a Hohmann transfer to reach the target orbit, and then it will perform a second maneuver to match the velocity of the target. The properties of the orbits are the same as in the previous section. The only difference is that the target is moving in its orbit, and the interceptor has to catch up to it, at just the right time.

A launch window is a time period during which the interceptor can be launched to reach the target. The launch window is determined by the relative positions of the two satellites in their orbits. The launch window is open when the interceptor is at periapsis, and the target is at apoapsis.

Let's assume that the interceptor and target are in just the right configuration for the rendezvous maneuver. The lead angle $\alpha_\text{lead}$ is the angle between the initial position of the target and the (future) rendezvous point.

$$\tag{3.6.10} \alpha_\text{lead} = \omega_\text{target} \cdot T_t $$

where $\omega_\text{target}$ is the angular velocity of the target, and $T_t$ is the time it takes for the interceptor to reach the target orbit. The phase angle $\phi$ is the angle between the interceptor and the target at any instant. It is measured from the interceptor to the target, in the direction of motion. At the start of the maneuver, the phase angle is given by

$$\tag{3.6.11} \phi_0 = \pi - \alpha_\text{lead} $$

After the maneuver, obviously, the phase angle is zero.

If the interceptor and target are not in the correct configuration, the interceptor will have to wait for the next launch window. Say the phase angle at this moment is $\phi$. The wait time $T_w$ is given by

$$\tag{3.6.12} 2n\pi + \phi_0 - \phi = (\omega_\text{target} - \omega_\text{interceptor}) \cdot T_w $$

where $n$ is a non-negative integer.

## Bi-elliptic Transfer

The Bi-elliptic transfer is an orbital maneuver that moves a spacecraft from one orbit to another and may, in certain situations, require less delta-v than a Hohmann transfer maneuver. The bi-elliptic transfer consists of two half-elliptic orbits. From the initial orbit, a first burn expends delta-v to boost the spacecraft into the first transfer orbit with an apoapsis at some point $r_b$ away from the central body. At this point a second burn sends the spacecraft into the second elliptical orbit with periapsis at the radius of the final desired orbit, where a third burn is performed, injecting the spacecraft into the desired orbit.

## Gravity assists

A spacecraft when launched from Earth, has to first leave Earth's hill sphere. After that it enters the interplanetary space with some geocentric velocity, which together with Earth's orbital velocity puts it into a heliocentric orbit to, say, Mars. During the transfer, it will be perturbed slightly by the Earth. As it enters Martian hill sphere, it is said to be solar perturbed about that planet. Its subsequent solar orbit will be quite different from its pre-Martian encounter orbit.

Planetary flypasts have the ability to change the energy of small bodies, and give it an entirely different heliocentric orbit. A gravity assist is a maneuver that uses the gravitational field of a planet or moon to change the speed and direction of a spacecraft. The spacecraft approaches the planet or moon, and as it passes close to the body, it is accelerated by the gravitational field. The spacecraft then moves away from the body, having gained speed and changed direction. Gravity assists are often used to increase the speed of a spacecraft, allowing it to reach its destination more quickly or to save fuel.

Let a spacecraft having a velocity $v$ relative to the sun, approach Jupiter. From Jupiter's frame, the spacecraft has a velocity of $v_J - v$. The velocity after the slingshot, from Jupiter's frame is the same, $v_J - v$, but its direction has changed. However, from a heliocentric frame, the velocity is $v_J + (v_J - v) = 2v_J - v > v$. The spacecraft has gained a velocity of $2(v_J - v)$ in the heliocentric frame.
