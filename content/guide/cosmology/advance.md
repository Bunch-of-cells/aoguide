---
title: Advanced Topics
weight: 5
---

## Recombination and Decoupling

The epoch of recombination is the time at which the baryonic component of the universe goes from being ionized to neutral. The epoch of photon decoupling is the time at which the rate at which the photons scatter from electrons becomes less than the Hubble parameter. Here the universe becomes transparent. The epoch of last scattering is the time at which a typical CMB photon underwent its last scattering from an electron.

In early universe,

$$H + \gamma \leftrightharpoons p + e$$

while the photons are still coupled to the baryonic component. This reaction will be in statistical equillibrium. In statistical equillibrium at temperature $T$, the number density $n_X$ of particles with mass $m_X$ is given by

$$\tag{7.4.1} n_X = g_X \left( \frac{m_X kT}{2 \pi \hbar^2} \right)^{3/2} \, \exp(-\frac{m_X c^2}{kT})$$

when $kT \ll m_X c^2$. Here $g_X$ is the statistical weight of the particle $X$. For electrons, protons and neutrons, $g = 2$. For Hydrogen, $g_H = g_p g_e = 4$.

Since $m_H \approx m_p$ and $Q = (m_p + m_e - m_H)c^2 \approx 13.6 \, \mathrm{eV}$, we get

$$\tag{7.4.2} \frac{n_H}{n_e n_p} = \left( \frac{m_e kT}{2 \pi \hbar^2} \right)^{-3/2} \, \exp(-\frac{Q}{kT})$$

This is called the Saha equation.

We define the fraction ionisation $X$ as

$$\tag{7.4.3} X = \frac{n_p}{n_p + n_H} = \frac{n_e}{n_\text{bary}} = \frac{n_e}{n_\text{bary}}$$

From this we get that $n_H = \frac{1-X}{X} n_p$. For overall charge neutrality, we have $n_e = n_p$. Therefore

$$\tag{7.4.4} \frac{1-X}{X} = n_p \left( \frac{m_e kT}{2 \pi \hbar^2} \right)^{-3/2} \, \exp(-\frac{Q}{kT})$$

We define

$$\eta = \frac{n_\text{bary}}{n_\gamma} = \frac{n_p}{X n_\gamma}$$

For the blackbody spectrum, $n_\gamma = 0.243 \left( \frac{kT}{\hbar c} \right)^3$.

For $X = 0.5$ and $\eta = 5.5 \times 10^{-10}$, we get $T_\text{rec} = 3740 \, \mathrm{K}$ and $z_\text{rec} = 1370$, which is $t = 240,000 \, \mathrm{yrs}$ after bigbang.

The rate of photon scattering is

$$\tag{7.4.5} \Gamma = \frac{c}{\lambda} = n_e \sigma_e c= X (1+z)^3 n_{\text{bary},0} \sigma_e c$$

where $\sigma_e$ is the Thomson cross-section. Since $\frac{H^2}{H_0^2} = \Omega_{\text{m},0} (1+z)^3$, we get

$$\tag{7.4.6} 1+z_\text{dec} \approx \frac{43}{X z_\text{dec}^{3/2}}$$

The redshift of photon decoupling was found to be $z_\text{dec} = 1120$. However, the exact value is somewhat smaller, about $z_\text{dec} = 1090$, for which $T_\text{dec} = 2970 \, \mathrm{K}$ and $t = 371,000 \, \mathrm{yrs}$. The last scattering happened too around this time, $z_\text{ls} \approx z_\text{dec} \approx 1100$.
