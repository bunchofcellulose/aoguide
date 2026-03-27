---
title: The Milky Way
weight: 2
---

## Milky Way

The Milky Way is a barred spiral galaxy or type SBbc or SBc that is home to our solar system. It is composed of several components, including the galactic bulge, disk, and halo. The galactic bulge is a dense and bright region of stars located at the center of the galaxy. The disk is a flat region that contains most of the galaxy's stars and gas, a few kiloparsecs thick. The stars found in the disk are relatively younger. The halo is a spherical region that surrounds the galaxy and contains globular clusters, older and redder stars, and dark matter. It is almost spherical.

{{< callout type="image" >}}
{{< png "gal/milkyway.png" "Milky Way" "Structure of our Milky Way galaxy" >}}
{{< /callout >}}

Sun's orbital speed around the galactic center is around 220 km/s, and is at a distance of about 8.5 kpc from the galactic center.

Let the angular velocity of a star in circular orbit around the center of the galaxy be

$$ \omega(R) = \sqrt{\frac{G M(R)}{R^3}} $$

It has been observed that the angular velocity of rotation depends on the distance from the galactic center. Such rotation is called differential rotation. Thus the rotation curve of the galaxy is not keplerian, but rather flattens out after a few kiloparsecs.

{{< callout type="remark" >}}

For stars and gas in the disk of our galaxy to be in stable circular orbits (assuming spherical mass distribution),

$$\tag{6.1.6} \frac{V(R)^2}{R} = \frac{GM(R)}{R^2} \implies M(R) = \frac{V(R)^2 R}{G} $$

It has been observed that in the region outside sun's orbital radius, the orbital velocity is roughly constant, hence the mass enclosed must increase. However, the luminosity decreases exponentially. This "extra" non-luminous mass is termed as dark matter. Approximately 85% of all matter in the universe is in the form of dark matter.

{{< /callout >}}

### Oort Equations

The Local Standard of Rest (LSR) is the reference frame in which the mean velocity of the stars in the solar neighborhood is zero. The velocity of the individual stars relative to the LSR is called the peculiar velocity of the star. The point towards which the Sun is moving relative to the LSR is called the solar apex. The opposite point on the celestial sphere is called the solar antapex. Sun's velocity with respect to the LSR is around 20 km/s, with the apex being located in the constellation Hercules.

Let the sun's orbital speed and orbital radius be $V_\odot$ and $R_\odot$ respectively. For a star in the galactic plane at galactic longitude $l$ and distance $r$ from the sun, its relative velocity with respect to sun is given by

$$\tag{6.3.1} \begin{aligned} V_r &\approx Ar \sin 2l \\ V_t &\approx Ar \cos 2l + Br \implies \mu \approx A \cos 2l + B \end{aligned}$$

where $A$ and $B$ are the first and second Oort constants respectively.

$$\tag{6.3.2}
\begin{aligned}
A &= \frac{1}{2} \left( \frac{V_\odot}{R_\odot} - \frac{d V}{d R} {\Big|}_{r=R_\odot} \right) \approx 15 \mathrm{\,km\,s^{-1}\,kpc^{-1}} \\
B &= -\frac{1}{2} \left( \frac{V_\odot}{R_\odot} + \frac{d V}{d R} {\Big|}_{r=R_\odot} \right) \approx 20 \mathrm{\,km\,s^{-1}\,kpc^{-1}}
\end{aligned}
$$

The angular velocity of LSR around the galactic center ($\omega_0$) can thus be found.

$$
\begin{aligned}
A + B &= -\frac{dV}{dR} \Big|_{r=R_\odot} \\ A-B &= \frac{V_\odot}{R_\odot} = \omega_0\\
\end{aligned}
$$

{{< callout type="image" >}}
{{< svg "gal/oort.svg" "Relative motion of a star in the galaxy" "The Oort equations describe the relative motion of a star in the galaxy." >}}
{{< /callout >}}

### ISM

The interstellar medium (ISM) is the matter that exists in the space between the stars in a galaxy. It is composed of gas, dust, and cosmic rays. The ISM causes extinction and reddening of light from distant stars, which can affect the observed properties of those stars. This is mainly in two ways

- **Absorption**: The radiant energy is absorbed by the ISM and re-radiated in infrared wavelengths (corresponding to the temperature of the ISM particles).
- **Scattering**: The direction of light propagation is changed by the ISM particles, which causes the light to be scattered in different directions. This causes a reduction in the intensity of light reaching the observer.

Assume all dust particles are spheres of radius $a$. The extinction cross section of the particles $C_\text{ext}$ is given by

$$\tag{6.1.1} C_\text{ext} = Q_\text{ext} \pi a^2 $$

where $Q_\text{ext}$ is the extinction efficiency factor, which is a function of the wavelength of light. It can be calculated using rayleigh scattering or mie scattering. If the number density of particles is $n$, the optical depth $\tau$ is given by

$$\tag{6.1.2} d\tau = n \, C_\text{ext} \, dl $$
$$\tag{6.1.3} \tau = \bar{n} \, C_\text{ext} \, L $$

where $dl$ is a small distance in the direction of propagation of light, $L$ is the total distance travelled by light, and $\bar{n}$ is the average number density of particles along the path of light. The optical depth is a measure of the amount of light absorbed or scattered by the ISM. The total extinction $A$ is given by

$$\tag{6.1.4} A = 2.5 \log e\,  \tau \approx 1.09 \, \tau $$

Extinction highly depends on the wavelength of light. Blue light is scattered more than red light. Hence the ISM is also responsible for the reddening of the light of stars.

$$\tag{6.1.5} B-V = (B-V)_0 + E_{B-V} $$
$$\tag{6.1.6} R = \frac{A_V}{E_{B-V}} \approx 3 $$

where $B$ and $V$ are the magnitudes of the star in the blue and visual bands respectively, $(B-V)_0$ is the intrinsic color of the star, $E_{B-V}$ is the color excess, and $R$ is the ratio of total to selective extinction.

Interstellar gas can be detected via the following methods

- **Absorption lines**: The ISM absorbs light from stars, which can be detected as absorption lines in the spectrum of the star. The strength and shape of the absorption lines can provide information about the composition and physical conditions of the ISM.
- **Emission lines**: The ISM can also emit light, which can be detected as emission lines in the spectrum of the ISM. The strength and shape of the emission lines can provide information about the composition and physical conditions of the ISM.
- **Bremsstrahlung radiation**: The ISM can emit bremsstrahlung radiation, which is a type of radiation produced by the acceleration of charged particles. This radiation can be detected in the radio and X-ray wavelengths.
- **21 cm line**: The ISM can emit radiation at a wavelength of 21 cm, which is produced by the hyperfine transition of neutral hydrogen. This radiation can be detected in the radio wavelengths and is used to map the distribution of neutral hydrogen in the ISM.
- **Radio line emission**: The ISM can emit radiation at various wavelengths, which can be detected in the radio wavelengths. This radiation is produced by various processes, including synchrotron radiation and thermal emission from dust.

The 21 cm line is a spectral line that is produced by the hyperfine transition of neutral hydrogen. It is emitted when the spin of the electron and proton in a hydrogen atom are parallel (triplet state) and flips to the state where they are anti-parallel (singlet state). The energy difference between these two states is very small, which corresponds to a wavelength of 21 cm. It is a very important tool for studying the ISM, as it allows astronomers to map the distribution of neutral hydrogen in the ISM.
