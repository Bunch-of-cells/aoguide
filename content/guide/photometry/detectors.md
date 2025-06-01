---
title: Detectors
weight: 4
---

Detectors are devices that convert light into an electrical signal. They are used in telescopes to capture images of celestial objects. The most common type of detector used in telescopes is the Charge-Coupled Device (CCD). Other types of detectors include photomultiplier tubes (PMTs), photodiodes, and avalanche photodiodes. They play a crucial role in astrophotometry, which is the measurement of the brightness of celestial objects.

A telescope is an optical instrument that collects and magnifies light from distant objects. It consists of a primary mirror or lens that gathers light and focuses it to form an image. The image is then magnified by an eyepiece or camera, allowing the observer to see the object in greater detail.

## Focal Length and Aperture

Aperture is the opening through which light enters a telescope, and is often referred to as the diameter $D$ of the primary mirror or lens of a telescope. It is the most important factor in determining the light-gathering power of a telescope. The larger the aperture, the more light the telescope can collect, and the fainter objects it can observe.

The transmission efficiency $\eta$ of a detector is defined as the fraction of the energy found in an image to the energy collected by the aperture.

The focal length $F$ of a telescope is the distance from the primary image to the aperture. The primary image is formed at the focal plane, where the light rays converge after passing through the primary mirror or lens.

The focal ratio or f number of a telescope is defined as

$$\tag{2.4.1} f = \frac{F}{D} $$

This is synonymous with the speed of an optical system (in everyday photography, exposure time scales as $f^2$).

For 2 objects separated by an angular distance $\theta$ in the sky, the separation between their images on the focal plane is

$$\tag{2.4.2} s = F \tan \theta \approx F \theta $$

The small angle approximation can be used when $\theta$ is small. The plate scale is defined as

$$\tag{2.4.3} \frac{d \theta}{d s} = \frac{1}{F} $$

## Resolving Power

The resolving power of a telescope is its ability to separate objects with small angle between them. The fundamental limit for a telescope to separate objects which are apparently close together is the theoretical resolving power of the instruments. It is the least angular separation between two stars for them to appear resolved. For a circular aperture,

$$\tag{2.4.4} \theta \approx 1.22 \frac{\lambda}{D} $$

For a slit aperture,

$$\tag{2.4.5} \theta = \frac{\lambda}{D}$$

These relations are derived from the diffraction limit of the aperture, which is a consequence of the wave nature of light. The Rayleigh criterion states that two point sources are considered resolved when the first minimum of the diffraction pattern of one source coincides with the central maximum of the diffraction pattern of the other source.

The resolving power of the eye is ~$1'$

{{< callout type="math" >}}
{{% details title="Diffraction by a Slit Aperture" closed="true" %}}

Consider a slit of width $D$. When monochromatic light of wavelength $\lambda$ passes through the slit, it diffracts and forms an interference pattern on a distant screen. The condition for the first minimum in the diffraction pattern is

$$ D \sin \theta = \lambda $$

For small angles, $\sin \theta \approx \theta$, so

$$ \theta = \frac{\lambda}{D} $$

This gives the angular resolution limit for a slit aperture.

{{% /details %}}
{{< /callout >}}

{{< callout type="math" >}}
{{% details title="Diffraction by a Circular Aperture" closed="true" %}}

Consider a circular hole of radius $R$ in the $xy$ plane. Coherent light enters the hole from the direction of the negative $z$ axis. We consider light rays leaving the hole parallel to the $xz$ plane forming an angle $\theta$ with the $z$ axis. The light waves interfere on a screen far away. The phase difference between a wave through a point $(x,y)$ and a wave going through the centre of the hole can be calculated from the different path lengths $s = x \sin \theta$:

$$ \delta = \frac{s}{\lambda} 2\pi = \frac{2 \pi \sin \theta}{\lambda} x \equiv kx $$

Thus, the phase difference $\delta$ depends on the $x$ coordinate only. The sum of the amplitudes of the waves from a small surface element is proportional to the area of the element $dx \, dy$. Let the amplitude coming through the centre of the hole be $d\vec{a_0} = dx \, dy \, \hat{i}$. The amplitude coming from the point $(x,y)$ is then

$$ d\vec{a} = dx \, dy \, (\cos \delta \hat{i} + \sin \delta \hat{j})$$

We sum up the amplitudes coming from different points of the hole

$$\begin{align*}
\vec{a} &= \int_\text{Aperture} d\vec{a} \\
&= \int_{x = -R}^{R} \int_{y = -\sqrt{R^2 - x^2}}^{\sqrt{R^2 - x^2}} dx \, dy \, (\cos kx \hat{i} + \sin kx \hat{j}) \\
&= 2 \int_{-R}^R \sqrt{R^2 - x^2} \cos kx \, dx \, \hat{i} + 2 \int_{-R}^R \sqrt{R^2 - x^2} \sin kx \, dx \, \hat{j} \\
&= 4 \int_{0}^R \sqrt{R^2 - x^2} \cos kx \, dx \, \hat{i}
\end{align*}$$

The second integral vanishes because the integrand is an odd function. The first integral can be solved using integration by parts, or by using the formula for the Bessel function of the first kind of order one $J_1(x)$:

$$\int_0^R \sqrt{R^2 - x^2} \cos kx \, dx = R^2 J_1(kR)$$

The first zero of the Bessel function $J_1(x)$ is at $x \approx 3.8317$. The first zero of the diffraction pattern is at

$$ kR = 3.8317 \implies \theta = \frac{3.8317 \lambda}{2\pi R} $$

The first zero of the diffraction pattern is at

$$\theta \approx 1.22 \frac{\lambda}{D} $$

where $D = 2R$ is the diameter of the aperture. This is the theoretical resolving power of a telescope with a circular aperture.

{{% /details %}}
{{< /callout >}}

{{< callout type="remark" >}}
Telescopes whose resolving power is limited by the theoretical resolving power are called diffraction limited. Usually Earth based telescopes are not diffraction limited, but seeing limited, which is a phenomenon caused by the atmosphere.

Seeing is the degradation of images caused by the turbulence in the Earth's atmosphere, that may be visible as blurring, twinkling or variable distortion of images. The diameter of the seeing disk is defined as the FWHM (full width at half maximum) of its optical intensity. A seeing of 1'' means that the smallest resolvable detail in an image are blurred out to a disk of 1 arcsecond in diameter. The seeing disk is the image of a point source, such as a star, as seen through the atmosphere. The seeing disk is typically about 1-2'' in diameter for good observing conditions.

To overcome seeing, telescopes are built at high altitudes, where the atmosphere is thinner and less turbulent. Adaptive optics is also used to correct for atmospheric distortions in real time.
{{< /callout >}}

## Magnifying Power

The magnifying power of a telescope is the ratio of the angle subtended by the virtual image at the eye to the angle subtended by the object at the collector

$$\tag{2.4.6} m = \frac{\alpha_e}{\alpha_c}$$

Usually, position of the eyepiece is adjusted to give a virtual image at infinity. The collector aperture acts as the entrance pupil and image of it formed by the eyepiece acts as the exit pupil. The eye relief is the distance between the eyepiece and the eye. In such a configuration, the magnifying power is given by

$$\tag{2.4.7} m = \frac{\alpha_e}{\alpha_c} = \frac{F_c}{F_e} = \frac{D}{d} $$

where $F_c$ and $F_e$ are the focal lengths of the collector and eyepiece respectively, and $D$ and $d$ are the diameters of the collector and eyepiece respectively.

{{< callout type="remark" >}}
In reality, the magnifying power of a telescope is limited by several factors, including the size of the exit pupil, the resolving power of the eye, and the quality of the optics.

For all light collected by the collector be made available for viewing by the eye, the magnification must be sufficiently great to make the exit pupil equal to or smaller than the entrance pupil of the eye ($d_\text{eye} \approx 8 \, \mathrm{mm}$).

$$ m = \frac{D}{d} \ge \frac{D}{d_\text{eye}} = \frac{D}{8 \, \mathrm{mm}} $$

A further lower limit on magnification is set by the resolving power of the eye. The minimum resolvable angle is given by

$$ m \ge \frac{D}{2 \, \mathrm{mm}} $$

The upper limit to magnification is set by the quality of the optics and quality of the formed image. Whittaker's rule states

$$ m \le \frac{D}{1 \, \mathrm{mm}} $$
{{< /callout >}}

## Limiting Magnitude

For starlight, the limit of unaided eye detection is set at about $6^m$. This limit however can be increased by using a detector with a larger aperture size, such as a telescope. Consider a telescope with an aperture diameter D. Since the flux recieved is directly propotional to the recieving area,

$$ \frac{F_t}{F_e} = \frac{D^2}{d^2} $$

where $d$ is the size of the eye pupil, approximately $8 \, \mathrm{mm}$. The limiting magnitude of the telescope is defined as the magnitude of the faintest object that can be detected by the telescope. The limiting magnitude $m_t$ of a telescope with an aperture diameter D is given by

$$\tag{2.4.8} m_t - m_e = -2.5 \log \left( \frac{F_t}{F_e} \right) = -5 \log \frac{D}{d} $$

where $m_e = 6^m$ is the limiting magnitude of the eye.

100% of the light hitting the aperture is not collected by the telescope. The light is scattered, absorbed, and reflected by the telescope optics. The fraction of light that is actually collected is called the transmission efficiency $\eta$. The limiting magnitude of a telescope with an aperture diameter D and trasmission efficiency $\eta$ is given by

$$\tag{2.4.9} m_t = m_e -2.5 \log \left( \eta \frac{D^2}{d^2} \right)$$

## Field of view

The field of view of the eyepiece or the apparent field of view is the angular extent of the sky that can be seen with the eyepiece.

The true field of view or the field of view of the telescope is the angular extent of the sky that can be seen through the telescope. The true field of view is given by

$$\tag{2.4.10} \text{FOV} = \frac{\text{AFOV}}{m} $$

where AFOV is the apparent field of view and $m$ is the magnification.

## Charge-Coupled Devices (CCDs)

A CCD is a semiconductor device that converts light into an electrical signal. It consists of an array of pixels, typically ~$10^4 \times 10^4$, each of which can store a charge proportional to the amount of light that falls on it. The charge is then read out and converted into a digital signal, which can be processed and analyzed.

The final output of the signal levels are expressed in 'analogue to digital' units or ADUs (Analog to Digital Units). A specific number of photoelectrons correspond to a single ADU, which varies from CCD to CCD.

A CCD has a linear response to the number of photons incident on it, meaning that the output signal is directly proportional to the number of photons detected. However, the response is not perfectly linear, and there is a saturation point beyond which the CCD cannot detect any more photons. This saturation point is called the full well capacity.

### Pixel Spread Function (PSF)

Stars have finite size in CCD images. This is because of the diffraction limit of the telescope used, atmospheric effects and optics of the telescope. Typically 3-4 pixels are required to resolve a star. The PSF is the response of the system to a point source of light. The star's light is spread over a number of pixels, and the PSF is the distribution of light over these pixels. The PSF is usually modeled as a Gaussian function.

All of the star's light falling on a single pixel is undesirable, since it makes it hard to distinguish noise from the signal. The PSF looks different for faint and bright stars, because the noise is high in faint sources (hence PSF is higher for brighter stars).

### Noise

Noise are the unpredicatable variations in data that obscure or distort the true characteristics of the system under study. Noise encompasses all factors that contribute to measurement uncertainities $\sigma_i$. If all noise sources are independent, the total noise is given by

$$\tag{2.4.11} \sigma^2 = \sum_i \sigma_i^2 $$

The number of photons from a star of spectral flux density $F_\lambda$ hitting the aperture of the detector are

$$\tag{2.4.12} N_T = \frac{\pi}{4} D^2 \cdot \Delta t \cdot \int_{\lambda_2}^{\lambda_1} \frac{F_\lambda}{hc / \lambda} \, d\lambda $$

where $\lambda_1$ and $\lambda_2$ are the limit for the spectral range of the measurement and $\Delta t$ is the integration time of measurement.

When the arriving flux is low, fluctuations are seen in any recorded signal, termed photon shot noise. If no other noise sources are present, the uncertainity is given by $\pm \sqrt{N_T}$. Hence any recorded signal may be expressed as $N_T \pm \sqrt{N_T}$.

The signal to noise ratio (SNR) is a measure of the quality of the signal relative to the noise. A higher SNR indicates a better quality signal, while a lower SNR indicates a poorer quality signal. The SNR is an important factor in determining the sensitivity of a detector and its ability to detect faint objects. If the only noise source is the photon shot noise, the SNR is given by

$$\tag{2.4.13} \text{SNR} = \frac{N_T}{\sqrt{N_T}} = \sqrt{N_T} $$

The dynamic range of a CCD is the ratio of the maximum signal that can be detected (the full-well capacity of the CCD) to the camera noise. It's essentially the ability of the camera to capture both bright and dim areas simultaneously. The dynamic range is typically around $10^4$ for CCDs.

{{< callout type="remark" >}}
The dark current $N_\text{d}$ is the number of electrons generated by thermal noise in the CCD per second. It is a source of noise that adds to the photon shot noise. The readout noise $\sigma$, also called bias voltage, is the noise introduced while reading out the signal from the CCD. It is also a source of noise that adds to the photon shot noise.

The image can be corrected for dark current and readout noise by subtracting a dark frame. The dark frame is an image taken with the shutter closed, which captures the dark current and readout noise.

The quantum efficiency is defined as the fraction of photons detected by the CCD to the total number of photons incident on the CCD. For CCDs, the quantum efficiency is typically above 80%, and it varies from pixel to pixel. The pixel-to-pixel variations can be corrected by dividing the image by a flat field image. The flat field image is an image taken with a uniform illumination of the CCD, which captures the pixel-to-pixel variations in the quantum efficiency. Additionally, it is important to calibrate the CCD to ensure accurate measurements.

The quantum efficiency of the human eye is approximately 1%.
{{< /callout >}}

Suppose over an exposure a star provides $N_*$ photons spread over $p$ pixels, and the background sky signal provides $N_\text{sky}$ photons to the same pixels. For an exposure time $t$ with a dark current of $N_d \mathrm{\,s^{-1}}$ per pixel and with a readout noise of $\pm \sigma$ per pixel, the SNR is given by

$$\tag{2.4.14} \text{SNR} = \frac{N_*}{\sqrt{N_* + N_\text{sky} + p N_d t + p \sigma^2}} $$

### Intrumental Magnitude

The intrumental magnitude is a measure of the brightness of an object as seen by a detector, such as a CCD. Instrumental magnitudes are usually measured relative to the sky background in each CCD frame. Prior to measuring the instrumental magnitudes the various instrumental effects should be removed from the CCD frames. It is defined as

$$\tag{2.4.15} m_\text{inst} = A -2.5 \log \left[ \frac{\left(\sum_{i=1}^{n} C_{i}\right) - nC_\text{sky}}{\Delta t} \right]$$

where

- $A$ is an arbitrary constant which is often added to the instrumental magnitudes. This is often set to a silly value, say 30, so that the instrumental magnitudes have very different values from the corresponding calibrated magnitudes and hence the two are unlikely to be inadvertently confused.
- $C_i$ is the count in the $i^\text{th}$ pixel inside the aperture.
- $C_\text{sky}$ is the average count in the background sky pixels.
- $n$ is the number of pixels in the aperture.
- $\Delta t$ is the exposure time, or the integration time of the frame.

The instrumental magnitude then has to be calibrated to the standard magnitude system, such as the Johnson-Cousins system, to obtain the standard magnitude of the object. When calibrating without color correction, the instrumental magnitude is related to the calibrated magnitude by

$$\tag{2.4.16} m_\text{calib} = m_\text{inst} - A + Z + \kappa X $$

where $Z$ is a photometric zero point between the standard and instrumental systems (determined using a standard star), $\kappa$ is the atmospheric extinction coefficient, and $X$ is the airmass of the observation.

## Problems

{{< tabs items="P1,Solution,IOAA 2012" >}}
    {{< tab >}}
    An astronomer on Earth observes a globular cluster, which has an angular diameter $\alpha$ and contains $N$ stars, each one with the same absolute magnitude $M_0$, and is at a distance $D$ from the Earth. A biologist is in the center of that cluster.

    a) What is the difference between the combined visual magnitudes of all stars observed by the astronomer and the biologist. Consider that the spatial distribution of stars in the cluster is perfectly homogeneous and the biologist is measuring the combined magnitude of the entire cluster. <br>
    b) What is the diameter of the astronomer’s telescope, considering he wants to visualize the cluster with the same brightness that the biologist sees? <br>
    c) What would be the difference between the visual magnitudes observed by the two scientists, if the diameter of the feild of view of the biologist is also $\alpha$.
    {{< /tab >}}

    {{< tab >}}
    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P2,Solution,IOAA 2017" >}}
    {{< tab >}}
    Supernova SN 1987A was at its brightest with an apparent magnitude of $+3$ on about 15th May  1987 and then faded, finally becoming invisible to the naked eye by 4$^\text{th}$ February 1988. It is  assumed that brightness $B$ varied with time $t$ as an exponential decline, $B(t) = B_0 e^{-t/\tau}$, where $B_0$ and $\tau$ are constant. The maximum apparent magnitude which can be seen by the naked eye is $+6$.

    a) Determine $\tau$ in days. <br>
    b) Find the last day that observers could have seen the supernova if they had a 6-inch (15.24cm) telescope with transmission efficiency $\eta = 0.7$. Assume that the average diameter of the human pupil is 0.6 cm.
    {{< /tab >}}

    {{< tab >}}
    **a)** The time difference in days between 15 May 1987 and 4 February 1988 is 265 days. Since the supernova was last visible to naked eye on 4 February 1988, its apparent magnitude on that day was $m = 6$. Since the flux is propotional to the brightness, using Pogson's equation we have

    $$ 6.0 - 3.0 = -2.5 \log \frac{B(t)}{B_0} = 2.5 \frac{t}{\tau} \log e $$
    $$ \implies \boxed{\tau \approx 96 \, \mathrm{days}} $$

    **b)**
    {{< /tab >}}
{{< /tabs >}}
