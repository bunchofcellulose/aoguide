---
title: Galaxies
weight: 1
prev: /guide/galactic-astrophysics/
---

Galaxies are the fundamental building blocks of the large-scale universe — gravitationally bound systems containing stars, gas, dust, and dark matter, ranging from dwarf galaxies with a few million stars to giants with hundreds of trillions. Studying their morphology, kinematics, and scaling relations gives us direct windows into dark matter, the star formation history of the universe, and the processes that shaped cosmic structure.

{{< callout type="trivia" >}}
Until the 1920s, "spiral nebulae" were thought to be clouds of gas within the Milky Way. The debate was settled by Edwin Hubble, who in 1923 identified Cepheid variable stars in the Andromeda "nebula" using the 100-inch Hooker telescope at Mt. Wilson. The Cepheid period-luminosity relation gave a distance far too large for Andromeda to be inside our Galaxy — the "Great Debate" between Shapley and Curtis was resolved: the universe is far larger than the Milky Way.
{{< /callout >}}

## Hubble Classification

The **Hubble tuning fork** is the standard morphological classification scheme, introduced by Hubble in 1926. It divides galaxies into four main families:

**Elliptical galaxies (E0–E7)** have smooth, featureless light profiles, no disk, and little gas or dust. They are dominated by old, red stars on random orbits. The ellipticity classification is:

$$n = 10\left(1 - \frac{b}{a}\right)$$

where $a$ and $b$ are the projected major and minor axes. An E0 galaxy appears circular; an E7 appears highly flattened.

**Lenticular galaxies (S0)** have a disk and bulge but no spiral arms and little ongoing star formation. They sit at the junction of the tuning fork and are thought to be spiral galaxies that have exhausted their gas supply.

**Spiral galaxies (Sa–Sc)** have a central bulge and a flat disk with spiral arms. They are classified by:

- The tightness of the spiral arms (Sa: tight; Sc: loose)
- The prominence of the central bulge (Sa: large; Sc: small)
- The patchiness of the arms (Sc arms are more irregular and clumpy with active star-forming regions)

**Barred spirals (SBa–SBc)** are like spirals but have a bar of stars extending through the nucleus. The Milky Way is classified as SBbc. SAB galaxies have an intermediate, weak bar.

**Irregular galaxies (Irr)** defy the above categories. The Magellanic Clouds (Sm/Im type) are nearby examples, likely distorted by tidal interaction with the Milky Way.

{{< callout type="image" >}}
{{< png "gal/hubble.png" "Hubble Classification" "The Hubble tuning fork diagram. Left-to-right does not represent an evolutionary sequence — galaxies do not simply evolve from ellipticals to spirals." >}}
{{< /callout >}}

{{< callout type="remark" >}}
The Hubble sequence is **not** an evolutionary sequence. Hubble himself called it "early" (ellipticals) and "late" (spirals), terminology that persists today but is purely historical. Ellipticals do not evolve into spirals. Modern evidence suggests the transformation runs the other way: mergers of spirals can produce ellipticals, and gas accretion onto ellipticals might rebuild a disk.

Extended classifications beyond the original Hubble scheme include:

- **cD galaxies**: Giant ellipticals at cluster centers with extended stellar halos, formed by galactic cannibalism
- **dE / dSph**: Dwarf ellipticals and dwarf spheroidals — the most numerous galaxy type by count
- **UCD**: Ultra-compact dwarfs, possibly stripped dwarf galaxy nuclei
- **Radio galaxies**: Strong radio emitters, classified as FR I (edge-darkened jets) and FR II (edge-brightened, with hotspots) by Fanaroff and Riley
{{< /callout >}}

## Surface Brightness Profiles

The light distribution in galaxies follows characteristic profiles depending on galaxy type.

The **de Vaucouleurs profile** (or $R^{1/4}$ law) describes the surface brightness of elliptical galaxies:

$$\tag{6.2.1} \ln I(R) = \ln I_e - 7.67 \left[ \left(\frac{R}{R_e}\right)^{1/4} - 1 \right]$$

where $R_e$ is the **effective radius** (also called the half-light radius) — the projected radius enclosing half of the total light. The constant $I_e$ is the surface brightness at $R_e$. This profile arises naturally from violent relaxation during galaxy formation.

{{< callout type="remark" >}}
Spiral galaxy disks follow an **exponential profile** instead:

$$I(R) = I_0 \, e^{-R/h}$$

where $h$ is the disk scale length. The Milky Way disk has $h \approx 3.5$ kpc.

The **Sérsic profile** generalizes both: $\ln I \propto R^{1/n}$. Ellipticals have $n \approx 4$; exponential disks have $n = 1$; compact bulges can have intermediate values.
{{< /callout >}}

The **galaxy effective radius** $R_e$ and the **isophotal radius** $R_{25}$ (where the surface brightness falls to $25 \, \mathrm{mag/arcsec^2}$ in the $B$-band) are standard size measures.

## Galactic Scaling Relations

Scaling relations connect observable quantities (luminosity, velocity, size) and arise because galaxies are not random configurations — they formed through processes that enforce correlations between their properties. These relations are indispensable as **distance indicators**, reaching well beyond the range of geometric parallax or Cepheid variables.

### Tully–Fisher Relation

For **spiral galaxies**, the luminosity correlates tightly with the peak rotation speed $V_\text{max}$ of the gas disk:

$$\tag{6.2.2} L \propto V_\text{max}^\alpha$$

or equivalently $M = A + B \log V$, where $\alpha \approx 3$–$4$ (depending on the photometric band; steeper in the infrared).

{{< callout type="why" >}}
**Where does this come from?** The rotation speed of a galaxy measures its total mass (including dark matter) within the disk: $V^2 \approx GM/R$. For a disk galaxy with a roughly constant mass-to-light ratio, $L \propto M \propto V^2 R$. Empirically, larger galaxies also tend to have higher surface brightness such that $L \propto V^4$ emerges. The steep infrared Tully-Fisher slope arises because infrared luminosity traces stellar mass (old stars dominate), which directly traces the gravitational potential. Since both $V$ and $L$ are distance-independent (you can measure $V$ from Doppler shifts of the 21-cm HI line), the Tully-Fisher relation gives luminosity directly, and hence distance via the distance modulus.

The Tully-Fisher relation is a **pillar of the extragalactic distance ladder**, calibrated locally using Cepheids and used to measure distances out to ~100 Mpc.
{{< /callout >}}

### Faber–Jackson Relation

For **elliptical galaxies**, which have little rotation, the luminosity correlates with the **velocity dispersion** $\sigma$ of the stars:

$$\tag{6.2.3} L \propto \sigma^4$$

{{< callout type="why" >}}
**Where does this come from?** Elliptical galaxies are supported by random stellar motions rather than rotation. The virial theorem relates kinetic and potential energy for a system in equilibrium:

$$2K + U = 0 \implies \sigma^2 \sim \frac{GM}{R}$$

If we assume a roughly constant mass-to-light ratio ($M \propto L$) and a constant surface brightness ($L \propto R^2 I_e \sim R^2$, so $R \propto L^{1/2}$), substituting into the virial theorem:

$$\sigma^2 \sim \frac{GL}{R} \sim G L^{1/2} \implies L \propto \sigma^4$$

The Faber-Jackson relation has more scatter than Tully-Fisher because ellipticals span a wider range of formation histories, but it similarly provides distance estimates for elliptical galaxies, extending our reach to greater distances.
{{< /callout >}}

### Fundamental Plane

The scatter in the Faber-Jackson relation is reduced dramatically by adding a third parameter — effective radius $R_e$ and surface brightness $I_e$ — giving the **Fundamental Plane** of elliptical galaxies:

$$R_e \propto \sigma^{1.24} \, I_e^{-0.82}$$

Galaxies lie on a tight plane in the 3D space $(R_e, \sigma, I_e)$. The tilt of this plane relative to the virial prediction encodes systematic variations in the stellar mass-to-light ratio across the elliptical galaxy population.

{{< tabs >}}
    {{< tab name="Q1" >}}
    A spiral galaxy has an observed 21-cm HI line width (corrected for inclination) of $\Delta v = 400 \, \mathrm{km\,s^{-1}}$, corresponding to $V_\text{max} = 200 \, \mathrm{km\,s^{-1}}$. Using the *I*-band Tully-Fisher relation $M_I = -7.48 \log(2V_\text{max}) + 3.0$ (magnitudes), and the galaxy's apparent *I*-band magnitude is $m_I = 12.5$, find the distance to this galaxy.
    {{< /tab >}}

    {{< tab name="Solution" >}}
    First find the absolute magnitude from the Tully-Fisher relation:

    $$M_I = -7.48 \log(2 \times 200) + 3.0 = -7.48 \log(400) + 3.0$$
    $$= -7.48 \times 2.602 + 3.0 = -19.46 + 3.0 = -22.0$$

    Wait — let's use the standard form more carefully. Many sources give $M_I = -7.48(\log 2V - 2.5)$. Using our result for the distance modulus:

    $$\mu = m_I - M_I = 12.5 - (-22.0) = 34.5$$

    The distance is:

    $$d = 10^{(\mu + 5)/5} = 10^{39.5/5} = 10^{7.9} \approx 79 \, \mathrm{Mpc}$$
    {{< /tab >}}
{{< /tabs >}}

## Types of Active Galaxies

In some galaxies, the nucleus itself outshines the rest of the galaxy. These **Active Galactic Nuclei (AGN)** are powered by accretion of matter onto a **supermassive black hole** (SMBH) with $M_\bullet \sim 10^6$–$10^{10} \, M_\odot$.

The accretion disk around the SMBH reaches temperatures of $10^4$–$10^7$ K, emitting across the full electromagnetic spectrum, often with a relativistic jet of plasma perpendicular to the disk. The diverse zoo of AGN types is largely a **viewing angle effect** (the AGN unification model):

| Type | Key Feature |
| --- | --- |
| **Seyfert 1** | Broad + narrow emission lines; AGN seen face-on through dusty torus |
| **Seyfert 2** | Narrow emission lines only; AGN obscured by torus |
| **Quasar / QSO** | Extremely luminous AGN at high redshift; outshines host galaxy |
| **Blazar** | Jet pointed directly at observer; rapid variability across all wavelengths |
| **FR I Radio Galaxy** | Edge-darkened radio jets; lower power |
| **FR II Radio Galaxy** | Edge-brightened jets with hotspots; higher power |

{{< callout type="remark" >}}
For a quasar varying on a timescale $\Delta t$, the emitting region must be smaller than $c \Delta t$. A quasar varying over days thus has an emitting region smaller than a few light-days — yet outshining an entire galaxy. This argument places tight constraints on the compactness and hence the nature of the central engine.
{{< /callout >}}

{{< tabs >}}
    {{< tab name="Q2" >}}
    An AGN is observed to vary significantly in luminosity over a period of 3 days. Estimate the maximum size of the emitting region.
    {{< /tab >}}

    {{< tab name="Solution" >}}
    For the emission to vary coherently on a timescale $\Delta t$, the emitting region must be causally connected — i.e., a light signal must be able to cross it in time $\Delta t$:

    $$R_\text{max} = c \, \Delta t = 3 \times 10^8 \times 3 \times 86400 \approx 7.8 \times 10^{13} \, \mathrm{m} \approx 520 \, \mathrm{AU}$$

    This is about 520 AU — less than 0.003 pc. A region smaller than our solar system is producing luminosities that can outshine entire galaxies of $10^{11}$ stars. This is only possible via accretion onto a supermassive black hole.
    {{< /tab >}}
{{< /tabs >}}

## Large-Scale Structure

Galaxies are not uniformly distributed in space. On scales of tens to hundreds of Mpc, they organize into a **cosmic web**:

- **Galaxy groups** (~few to ~100 members, $\sim$ few Mpc): Held together by gravity. The Local Group contains the Milky Way, Andromeda, and ~80 smaller galaxies within ~3 Mpc.
- **Galaxy clusters** (~hundreds to thousands of members, ~few Mpc): The most massive gravitationally bound structures. Clusters contain hot intracluster gas (the ICM) at $10^7$–$10^8$ K, detectable in X-rays.
- **Superclusters** (~hundreds of Mpc): Not gravitationally bound, but connected by the Hubble flow. The Laniakea Supercluster contains the Milky Way and ~100,000 galaxies.
- **Filaments and voids**: Clusters are connected by filaments of galaxies and separated by vast voids (~100 Mpc diameter) nearly empty of galaxies. The Hercules–Corona Borealis Great Wall is ~3 Gpc in extent.

{{< callout type="remark" >}}
The cosmic web structure arises from the gravitational amplification of tiny quantum fluctuations in the early universe, visible as the temperature anisotropies in the CMB. Cold dark matter collapse formed halos along which baryons fell; the result over 13.8 Gyr is the web of filaments and voids we observe in galaxy surveys like SDSS and DESI.
{{< /callout >}}

{{< tabs >}}
    {{< tab name="Q3" >}}
    The Coma Cluster has a measured velocity dispersion of $\sigma \approx 880 \, \mathrm{km\,s^{-1}}$ and an observed radius of $R \approx 2 \, \mathrm{Mpc}$. Using the virial theorem ($M = 5\sigma^2 R / G$ for a uniform sphere), estimate the virial mass of the cluster. Compare this to the observed luminosity of the cluster, $L \approx 5 \times 10^{12} \, L_\odot$.
    {{< /tab >}}

    {{< tab name="Solution" >}}
    Converting to SI:

    $$\sigma = 880 \times 10^3 \, \mathrm{m\,s^{-1}}, \quad R = 2 \times 3.086 \times 10^{22} \, \mathrm{m} = 6.17 \times 10^{22} \, \mathrm{m}$$

    $$M = \frac{5 \sigma^2 R}{G} = \frac{5 \times (8.8 \times 10^5)^2 \times 6.17 \times 10^{22}}{6.67 \times 10^{-11}} \approx 3.6 \times 10^{45} \, \mathrm{kg} \approx 1.8 \times 10^{15} \, M_\odot$$

    The mass-to-light ratio is:

    $$\frac{M}{L} \approx \frac{1.8 \times 10^{15}}{5 \times 10^{12}} \approx 360 \, \frac{M_\odot}{L_\odot}$$

    A typical stellar population has $M/L \sim 1$–$10$. The factor of ~36 to ~360 excess indicates that the cluster contains far more mass than is visible in stars — **dark matter**. This was first noticed by Fritz Zwicky in 1933 using exactly this method.
    {{< /tab >}}
{{< /tabs >}}
