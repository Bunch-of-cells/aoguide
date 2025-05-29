---
title: Types of Telescopes
weight: 5
---

## Refracting Telescopes

A refracting telescope uses a lens to form an image. The main lens, called the objective lens, is typically a large, heavy piece of glass. The eyepiece lens magnifies the image produced by the objective lens.

### Thin Lens Approximation

The thin lens approximation simplifies the analysis of lenses by assuming the lens is thin compared to its focal length and that light rays passing through the lens are nearly parallel.

The thin lens equation is:

$$\tag{2.5.1} \frac{1}{F} = (n-1) \left( \frac{1}{R_1} - \frac{1}{R_2} \right) $$

where $F$ is the focal length of the lens, $n$ is the refractive index of the lens material, and $R_1$ and $R_2$ are the radii of curvature of the two surfaces of the lens. The term $n - 1$ is called the refractive power of the lens.

{{< callout type="remark" >}}
Refracting telescopes have several drawbacks:

- Large lenses are heavy and difficult to manufacture.
- Both surfaces of the lens must be polished to a high degree of accuracy.
- Lenses absorb light in proportion to their thickness.
- Large lenses may deform under their own weight, causing the image to go out of focus.
- Lenses bend light of different wavelengths by different amounts, causing chromatic aberration.
{{< /callout >}}

## Reflecting Telescopes

Reflecting telescopes use a mirror to form an image. The mirror is usually a large, heavy piece of glass polished to a high degree of accuracy. The eyepiece lens magnifies the image formed by the mirror.

Reflecting telescopes avoid many problems of refracting telescopes and can be made much larger. They do not suffer from chromatic aberration, as all wavelengths of light are reflected equally.

There are several designs for reflecting telescopes, including Newtonian, Cassegrain, and Ritchey-Chrétien. Each design has its own advantages and disadvantages, and the choice depends on the specific requirements of the telescope.

The focal length of a concave mirror is given by:

$$\tag{2.5.2} F = \frac{R}{2} $$

where $R$ is the radius of curvature of the mirror.

## Aberrations

### Chromatic Aberration

The refractive index $n$ of a lens depends on the wavelength $\lambda$ of light. As a result, different wavelengths have different focal lengths and focus at different planes. This defect is called chromatic aberration. Reflecting telescopes do not suffer from chromatic aberration, as they use mirrors that reflect all wavelengths equally.

The plane containing the smallest possible image (not a point) is called the plane of sharpest focus. The image is known as the circle of least confusion. The spread of the image along the optical axis is called longitudinal aberration, and the spread in the plane perpendicular to the optical axis at the plane of sharpest focus is called lateral aberration.

Chromatic aberration can be corrected by using a combination of lenses made from different materials with different refractive indices. This arrangement is called an achromatic doublet.

{{< callout type="image" >}}
{{< svg "images/photometry/chromatic_aberration.svg" "Chromatic Aberration" "Chromatic Aberration in a lens (source: Wikipedia)" >}}
{{% /callout %}}

### Spherical Aberration

The focus position of a spherical lens for any incident ray depends on its distance from the optical axis. This causes the image to spread along the optical axis, known as spherical aberration. The severity of this aberration can be expressed as the ratio $\Delta F / F$, where $\Delta F$ is the spread of the image along the optical axis and $F$ is the focal length of the lens.

Spherical aberration can be corrected by using a combination of lenses with different shapes, known as a compound lens. It can also be corrected by aspherization, where the lens is shaped to have a non-spherical surface. In case of reflecting telescopes, spherical aberration can be corrected by using a parabolic mirror instead of a spherical one.

{{< callout type="image" >}}
{{< svg "images/photometry/spherical_aberration.svg" "Spherical Aberration" "Spherical Aberration in a lens (source: Wikipedia)" >}}
{{% /callout %}}

### Coma

Coma is an aberration where the image of a point object off the optical axis appears comet-shaped.

Coma can be corrected using an aplanatic lens, which is a combination of two lenses with different shapes. The first lens is positive, and the second is negative. The two lenses are placed at a distance equal to their focal lengths, with their optical axes aligned.

{{< callout type="image" >}}
{{< svg "images/photometry/coma.svg" "Coma" "Coma in a lens (source: Wikipedia)" >}}
{{% /callout %}}

### Astigmatism

Astigmatism is a defect where the image of a point object appears as a line rather than a point. This occurs when the lens is not perfectly spherical. It can be corrected by using a combination of lenses with different shapes.

A parabolic mirror corrects spherical aberration but increases astigmatism. A spherical mirror reduces astigmatism but increases spherical aberration.

### Field Curvature

Field curvature is a defect where the image of a point object forms on a curved surface rather than a flat plane. This can be corrected by using a combination of lenses with different shapes.

A field flattener is a lens used to correct field curvature. It is placed at the focal plane of the telescope and aligned with the optical axis.

### Distortion

Distortion is a defect where the image of a point object appears as a distorted shape. This can be corrected by using a combination of lenses with different shapes.

A distortion corrector is a lens placed at the focal plane of the telescope and aligned with the optical axis to correct distortion.

## Types of Telescopes

### Galilean Telescope

A Galilean telescope is a type of refracting telescope that uses a converging lens as the objective and a diverging lens as the eyepiece. Parallel rays of light from a distant object are brought to a focus by the objective lens. The diverging eyepiece lens intercepts these rays and makes them parallel again. Non-parallel rays from the object, traveling at an angle to the optical axis, emerge at a larger angle after passing through the eyepiece. This increases the apparent angular size and produces magnification. The final image is virtual, located at infinity, and is upright (not inverted).

### Keplerian Telescope

The Keplerian telescope improves on Galileo's design by using a convex lens as the eyepiece instead of a concave one. This arrangement causes the rays of light emerging from the eyepiece to be converging, allowing for a wider field of view and greater eye relief. However, the image is inverted. Higher magnifications are possible with this design, but it still uses a simple single-element objective lens, so a high focal ratio is needed to reduce aberrations.

### Cassegrain Telescope

The Cassegrain reflector uses a primary concave mirror and a secondary convex mirror. The optical path folds back onto itself, placing the focal point behind the primary mirror. The convex secondary mirror creates a telephoto effect, resulting in a much longer focal length in a compact system.

#### Ritchey-Chrétien Telescope

The Ritchey-Chrétien is a specialized Cassegrain reflector with two hyperbolic mirrors (instead of a parabolic primary). It is free of coma and spherical aberration at a flat focal plane, making it ideal for wide-field and photographic observations.

#### Catadioptric Cassegrains

Catadioptric Cassegrains use two mirrors, often with a spherical primary mirror to reduce cost, combined with refractive corrector elements to correct aberrations. Examples include the Schmidt-Cassegrain and Maksutov-Cassegrain designs. The Schmidt-Cassegrain uses a thin corrector plate to correct spherical aberration, while the Maksutov-Cassegrain uses a thick meniscus lens to correct both spherical aberration and coma.

### Newtonian Telescope

A Newtonian telescope consists of a primary mirror, usually parabolic, and a smaller flat secondary mirror. The primary mirror collects light from the sky, while the secondary mirror redirects the light at a right angle so it can be viewed through an eyepiece.

## Interferometry

Interferometry is a technique that combines the light from two or more telescopes to create an interference pattern. This allows astronomers to achieve higher resolution than a single telescope can provide. The technique is based on the principle of superposition, where the light waves from different telescopes combine to produce a new wave pattern.

Interferometry can be used with both radio and optical telescopes. In radio interferometry, the signals from multiple radio antennas are combined to create a virtual telescope with a much larger effective aperture. In optical interferometry, the light from multiple telescopes is combined using beamsplitters and mirrors to create interference patterns that can be analyzed to determine the properties of astronomical objects.

The resolution of an interferometer is determined by the distance between the telescopes, known as the baseline. The longer the baseline, the higher the resolution.
