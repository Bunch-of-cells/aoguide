---
title: Detectors
weight: 1
prev: /guide/optics/
---

## Focal Length and Aperture

The light gathering power of any telescope is propotional to the area of its aperture, which is proptional to the square of its diameter $D$. Hence the size of a telescope is expressed in terms of its diameter.

The transmission efficieny is the fraction of the energy found in an image to the energy collected by the aperture.

The distance between primary image and the aperture is defined as the focal length $F$. The focal ratio or f number is defined as

$$\tag{4.1.1} f = \frac{F}{D} $$

This is synonymous with the speed of an optical system (in everyday photography, exposure time scales as $f^2$).

For 2 stars separated by an angular distance $\theta$, the separation between their images on the focal plane is

$$\tag{4.1.2} s = F \tan \theta \approx F \theta $$

The small angle approximation can be used when $\theta$ is small. The plate scale is defined as

$$\tag{4.1.3} \frac{d \theta}{d s} = \frac{1}{F} $$

## Resolving Power

The resolving power of a telescope is its ability to separate objects with small angle between them. The fundamental limit for a telescope to separate objects which are apparently close together is the theoretical resolving power of the instruments. It is the least angular separation between two stars for them to appear resolved. For a circular aperture,

$$\tag{4.1.6} \theta \approx 1.22 \frac{\lambda}{D} $$

For a slit aperture, $\theta = \frac{\lambda}{D}$

Telescopes whose resolving power is limited by the theoretical resolving power are called diffraction limited. Usually Earth based telescopes are not diffraction limited, by seeing limited, which is a phenomenon caused by the atmosphere.

## Magnifying Power

The magnifying power of a telescope is the ratio of the angle subtended by the virtual image at the eye to the angle subtended by the object at the collector

$$\tag{4.1.8} m = \frac{\alpha_e}{\alpha_c}$$

Usually, position of the eyepiece is adjusted to give a virtual image at infinity. The collector aperture acts as the entrance pupil and image of it formed by the eyepiece acts as the exit pupil. The eye relief is the distance between the eyepiece and the eye. In such a configuration, the magnifying power is given by

$$\tag{4.1.9} m = \frac{\alpha_e}{\alpha_c} = \frac{F_c}{F_e} = \frac{D}{d} $$

where $F_c$ and $F_e$ are the focal lengths of the collector and eyepiece respectively, and $D$ and $d$ are the diameters of the collector and eyepiece respectively.

For all light collected by the collector be made available for viewing by the eye, the magnification must be sufficiently great to make the exit pupil equal to or smaller than the entrance pupil of the eye ($d_\text{eye} \approx 8 \, \mathrm{mm}$).

$$ m = \frac{D}{d} \ge \frac{D}{d_\text{eye}} = \frac{D}{8 \, \mathrm{mm}} $$

The resolving power of the eye is ~$1'$. A further lower limit on magnification is set by the resolving power of the eye. The minimum resolvable angle is given by

$$ m \ge \frac{D}{2 \, \mathrm{mm}} $$

The upper limit to magnification is set by the quality of the optics and quality of the formed image. Whittaker's rule states

$$ m \le \frac{D}{1 \, \mathrm{mm}} $$

Refracting telescopes suffer from many problems

- Large lenses are heavy and difficult to make
- Both the surfaces of the lens must be polished to a high degree of accuracy
- Lenses absorb light, propotional to the thickness of the lens
- In larger lenses, the glass may deform under its own weight and slide out of focus
- Lenses bend light of different wavelengths by different amounts, causing chromatic abberation

## Field of view

The field of view of the eyepiece or the apparent field of view is the angular extent of the sky that can be seen with the eyepiece.

The true field of view or the field of view of the telescope is the angular extent of the sky that can be seen through the telescope. The true field of view is given by

$$\tag{4.1.7} \text{FOV} = \frac{\text{AFOV}}{m} $$

where AFOV is the apparent field of view and $m$ is the magnification.

## Charge-Coupled Devices (CCDs)

A CCD comprises of a matrix of pixels, typically ~$10^4 \times 10^4$ in number. The final outputs of the signal levels are expressed in 'analogue to digital' units or ADUs. A specific number of photoelectrons correspond to a single ADU, which depends on the CCD. The quantum efficiency is the fraction of photons detected by the CCD. For CCDs, the quantum efficiency is above 80%, and varies from pixel to pixel. Flat fielding (uniform illumination of CCD) is done to estimate the quantum efficiency across pixels. Quantum efficiency of the eye is ~1%. A CCD has a linear response to the number of photons incident on it.

## Pixel Spread Function (PSF)

Stars have finite size in CCD images. This is because of the diffraction limit of the telescope used, atmospheric effects and optics of the telescope. Typically 3-4 pixels are required to resolve a star. The PSF is the response of the system to a point source of light. The star's light is spread over a number of pixels, and the PSF is the distribution of light over these pixels. All of the star's light falling on a single pixel is bad, since it makes it hard to distinguish noise. The PSF looks different for faint and bright stars, because the noise is high in faint sources (hence PSF is higher for bright stars). The PSF is usually modeled as a Gaussian function, which is a bell-shaped curve. The width of the Gaussian is called the full width at half maximum (FWHM), which is the distance between the two points on the curve where the intensity is half of its maximum value.

## Noise

Noise are the unpredicatable variations in data that obscure or distort the true characteristics of the system under study. Noise encompasses all factors that contribute to measurement uncertainities $\sigma_i$. If all noise sources are independent, the total noise is given by

$$\tag{4.1.10} \sigma^2 = \sum_i \sigma_i^2 $$

### Telescope

The number of photons from a star of spectral flux density $F_\lambda$ hitting the aperture are

$$\tag{4.1.4} N_T = \frac{\pi}{4} D^2 \cdot \Delta t \cdot \int_{\lambda_2}^{\lambda_1} \frac{F_\lambda}{hc / \lambda} \, d\lambda $$

where $\lambda_1$ and $\lambda_2$ are the limit for the spectral range of the measurement and $\Delta t$ is the integration time of measurement.

When the arriving flux is low, fluctuations are seen in any recorded signal, termed photon shot noise. If no other noise sources are present, the uncertainity is given by $\pm \sqrt{N_T}$. Hence any recorded signal may be expressed as $N_T \pm \sqrt{N_T}$. The signal to noise ratio (SNR) is defined as

$$\tag{4.1.5} \text{SNR} = \frac{N_T}{\sqrt{N_T}} \propto D \sqrt{\Delta t} $$

### CCD

Suppose over an exposure a star provides $N_*$ photons spread over $p$ pixels, and the background sky signal provides $N_\text{sky}$ photons to the same pixels. For an exposure time $t$ with background signal (dark current) of $N_d \mathrm{\,s^{-1}}$ per pixel and with a readout noise of $\pm \sigma$ per pixel, the SNR is given by

$$\tag{4.2.1} \text{SNR} = \frac{N_*}{\sqrt{N_* + N_\text{sky} + p N_d t + p \sigma^2}} $$

The dark current is the thermal noise in the CCD. Readout noise, also called bias voltage, leak noise or residual voltage, is the noise introduced while reading out from the CCD. Dynamic range is the maximum SNR of a CCD.

Subtracting the dark frame (image captured with the shutter closed) removes the dark current and readout noise. Dividing by the flat field image removes the pixel-to-pixel variations in the quantum efficiency. Additionally, it is important to calibrate the CCD to ensure accurate measurements.
