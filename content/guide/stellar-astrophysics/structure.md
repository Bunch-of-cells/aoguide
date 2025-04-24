---
title: Stellar Structure
prev: /guide/stellar-astrophysics
weight: 1
---

Stars are huge spheres of gas. The gas in the stars are completely ionised. Hence to a good approximation, we can assume it to be an ideal gas

$$ P = \frac{k}{\mu m_H} \rho T$$

where $\mu$ is the mean molecular weight. Hydrogen when ionized gives rise to two particles ($\ce{H^+}$ and $\ce{e}$), per nucleon (single proton in Hydrogen). Helium gives $3/4$ particles per nucleon when ionized (3 particles from one atom, each atom has 4 nucleons). For other elements having atomic number $Z$, give rise to ~$1/2$ particles per nucleon when ionized. Let the relative mass fractions of Hydrogen, Helium and heavier elements (which are all called metals by astronomers) be $X$, $Y$ and $Z$ respectively. Then

$$ X + Y + Z = 1 $$

$$ \mu = \frac{1}{2X + \frac{3}{4}Y + \frac{1}{2} Z } $$

For our sun, $\mu_\odot \approx 0.6$.

A star can go on shining steadily for thousands of millions of years. Thus the equilibrium of a star must remain stable for such long periods. Mathematically the conditions for the internal equilibrium of a star can be expressed as four differential equations governing the distribution of mass, gas pressure and energy production and transport in the star.

## Mass Continuity

The second equation gives the mass contained within a given radius. Consider a spherical shell of thickness dr at the distance r from the centre. Its mass is

$$ dm = 4 \pi r^2 \rho dr $$

which gives the mass continuity equation

$$\tag{5.1.1} \boxed{ \frac{dm}{dr} = 4 \pi r^2 \rho } $$

## Energy Continuity

The third equilibrium condition expresses the conservation of energy, requiring that any energy produced in the star has to be carried to the surface and radiated away. Let $\varepsilon$ is the energy production coefficient, which is the amount of energy released in the star per unit time and mass. Let $l$ be the energy flux at radius $r$, then

$$\tag{5.1.2} \frac{dl}{dm} = \varepsilon $$

or

$$\tag{5.1.3} \boxed{\frac{dl}{dr} = 4\pi r^2 \rho \varepsilon} $$

If the mean free path of a photon in the star is $\lambda$, the probability of it getting absorbed in length $dr$ is $\frac{dr}{\lambda}$. Hence the change in flux is

$$\tag{5.1.4} dF = \frac{F}{\lambda} dr$$

The opacity is defined as

$$\tag{5.1.5} \kappa = \frac{1}{\rho \lambda} $$

## Hydrostatic Equillibrium

The force of gravity pulls the stellar material towards the centre. It is resisted by the pressure force due to the thermal motions of the gas molecules. The first equilibrium condition is that these forces be in equilibrium.

Consider a cylindrical volume element at the distance $r$ from the centre of the star. If the mass enclosed inside radius $r$ is $m$, the force of gravity on the element is

$$ dF_g = -\frac{Gm dm}{r^2} = -\frac{Gm \rho}{r^2}\,dA\,dr $$

If the pressure at the lower surface of the volume element is P and at its upper surface P +dP , the net force of pressure acting on the element is

$$ dF_p = -dP \, dA $$

Hence the equillibrium considtion becomes $dF_g + dF_p = 0$, or

$$\tag{5.1.6} \boxed{ \frac{dP}{dr} = - \frac{Gm \rho}{r^2}  = - g \rho } $$

or

$$\tag{5.1.7} \frac{dP}{dm} = - \frac{Gm}{4 \pi r^4} $$

### Central Pressure

The central pressure can be calculated as

$$ \int_0^S dP = \int_0^S - \frac{Gm \, dm}{4 \pi r^4} \gt \int_0^S - \frac{Gm \, dm}{4 \pi R^4} = -\frac{GM^2}{8 \pi R^4} $$

where $S$ represents the surface of the star, at $r= R$. Taking the pressure at surface to be zero, we get

$$\tag{5.1.8} P_c > \frac{GM^2}{8 \pi R^4} $$

If density is constant,

$$P_c = \frac{3GM^2}{8 \pi R^4}$$

### Virial Theorem

$$ \frac{dP}{dm} = -\frac{Gm}{4\pi r^4} \implies \int_0^S 4 \pi r^3 dP = \int_0^S -\frac{Gm \, dm}{r} = \Omega $$

where $\Omega$ is the total gravitational potential energy of the star. Now since $4 \pi r^3$ = $3V$, where $V$ is the volume of the sphere upto radius $r$, using integration by parts we get

$$ 3 \int_0^S V dP = 3 \left( VP |_0^S - \int_0^S P dV \right) = -3 \int_0^S P dV $$

Since at $r=0$ we have $V=0$and at $r=R$ we have $P =0$. Putting this back, we get the virial theorem

$$\tag{5.1.9} \boxed{ -3 \int_0^S P \, dV = \Omega } $$

Assuming an ideal gas star with an adiabatic index $\gamma$,

$$ u = \frac{E}{V} = \frac{n}{V} C_V R T = \frac{P}{\gamma - 1} \implies P = (\gamma - 1)u $$

$$\tag{5.1.10} \therefore \quad \boxed{\, 3 (\gamma - 1) U + \Omega = 0 \,} $$

where $U = \int_0^S u dV$ is the total internal energy of the gas.

The total energy of the star is

$$ E = U + \Omega \:= -(3\gamma - 4) \, U \:= \frac{3\gamma - 4}{3 \gamma - 3} \, \Omega $$

For a monoatomic gas, $\gamma = 5/3$, hence the total energy is $E = -U = \frac{1}{2} \Omega$.

As the total energy of a star increases, its gravitational potential energy increases (expands) and internal energy decreases (cools down). Hence, stars have negative heat capacity.

## Energy transport

The total energy flux consists of energy flux due to radiation, convection and conduction. In stars, conduction is very inefficient, hence convection and radiation are the only processes at play.

### Energy transport via radiation

The pressure due to radiation is

$$\tag{5.1.11} P_\text{rad} = \frac{1}{3}aT^4 $$

where $a = 4\sigma /c$ is the radiation constant.

The energy flux due to radiation is

$$ dF = d \left( \frac{1}{A} \frac{dE}{dt} \right) = d \left( \frac{1}{A} \frac{dp}{dt} c \right) = c \, dP_\text{rad}$$

Combining this with eq 5.1.4 and eq 5.1.11,

$$ F \, \frac{dr}{\lambda} = \frac{4}{3} \, ac T^3 \, dT $$

Since $F = \frac{l_\text{rad}}{4 \pi r^2}$, we get

$$\tag{5.1.12} \boxed{ \frac{dT}{dr} = -\frac{3}{4ac} \: \frac{\kappa \rho}{T^3} \frac{l_\text{rad}}{4 \pi r^2} } $$

or

$$\tag{5.1.13} \frac{dT}{dm} = -\frac{3}{64 \pi^2 ac} \: \frac{\kappa l_\text{rad}}{r^4 T^3}$$

### Energy transport via convection

To model convection, consider a small blob of gas in a star. Initially, it is in hydrostatic equillibrium with the surroundings ($P_b = P_g$, $\rho_b = \rho_g$). After is rises up, it expands adiabatically. If in the new position, the blob has a density $\rho_b + d\rho_b > \rho_g + d\rho_g$, the blob will sink back down and the gas is stable to convection. If $\rho_b + d\rho_b < \rho_g + d\rho_g$, the blob is buoyant and will continue to rise; this marks the onset of convection. Hence the condition for stability against convection is

$$ d\rho_b > d\rho_g $$

Given $\rho_b = \rho$ and $P_b = P$, and that in the new position it is in hydrostatic equillibrium ($dP_b = dP$), we get

$$\tag{5.1.14} - \left( 1 - \frac{1}{\gamma} \right) \frac{T}{P} \frac{dP}{dr} > -\frac{dT}{dr} $$

Assuming an ideal gas with adiabatic index $\gamma$. The LHS of the expression is the adiabatic temperature gradient, while the RHS is the actual temperature gradient. As long as eq 5.1.14 is satisfied, convection will not take place. Convection starts when these two are just equal, or

$$\tag{5.1.15} \boxed{ \frac{dT}{dr} = \left(1 - \frac{1}{\gamma} \right) \frac{T}{P} \frac{dP}{dr} } $$

### Eddigton Luminosity

The equation for temperature gradient due to radiation (eq 5.1.12) can be written in terms of radiation pressure as

$$ \frac{dP_\text{rad}}{dr} = - \frac{\kappa \rho}{c} \frac{L}{4 \pi R^2} $$

near the surface. Hydrostatic equillibrium demands that near the surface

$$ \frac{dP}{dr} = - \frac{GM \rho}{R^2} $$

This puts an upper limit on a star's luminosity, called the Eddington limit

$$\tag{5.1.16} L_\text{ED} = \frac{4\pi Gc}{\kappa} M $$

For pure ionized hydrogen, $\kappa = \sigma_T / m_p$.

Stars with higher luminosity will slowly their mass to attain hydrostatic equillibrium.

## Boundary Conditions

We have four differential equations for stellar structure

$$
\begin{aligned}
\frac{dm}{dr} = 4 \pi r^2 \rho \qquad \qquad&
\frac{dP}{dr} = - \frac{Gm \rho}{r^2} \\
\frac{dl}{dr} = 4\pi r^2 \rho \varepsilon \qquad \qquad&
\frac{dT}{dr} = \begin{cases}
-\frac{3}{4ac} \: \frac{\kappa \rho}{T^3} \frac{l_\text{rad}}{4 \pi r^2} &\small{\text{(for radiation)}} \\ \frac{dT}{dr} = \left(1 - \frac{1}{\gamma} \right) \frac{T}{P} \frac{dP}{dr} &\small{\text{(for convection)}}
\end{cases}
\end{aligned}
$$

But seven variables. Hence we need three more equations. Generally these are

- Equation of state: $P = P(\rho, T, [X])$
- $\kappa = \kappa(\rho, T, [X])$
- $\varepsilon = \varepsilon(\rho, T, [X])$

Here $[X]$ represents the chemical composition of the star. In addition to this, the boundary conditions usually taken are:

- $m(r=0) \,= 0,\quad\:\:  l(r=0) \:= 0$
- $m(r=R) = M,  \:\:\: l(r=R) \,= L$
- $T(r=R) \,= 0,\quad P(r=R) = 0, \quad \rho(r=R) = 0$

## Energy generation in stars

Stars are fueled by thermonuclear fusion reactions which take place in their cores. The binding energy of an atom $\ce{^A_ZX}$ is

$$ Q = Z m_p + (A-Z) m_n - m_X $$

The binding energy per nucleon is $Q/A$, which is maximum for iron (Z = 56).

The main reactions which take place in stars are

### Proton-Proton (pp) Chain

$$
\begin{align}
\text{ppI}: \qquad & \ce{^1H + ^1H &->& \quad ^2H + e^+ + \nu_e} \\
& \ce{^2H + ^1H &->& \quad ^3He + \gamma} \\
& \ce{^3He + ^3He &->& \quad ^4He + 2 ^1H} \\
\end{align}
$$

$$
\begin{align}
\text{ppII}: \qquad \tag{3} & \ce{^3He + ^4He &->& \quad ^7Be + \gamma} \\
& \ce{^7Be + e^- &->& \quad ^7Li + \nu_e} \\
& \ce{^7Li + ^1H &->& \quad ^4He + ^4He} \\
\end{align}
$$

$$
\begin{align}
\text{ppIII}: \qquad \tag{3} & \ce{^3He + ^4He &->& \quad ^7Be + \gamma} \\
\tag{4} & \ce{^7Be + ^1 H &->& \quad ^8B + \gamma} \\
\tag{5} & \ce{^8B &->& \quad ^8Be + e^+ + \nu_e} \\
\tag{6} & \ce{^8Be &->& \quad ^4He + ^4He} \\
\end{align}
$$

Reaction (1) has a very small probability of occuring, ~ $10^{10}$ years on average. The ppI chain is responsible for ~$91$% of sun's energy production.

### CNO Cycle

$$
\begin{align}
\tag{1} \ce{^{12}C + ^1H &-> ^{13}N + \gamma} \\
\tag{2} \ce{^{13}N &-> ^{13}C + e^+ + \nu_e} \\
\tag{3} \ce{^{13}C + ^1H &-> ^{14}N + \gamma} \\
\tag{4} \ce{^{14}N + ^1H &-> ^{15}O + \gamma} \\
\tag{5} \ce{^{15}O &-> ^{15}N + \gamma + \nu_e} \\
\tag{6} \ce{^{15}N + ^1H &-> ^{12}C + ^4He} \\
\tag{7} \end{align}
$$

### Triple Alpha Reaction

$$
\begin{align}
\tag{1} \ce{^{4}He + ^4He &<-> ^{8}Be} \\
\tag{2} \ce{^{4}He + ^8Be &-> ^{12}C + \gamma} \\
\end{align}
$$

This is commonly written as $\ce{3 ^4He -> ^{12}C + \gamma}$

### Carbon Burning

$$
\begin{aligned}
\ce{^{12}C + ^{12}C &-> ^{24}Mg + \gamma} \\
\ce{&-> ^{23}Na + ^1H} \\
\ce{&-> ^{20}Ne + ^4He} \\
\ce{&-> ^{23}Mg + n^0} \\
\ce{&-> ^{16}O + 2 ^4He} \\
\end{aligned}
$$

Carbon Burning occurs when Helium is exhausted.

### Oxygen Burning

$$
\begin{aligned}
\ce{^{16}O + ^{16}O &-> ^{32}S + \gamma} \\
\ce{&-> ^{31}P + ^1H} \\
\ce{&-> ^{28}Si + ^4He} \\
\ce{&-> ^{31}S + n^0} \\
\ce{&-> ^{24}Mg + 2 ^4He} \\
\end{aligned}
$$

### Silicon Burning

$$
\begin{aligned}
\ce{^{28}Si + ^{28}Si &-> ^{56}Ni + \gamma} \\
\ce{^{56}Ni &-> ^{56}Fe + 2e^+ + 2\nu_e} \\
\end{aligned}
$$
