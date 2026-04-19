---
title: Our Universe
weight: 1
prev: /guide/cosmology/
---

The universe is everything that exists — all matter, energy, space, and time. Studying it requires us to confront questions about its origin, geometry, composition, and fate. Before we can do any of that, we need a few observational and philosophical foundations.

## The Cosmological Principle

The cosmological principle is the foundational assumption of modern cosmology: **the universe is homogeneous and isotropic on sufficiently large scales** (above ~100 Mpc).

- **Homogeneous**: Every point in space looks the same as every other. There are no special locations.
- **Isotropic**: Space looks the same in every direction. There are no preferred axes.

{{< callout type="remark" >}}
These two properties are independent. A dartboard is isotropic when viewed from the center, but not homogeneous — the center is a special point. An infinite striped pattern is homogeneous (you can shift along a stripe and nothing changes) but not isotropic — the stripes pick out a preferred direction. The cosmological principle requires both simultaneously.
{{< /callout >}}

{{< callout type="why" >}}
Why do we assume this? On small scales it is obviously false — you are denser than the void between galaxy clusters. But galaxy surveys (SDSS, DES) show that when you average over scales larger than ~100 Mpc, the universe does look statistically uniform. The cosmological principle also has philosophical justification: it is the assumption that we do not live at a special location in the universe, called the Copernican principle.
{{< /callout >}}

## Olbers' Paradox

If the universe were infinite, static, and uniformly filled with stars, then **every line of sight would eventually terminate on the surface of a star**, and the night sky would be as bright as the surface of the Sun. But the sky is dark. This is Olbers' paradox.

{{< callout type="remark" >}}
One might guess that dust absorbs the light. But in an infinite, eternal universe, the dust would simply heat up until it re-radiates at the same temperature — so the paradox remains.

The resolution is that the universe is **neither infinitely old nor static**. Because light travels at a finite speed, we can only see out to the **cosmic horizon** — the distance light has traveled since the Big Bang, roughly 46 billion light-years (the observable universe). Stars beyond the horizon are causally disconnected from us. Additionally, because the universe is expanding, light from distant galaxies is redshifted to lower energies, further dimming them.
{{< /callout >}}

## Hubble–Lemaître Law

In 1929, Edwin Hubble (building on Lemaître's theoretical work) published observations showing that **galaxy recession velocity is proportional to distance**:

$$\tag{7.1.1} \boxed{v = H_0 \, d}$$

where $H_0$ is the **Hubble constant**, currently measured at $H_0 \approx 67$–$73 \, \mathrm{km \, s^{-1} \, Mpc^{-1}}$ (the exact value is under active debate — the **Hubble tension**).

{{< callout type="why" >}}
This is not galaxies moving *through* space — it is space itself expanding. An analogy: draw dots on a balloon and inflate it. Every dot sees every other dot receding, with recession speed proportional to separation. There is no center of expansion; every point is equivalent.

The Hubble law follows naturally from a homogeneous, expanding universe described by the scale factor $a(t)$ (discussed in Friedmann Equations). If physical distance is $d = a \, \chi$ where $\chi$ is the comoving coordinate, then

$$\dot{d} = \dot{a} \, \chi = \frac{\dot{a}}{a} \, d = H \, d$$

So Hubble's Law is a direct consequence of uniform expansion.
{{< /callout >}}

The Hubble time $t_H = H_0^{-1}$ gives a rough estimate of the age of the universe:

$$\tag{7.1.2} t_H = \frac{1}{H_0} \approx 14.4 \, \mathrm{Gyr}$$

This is the age the universe would have if it had been expanding at a constant rate. The true age (~13.8 Gyr) is close because the deceleration due to matter and the acceleration due to dark energy partially cancel.

## Redshift

When a source of light moves away from us, the wavelength of the emitted light is stretched. **Redshift** is defined as

$$\tag{7.1.3} \boxed{z = \frac{\lambda_\text{obs} - \lambda_\text{emit}}{\lambda_\text{emit}}}$$

A positive $z$ means the source is receding; $z = 0$ means no relative motion; a negative $z$ (blueshift) means the source is approaching.

Three distinct physical effects produce redshift in astronomy:

- **Doppler redshift**: From the peculiar velocity of the source. For non-relativistic speeds, $v = cz$. Relativistically, $1 + z = \sqrt{(1 + v/c)/(1 - v/c)}$.
- **Cosmological redshift**: From the expansion of space stretching photon wavelengths during travel. This is related to the scale factor by $1 + z = a_0 / a_\text{emit}$, where $a_0$ is the scale factor today.
- **Gravitational redshift**: From photons climbing out of a gravitational well. Derived from GR: $1 + z = 1/\sqrt{1 - r_s/r}$.

{{< callout type="remark" >}}
In practice, the total observed redshift is a combination of all three. For cosmological sources, the dominant contribution is cosmological redshift. For nearby objects (within the Local Group), peculiar velocities dominate, and Hubble's law cannot be applied directly.

Combining Hubble's law with the non-relativistic Doppler formula gives $z \approx H_0 d / c$, valid at low redshifts ($z \ll 1$). At high redshifts this breaks down and the full cosmological framework (FLRW metric, Friedmann equations) is required.
{{< /callout >}}

{{< tabs >}}
    {{< tab name="Q1" >}}
    A galaxy is observed to have a redshift of $z = 0.05$. Using Hubble's law with $H_0 = 70 \, \mathrm{km\,s^{-1}\,Mpc^{-1}}$, estimate its distance. Is the non-relativistic approximation valid here?
    {{< /tab >}}

    {{< tab name="Solution" >}}
    The recession velocity is $v = cz = 3 \times 10^5 \times 0.05 = 15000 \, \mathrm{km\,s^{-1}}$.

    From Hubble's law:

    $$d = \frac{v}{H_0} = \frac{15000}{70} \approx 214 \, \mathrm{Mpc}$$

    Since $v/c = 0.05 \ll 1$, the non-relativistic approximation is valid. The relativistic correction would be less than 0.25%.
    {{< /tab >}}
{{< /tabs >}}

## Cosmic Microwave Background Radiation

In 1948, Gamow, Alpher, and Herman predicted that the hot, dense early universe should have left behind a **relic radiation field** filling all of space. In 1965, Penzias and Wilson accidentally discovered this radiation — the **Cosmic Microwave Background (CMB)** — as an isotropic noise signal in their radio antenna.

{{< callout type="person" >}}
Penzias and Wilson initially thought the persistent noise in their antenna was due to pigeon droppings. After cleaning the antenna repeatedly and still finding the signal, they contacted Robert Dicke at Princeton, who immediately recognized what they had found. Penzias and Wilson received the 1978 Nobel Prize in Physics for the discovery.
{{< /callout >}}

The CMB is the thermal radiation from the epoch of **recombination** (~380,000 years after the Big Bang), when the universe cooled enough (~3000 K) for protons and electrons to combine into neutral hydrogen. The universe became transparent to photons at this point. Since then, the expansion of the universe has cooled and redshifted this radiation to its present temperature:

$$T_0 = 2.7255 \pm 0.0006 \, \mathrm{K}$$

The CMB has the most perfect blackbody spectrum ever measured. Its energy density and photon number density follow directly from the blackbody formulas derived in the Radiometry section:

$$\tag{7.1.4} u_0 = aT_0^4 \approx 4.17 \times 10^{-14} \, \mathrm{J\,m^{-3}} \approx 0.260 \, \mathrm{eV\,cm^{-3}}$$

$$\tag{7.1.5} n_0 = \beta T_0^3 \approx 411 \times 10^6 \, \mathrm{m^{-3}}$$

where $a = 4\sigma/c$ is the radiation constant and $\beta \approx 2.03 \times 10^7 \, \mathrm{m^{-3}\,K^{-3}}$ (both derived in Radiometry, eq. 2.1.31 and 2.1.33).

{{< callout type="remark" >}}
The CMB temperature scales with the scale factor as $T \propto 1/a$. This is a direct consequence of cosmological redshift — as the universe expands by a factor $a$, photon wavelengths stretch by the same factor, and since $\lambda_\text{peak} \propto 1/T$ (Wien's law), the temperature falls as $1/a$. At recombination, $z \approx 1100$, so $T_\text{rec} = T_0 (1 + z) \approx 3000 \, \mathrm{K}$.
{{< /callout >}}

Small temperature anisotropies in the CMB ($\delta T / T \sim 10^{-5}$) encode a snapshot of the density fluctuations in the early universe that seeded all large-scale structure (galaxies, clusters, filaments) we see today.

{{< tabs >}}
    {{< tab name="Q2" >}}
    The CMB has a temperature of $T_0 = 2.73 \, \mathrm{K}$. (a) At what wavelength does the CMB peak? (b) What was the temperature of the CMB when the universe was half its current size?
    {{< /tab >}}

    {{< tab name="Solution" >}}
    **(a)** Using Wien's displacement law:

    $$\lambda_\text{peak} = \frac{b_\lambda}{T_0} = \frac{2.898 \times 10^{-3}}{2.73} \approx 1.06 \, \mathrm{mm}$$

    This is in the microwave band, which is why this radiation is called the Cosmic Microwave Background.

    **(b)** If the universe was half its current size, the scale factor was $a = a_0/2$, corresponding to $z = 1$. Since $T \propto 1/a$:

    $$T = T_0 \times \frac{a_0}{a} = 2.73 \times 2 = 5.46 \, \mathrm{K}$$
    {{< /tab >}}
{{< /tabs >}}

## Big Bang Nucleosynthesis

In the first few minutes after the Big Bang, the universe was hot and dense enough for nuclear reactions to occur. This period is called **Big Bang Nucleosynthesis (BBN)**, and it produced the lightest elements in the universe.

The primordial abundances predicted by BBN are:

- ~75% hydrogen (by mass)
- ~25% helium-4 (by mass)
- Trace amounts of deuterium, helium-3, and lithium-7

These predictions agree extraordinarily well with observations of the oldest, least-processed astrophysical objects. The 25% helium fraction is a key observational pillar of Big Bang cosmology — stellar nucleosynthesis alone cannot produce this much helium.

{{< callout type="why" >}}
Why does BBN stop at helium? As the universe expanded and cooled below $\sim 0.1 \, \mathrm{MeV}$ (~$10^9$ K), the thermal photons could no longer dissociate helium nuclei, but the density had already dropped too low for reactions to proceed to carbon or heavier elements. The triple-alpha process (helium to carbon) requires the high densities found in stellar cores. BBN is thus a snapshot of nuclear physics at $t \sim 3$–$20$ minutes.
{{< /callout >}}

## The Composition of the Universe

Modern cosmological observations (CMB, BAO, supernovae) indicate the universe is composed of:

| Component | Fraction | Description |
| --- | --- | --- |
| Baryonic matter | ~5% | Ordinary atoms — all stars, gas, planets |
| Dark matter | ~27% | Non-baryonic, non-luminous; inferred gravitationally |
| Dark energy | ~68% | Responsible for accelerated expansion; nature unknown |

{{< callout type="remark" >}}
The term "dark matter" does not mean we know what it is — only that there is more gravitational mass than luminous mass, observed consistently in galaxy rotation curves, cluster dynamics, and gravitational lensing. Similarly, "dark energy" is a placeholder for whatever is causing the accelerated expansion discovered in 1998 from Type Ia supernovae observations (Perlmutter, Riess, Schmidt — 2011 Nobel Prize).
{{< /callout >}}

{{< tabs >}}
    {{< tab name="Q3" >}}
    The critical density of the universe today is $\rho_c = \frac{3H_0^2}{8\pi G} \approx 9.47 \times 10^{-27} \, \mathrm{kg\,m^{-3}}$ for $H_0 = 68 \, \mathrm{km\,s^{-1}\,Mpc^{-1}}$. If baryonic matter makes up 5% of the critical density, what is the mean number density of baryons in the universe? (Take the baryon mass $\approx m_p$.)
    {{< /tab >}}

    {{< tab name="Solution" >}}
    The baryonic matter density is:

    $$\rho_b = 0.05 \, \rho_c \approx 4.74 \times 10^{-28} \, \mathrm{kg\,m^{-3}}$$

    The number density of baryons is:

    $$n_b = \frac{\rho_b}{m_p} = \frac{4.74 \times 10^{-28}}{1.67 \times 10^{-27}} \approx 0.28 \, \mathrm{m^{-3}}$$

    So on average, there is less than one baryon per cubic meter in the universe. Compare this to the $\sim 411$ CMB photons per cubic meter — photons outnumber baryons by a factor of ~$10^9$. This ratio is the **baryon-to-photon ratio** $\eta \sim 6 \times 10^{-10}$, a fundamental parameter of cosmology.
    {{< /tab >}}
{{< /tabs >}}
