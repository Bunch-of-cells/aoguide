---
title: Unbound Orbits
weight: 3
---

As proved in section 3.1, hyperbolic and parabolic trajectories having total energy greater than or equal to zero are unbound.

## Parabolic trajectory

A parabola is a conic section with eccentricity equal to 1. The vertex point is the point of closest approach and is closest to the focus. If the distance to the focus from the vertex of the parabola is $r_p = a$, the length of the semi-latus rectum is $p = 2a$. The equation of the parabolic trajectory is

$$r = \frac{2a}{1 + \cos \theta}$$

The angular momentum of such a trajectory is $h = \sqrt{2 \mu a}$. The total energy of a parabolic trajectory is zero. Therefore the velocity at any point, at a distance $r$ from the focus, is equal to the escape velocity

$$v = \sqrt{\frac{2\mu}{r}}$$

The velocity at the point of closest approach is

$$v_p = \sqrt{\frac{2\mu}{r_p}} = \sqrt{\frac{2\mu}{a}}$$

## Hyperbolic trajectory

A hyperbola is a conic section with eccentricity greater than 1. The vertex point is the point of closest approach and is closest to the focus. Let the semi-major axis of the hyperbola be $a$. By convention, it is defined to be a negative quantity. This is done so that the equations match with those of an elliptical orbit. The distance of vertex from focus is

$$ r_p = (-a) (e - 1) = a(1-e) $$

The semi-latus rectum is

$$ p = (-a)(e^2 - 1) = a(1 - e^2) $$

The equation of the hyperbolic trajectory is

$$ r = \frac{a(1-e^2)}{1 + e \cos \theta} $$

We see that the true anamoly can only take values between $-\cos^{-1} \left(\frac{-1}{e}\right)$ and $\cos^{-1} \left(\frac{-1}{e}\right)$.

The angular momentum of the system is $h = \sqrt{\mu a (1 - e^)}$, and the total energy is given by $\varepsilon = -\frac{\mu}{2a}$. Note that the energy is positive, due to $a$ being negative. The velocity of the body at a distance $r$ from the focus is given by

$$v^2 = \mu \left( \frac{2}{r} + \frac{1}{a} \right)$$

The velocity at the point of closest approach is

$$v_p = \sqrt{\mu \left( \frac{2}{r_p} + \frac{1}{a} \right)} = \sqrt{\frac{\mu}{a} \left( \frac{1+e}{1-e} \right)}$$

The velocity at infinity is

$$v_\infty = \sqrt{\frac{\mu}{a} \left( \frac{1-e}{1+e} \right)}$$

## Variants of Kepler's Equation

In a parabolic trajectory, Barker's equation relates the time of flight $t$ to the true anamoly $\theta$. If the time of periapsis is $\tau$, then

$$t - \tau = \sqrt{\frac{2a^3}{\mu}} \left( \tan \frac{\theta}{2} + \frac{1}{3} \tan^3 \frac{\theta}{2} \right)$$

In a hyperbolic trajectory, the hyperbolic Kepler's equation relates the mean anamoly $M$ to the hyperbolic anamoly $H$:

$$M = e \sinh H - H$$

where the mean anamoly is defined as $M = \sqrt{\frac{\mu}{-a^3}} (t - \tau)$. The true anamoly and hyperbolic anamoly are related by

$$\tan \frac{\theta}{2} = \sqrt{\frac{e + 1}{e - 1}} \tanh \frac{H}{2}$$

## Radial trajectories

A radial parabolic trajectory is a degenerate case of an parabolic trajectory, where the eccentricity $e$ is still equal to 1, however the angular momentum of the system is zero. The trajectory is a straight line, and the two bodies move away from each other, the velocity tending to zero as they get infinity far away from each other. It is classified as an parabolic trajectory since the total energy of the system is zero.

A radial hyperbolic trajectory is a degenerate case of an hyperbolic trajectory, where the eccentricity $e$ is equal to 1 and the angular momentum of the system is zero. The trajectory is a straight line, and the two bodies move away from each other, having a finite velocity at infinity. It is classified as an hyperbolic trajectory since the total energy of the system is positive.
