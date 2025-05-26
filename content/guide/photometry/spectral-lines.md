---
title: Spectral Lines
weight: 3
---

## Nature of Radiation

The quanta of electromagnetic radiation is a photon, whose energy is given by $E = h \nu$ where $\nu$ is the frequency of the photon.

Atomic transitions give rise to line spectrum. Hot gases under low pressure produce an emission spectrum. If cold gas is used and observed against a white light, the same lines are seen as absorption lines.

If an electron bound to an atom, having energy $E < 0$ is given energy more than $|E|$, it will leave the atom. This is called a bound-free transition. The inverse process of capturing a free electron is called recombination or free-bound transition.

When an electron scatters from a nucleus or ion without being captured, the radiation emitted is called free-free radiation. In very hot gases, this is the most important form of radiation, and is called thermal bremsstrahlung. The absorption process can be called a bound-bound transition.

Electromagnetic radiation can be polarished - linearly, circularly or elliptically. For a partially linearly polarised beam, the degree of polarisation is defined as

$$ P = \frac{I_{\text{max}} - I_{\text{min}}}{I_{\text{max}} + I_{\text{min}}} $$

where $I_\text{max}$ and $I_\text{min}$ are the maximum and minimum intensities of the beam.

Scattering is an absorption followed by an instantaneous emission at the same wavelength but in a new direction.

Electric fields broaden spectral lines. This is called the Stark effect. The magnetic field also causes broadening of spectral lines, called the Zeeman effect.

A free charge in accelerated motion emits radiation, called synchrotron radiation.

## Bohr's Model of the Atom

Bohr's first postulate states that angular momentum of an electron must be a multiple of $\hbar$.

$$ mvr = n \hbar $$

where $n = 1,2,3, \ldots$ is called the principal quantum number.

The total energy of an electron in the $n^\text{th}$ orbit is

$$\tag{2.1.22} E_n = - \frac{m_e e^4 Z^2}{32 \pi^2 \varepsilon_0^2 \hbar^2 n^2} = - E_0 \frac{Z^2}{n^2} $$

During a transition from the $n_i^\text{th}$ to $n_f^\text{th}$ orbit, the energy of the photon emitted is given by

$$\tag{2.1.23} E = E_{n_i} - E_{n_f} = E_0 Z^2 \left( \frac{1}{n_f^2} - \frac{1}{n_i^2} \right) $$

Thus the wavelength of the photon is

$$\tag{2.1.24} \frac{1}{\lambda} = \frac{E_0 Z^2}{hc} \left( \frac{1}{n_f^2} - \frac{1}{n_i^2} \right) = RZ^2 \left( \frac{1}{n_f^2} - \frac{1}{n_i^2} \right) $$

The spectral lines of hydrogen can be classified into series, based on the final state of the electron. The series are:

- Lyman series: $n_f = 1$. These lie in the ultraviolet range.
- Balmer series: $n_f = 2$. These lies in the visible range.
- Paschen series: $n_f = 3$. These lies in the infrared range.
- Brackett series: $n_f = 4$. These lies in the infrared range.
- Pfund series: $n_f = 5$. These lies in the infrared range.
- Humphreys series: $n_f = 6$. These lies in the infrared range.

## Spectral Broadening

Spectral lines are not infinitely narrow, but have a finite width. The width of the line is called the line profile. The line profile is a function of the wavelength, and is denoted by $I(\lambda)$. The area under the line profile is equal to the total intensity of the radiation. There are several mechanisms which cause broadening of spectral lines. The most important ones are:

### Natural Broadening

The lifetime of excited states results in natural broadening, also known as lifetime broadening. The uncertainty principle relates the lifetime of an excited state with the uncertainty of its energy. A short lifetime will have a large energy uncertainty and a broad emission. This broadening effect results in an unshifted Lorentzian profile.

### Doppler Broadening

This is the broadening of spectral lines due to doppler shift caused by velocity distribution of particles. The resulting profile is called doppler profile, and follows a gaussian distribution.

In the non-relativistic case, doppler shift is $f = f_0 \left( 1 + \frac{v}{c} \right)$. If $P_v(v) \, dv$ is the number of particles having velocities between $v$ and $v + dv$, then the corresponding frequency distribution is

$$
\begin{aligned}
P_f (f) \, df &= P_v (v) \, \frac{dv}{df} \, df \\
&= \frac{c}{f_0} P_v \left[ c \left(\frac{f}{f_0} - 1 \right) \right] \, df
\end{aligned}
$$

Thermal doppler broadening is caused by the thermal motion of the molecules. The velocity distribution of the particles is given by the Maxwell-Boltzmann distribution

$$ P_v (v) \, dv = \sqrt{\frac{m}{2 \pi k T}} \, \exp\left(-\frac{mv^2}{2kT}\right) \, dv $$
$$ \implies P_f (f) \, df = \frac{c}{f_0} \sqrt{\frac{m}{2 \pi k T}} \, \exp\left(-\frac{mc^2}{2kT} \left( \frac{f}{f_0} - 1 \right)^2 \right)  \, df  $$

This is a gaussian profile with a standard deviation of $\sigma = \sqrt{\frac{kT}{mc^2}} f_0$ and FWHM

$$ \Delta f_\text{FWHM} = \sqrt{\frac{8 \ln 2 kT}{mc^2}} f_0 = 2 \sqrt{2 \ln 2} \, \sigma $$

### Pressure Broadening

Impact or collisional pressure broadening is caused by collisions of particles with other particles and follows a lorentzian profile. Pressure broadening can be classified into the following categories

- Impact pressure broadening or collisional broadening
- Quasistatic pressure broadening
- Linear stark broadening
- Quadratic stark broadening
- Vanderwaals broadening
- Resonance broadening
