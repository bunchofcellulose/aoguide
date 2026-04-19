---
title: Stellar Evolution
weight: 4
---

A star's life is a constant battle between gravity, which wants to compress it, and pressure, which resists. The fuel that sustains pressure is nuclear energy. When the fuel changes or runs out, the star responds: contracting, heating, expanding, changing luminosity and temperature. The **HR diagram** is the observational record of all these phases, and stellar evolution theory is the explanation of why stars trace the paths they do.

## Star Clusters and Stellar Populations

### Clusters as Stellar Laboratories

Stars in a cluster share a common origin (same molecular cloud, same distance, same age, same initial chemical composition) but differ in one key parameter: **initial mass**. This makes clusters ideal for testing stellar evolution theory, because the entire spread of the cluster's HR diagram traces the evolutionary paths of stars of different masses, all born at the same time.

**Open clusters** (a few hundred to a few thousand stars) are found in the galactic disk, are young to middle-aged, and have irregular shapes. Examples: Pleiades (~125 Myr), Hyades (~625 Myr).

**Globular clusters** (tens of thousands to millions of stars) are found in the galactic halo, are among the oldest objects in the universe (~10–13 Gyr), and have high central concentrations. Examples: M13, 47 Tucanae, Omega Centauri.

The **main sequence turnoff point** is the most powerful age-dating tool in astronomy. Massive stars exhaust their hydrogen faster (nuclear timescale $t_\text{nuc} \propto M/L \propto M^{-2.8}$) and evolve off the main sequence first. The color/temperature of the turnoff point — where the main sequence bends upward toward the giant branch — directly indicates the age of the cluster: older clusters have a redder (cooler) turnoff.

{{< callout type="why" >}}
**Why does the main sequence turn off?** 
Stars on the main sequence burn hydrogen in their cores. As hydrogen is consumed, the mean molecular weight $\mu$ increases (4 H → 1 He), so to maintain pressure ($P \propto \rho T / \mu$) the core must either increase in temperature or density. The luminosity rises slowly over the main sequence lifetime. When the core hydrogen is exhausted, the core contracts and the envelope expands — the star moves off the main sequence.

The turnoff luminosity (and hence temperature) scales as: a star leaves the main sequence when its hydrogen fuel is ~10% exhausted, i.e., after time $t \approx 0.1 \, Mc^2 \times 0.007 / L \propto M^{-2.8}$. By setting this equal to the cluster age, we find the turnoff mass and hence turnoff temperature.
{{< /callout >}}

### Stellar Populations

Stars are classified by their chemical composition (metallicity $Z$, the mass fraction of elements heavier than helium) and kinematics:

| Population | Age | Metallicity | Location | Example |
| --- | --- | --- | --- | --- |
| Pop I | Young (<a few Gyr) | Metal-rich ($Z \approx Z_\odot$) | Galactic disk, spiral arms | Sun, Pleiades |
| Pop II | Old (>10 Gyr) | Metal-poor ($Z \ll Z_\odot$) | Galactic halo, bulge, globular clusters | RR Lyrae, globular cluster stars |
| Pop III | $z > 20$ (theoretical) | Metal-free | First galaxies | Not yet directly observed |

Pop III stars are believed to have been very massive ($>100 \, M_\odot$), short-lived, and responsible for the first nucleosynthesis of metals. Their deaths as supernovae enriched the early interstellar medium, enabling Pop II star formation.

## Stellar Timescales

Three timescales govern stellar structure and evolution.

### Dynamical Timescale

The time for pressure waves to cross a star, or equivalently, the free-fall time if pressure support were suddenly removed:

$$\tag{5.1.1} t_\text{dyn} \sim \sqrt{\frac{R^3}{GM}} \sim \frac{1}{\sqrt{G\rho}}$$

For the Sun: $t_\text{dyn} \approx 27$ min. This is also roughly the period of stellar oscillations (pulsating variables have periods $\propto t_\text{dyn}$).

### Kelvin–Helmholtz (Thermal) Timescale

The time to radiate away all gravitational potential energy at the current luminosity. From the virial theorem, the gravitational energy of a star is $\sim GM^2/R$:

$$\tag{5.1.2} t_\text{KH} \sim \frac{GM^2 / R}{L}$$

For the Sun: $t_\text{KH} \approx 1.6 \times 10^7$ yr. This was once thought to be the Sun's age (Kelvin and Helmholtz both proposed gravitational contraction as the Sun's energy source), but it is far too short; fossils and radioactive dating showed a much older Earth.

### Nuclear Timescale

The main-sequence lifetime, during which hydrogen is fused to helium. About 10% of the total hydrogen mass is available in the core, and 0.7% of the rest mass is released as energy in pp-chain fusion:

$$\tag{5.1.3} t_\text{nuc} \sim 0.1 \times 0.007 \times \frac{Mc^2}{L} \approx 7 \times 10^{-4} \frac{ Mc^2}{L}$$

For the Sun: $t_\text{nuc} \approx 10^{10}$ yr. Using $L \propto M^{3.5}$ (mass-luminosity relation):

$$t_\text{nuc} \propto \frac{M}{L} \propto M^{-2.5}$$

A red dwarf of mass $0.3 M_\odot$ thus has a main sequence lifetime of $\sim 10^{11}$ yr, which is more than the current age of the universe.

## The Evolutionary Track: From Cloud to Remnant

### Stage 1: Molecular Cloud and Jeans Instability

Stars form from the gravitational collapse of cold, dense regions within **molecular clouds**: giant complexes of gas and dust (mostly H$_2$) with temperatures ~$10-30$ K and densities ~$10^8-10^{10}$ molecules/m³.

A cloud (or clump within one) will collapse under self-gravity when its gravitational potential energy exceeds its thermal kinetic energy. The **Jeans criterion** gives the critical mass for collapse.

Consider a cloud of mass $M$, radius $R$, temperature $T$, mean molecular mass $\mu$, and density $\rho$. The kinetic and potential energies are:

$$K = \frac{3}{2} N kT = \frac{3kT M}{2\mu m_H}, \qquad U = -\frac{3GM^2}{5R}$$

Collapse occurs when $|U| > 2K$ (virial theorem condition). Setting $|U| = 2K$ gives the **Jeans length** (critical radius):

$$\tag{5.4.1} \lambda_J = \left(\frac{15kT}{4\pi G \mu m_H \rho}\right)^{1/2}$$

and the **Jeans mass** (minimum mass that will collapse):

$$\tag{5.4.2} M_J = \frac{4}{3}\pi \lambda_J^3 \rho = \sqrt{\frac{375}{4\pi}\left(\frac{k}{G\mu m_H}\right)^3 \frac{T^3}{\rho}}$$

{{< callout type="remark" >}}
As a cloud collapses and density increases, $M_J$ falls. This means a collapsing cloud can fragment into smaller and smaller pieces, a process called hierarchical fragmentation, until each fragment is small enough to become opaque to its own radiation. Once opaque, the fragments heat up faster than they radiate, $M_J$ stops falling, and fragmentation halts. This is why molecular clouds form clusters of many stars rather than one giant star.
{{< /callout >}}

### Stage 2: Protostar

As the cloud fragment collapses, gravitational energy is converted to heat. The infalling gas heats up until the central region becomes opaque and pressure builds: a **protostar** forms. The protostar is luminous (powered by Kelvin-Helmholtz contraction), large, and cool. It sits to the upper right of the zero-age main sequence in the HR diagram.

Protostars are typically embedded in their parent molecular cloud, making them optically invisible but detectable in the infrared. The surrounding envelope and disk accrete onto the protostar; bipolar outflows and jets carry away excess angular momentum.

The protostar descends the **Hayashi track**, a nearly vertical path in the HR diagram at roughly constant effective temperature (~4000 K), as the luminosity drops while the star contracts. The Hayashi track represents fully convective stars; stars cannot exist in hydrostatic equilibrium to the right of this track.

Higher-mass stars then transition to nearly horizontal contraction (the **Henyey track**) as their interiors become radiative, before reaching the Zero-Age Main Sequence (ZAMS).

### Stage 3: Zero-Age Main Sequence (ZAMS)

When the core temperature reaches ~$10^7$ K, hydrogen fusion ignites via the **pp chain** (low-mass stars) or the **CNO cycle** (stars above ~$1.3 \, M_\odot$). The luminosity from nuclear reactions replaces the dwindling Kelvin-Helmholtz luminosity, and the star settles into a long-lived equilibrium: the **main sequence**.

The ZAMS is the locus of newly-ignited stars in the HR diagram. More massive stars are hotter and more luminous, giving the main sequence its characteristic slope ($L \propto T^8$ roughly, tracing the mass-luminosity and mass-temperature relations).

Main sequence stars obey:

$$\tag{5.2.1} L \propto M^{3.5}$$

(empirical; exact slope depends on the mass range).

### Stage 4: Main Sequence Evolution

During the main sequence phase, the **core becomes progressively helium-enriched** as hydrogen is consumed. The mean molecular weight $\mu$ increases, requiring higher temperature and density to maintain pressure. This causes a slow increase in luminosity and temperature over the main sequence lifetime: the Sun was only ~70% as luminous 4.6 Gyr ago as it is today.

The main sequence lifetime scales as $t_\text{MS} \propto M/L \propto M^{-2.8}$.

### Stage 5: Subgiant and Red Giant Branch (RGB)

When the **hydrogen in the core is exhausted**, the core (now pure helium) begins to contract (no energy source). By the virial theorem, gravitational contraction heats the core. This elevated temperature ignites hydrogen in a **shell** around the inert helium core.

The shell burning drives the **envelope to expand and cool**, dramatically increasing the stellar radius. The star moves off the main sequence toward the upper right of the HR diagram — the **subgiant branch** (nearly horizontal at first, then steeply rising in luminosity), then onto the **red giant branch (RGB)**. A $1 \, M_\odot$ star expands to ~100–200 $R_\odot$ on the RGB.

{{< callout type="why" >}}
**Why does the envelope expand when the core contracts?** This is the **mirror principle** (also called the virial mirror). In a shell-burning star, the shell is sandwiched between the contracting core and the expanding envelope. As the core contracts and the shell temperature rises, the shell burns more vigorously, depositing more energy into the envelope. By virial theorem arguments, the envelope cannot absorb this energy without expanding. The star's total luminosity rises sharply on the RGB because the shell burning grows more vigorous as the core contracts and the shell gets hotter.
{{< /callout >}}

On the RGB, the outer convective envelope deepens and dredges helium and CNO-processed material up to the surface. This **first dredge-up** changes the surface abundances of carbon, nitrogen, and oxygen isotopes.

### Stage 6: Helium Flash and Horizontal Branch

The helium core contracts until it becomes **electron-degenerate** (in stars $\lesssim 2 \, M_\odot$). A degenerate gas has pressure independent of temperature. When the core temperature reaches ~$10^8$ K, **helium ignites** to form carbon via the triple-alpha process:

$$3 \, {}^4\text{He} \rightarrow {}^{12}\text{C} + \gamma$$

But because the pressure does not increase with temperature, the fusion is **thermally unstable**: burning heats the core, which burns faster, which heats more: a runaway reaction called the **helium flash**. This deposits $\sim 10^{11} \, L_\odot$ of power in the core in seconds, but almost none reaches the surface (it goes into expanding and lifting the degeneracy).

After the flash, the core is non-degenerate and helium burning continues stably. The star settles on the **horizontal branch (HB)** of the HR diagram, roughly constant luminosity, at a temperature depending on the envelope mass lost on the RGB (a function of metallicity and other factors).

In more massive stars ($\gtrsim 2 \, M_\odot$), the helium core is never degenerate and ignites smoothly.

### Stage 7: Asymptotic Giant Branch (AGB)

When the **core helium is exhausted**, the star now has an inert **carbon-oxygen (C/O) core** with a helium-burning shell and a hydrogen-burning shell around it. The star again expands enormously, ascending the **asymptotic giant branch (AGB)**, which runs roughly parallel to and slightly to the right of the RGB.

AGB stars develop a powerful **stellar wind** (driven by radiation pressure on dust grains) that removes the envelope at rates $10^{-8}-10^{-4} \, M_\odot$/yr. The AGB is also characterized by **thermal pulses**: periodic ignition of helium in the shell, which drives convective mixing (**third dredge-up**) that brings freshly synthesized carbon and s-process elements to the surface, producing carbon stars and s-process enriched stars.

### Stage 8: Fate — Planetary Nebula + White Dwarf or Core Collapse

**For stars $\lesssim 8 \, M_\odot$**: The envelope is eventually completely ejected as a **planetary nebula**, a beautiful shell of ionized gas illuminated by the hot remnant stellar core. The core, now exposed as a C/O **white dwarf** of $\sim 0.5-1.0 \, M_\odot$, gradually cools over billions of years. White dwarfs are supported by electron degeneracy pressure and have no fusion; they simply radiate stored heat.

**For stars $\gtrsim 8 \, M_\odot$**: The core grows through successive fusion stages, C, Ne, O, Si, each faster than the last (Si burning lasts just few days). Finally, an **iron core** forms (iron cannot be fused exothermically). When the iron core exceeds the Chandrasekhar mass ($\sim 1.4 \, M_\odot$), electron degeneracy pressure is overcome, and the core collapses in milliseconds to a **neutron star** (or black hole for the most massive cases). The collapse rebounds as a **core-collapse supernova** (Types II, Ib, Ic), ejecting the outer layers at $\sim 10^{44}$ J of kinetic energy.

{{< callout type="remark" >}}
**Summary of evolutionary fates by initial mass:**

| Initial mass | Final remnant | Mechanism |
| --- | --- | --- |
| $< 0.08 \, M_\odot$ | Brown dwarf | Never ignites H |
| $0.08$–$0.5 \, M_\odot$ | Helium white dwarf | No He flash |
| $0.5$–$8 \, M_\odot$ | C/O white dwarf | AGB + planetary nebula |
| $8$–$20 \, M_\odot$ | Neutron star | Core-collapse SN (Type II) |
| $> 20 \, M_\odot$ | Black hole (or NS) | Core-collapse SN; massive mass loss |
| $> 100 \, M_\odot$ | Pair-instability SN or direct collapse | Exotic paths |

{{< /callout >}}

## Strömgren Sphere

A newly formed hot, massive star (O or B type) embedded in a uniform neutral hydrogen medium ionizes the surrounding gas out to a well-defined boundary called the **Strömgren sphere**. Outside it, the UV flux is insufficient to maintain ionization; inside it, hydrogen is nearly fully ionized.

The star produces ionizing photons (with $h\nu > 13.6 \, \mathrm{eV}$) at a rate:

$$\tag{5.4.3} Q_* = \int_{\nu_0}^{\infty} \frac{L_\nu}{h\nu} \, d\nu$$

In equilibrium, the ionization rate equals the recombination rate within the sphere of radius $R_S$:

$$\tag{5.4.8} Q_* = n_e^2 \, \alpha(T_e) \, \frac{4}{3}\pi R_S^3$$

where $\alpha(T_e) = \langle \sigma_\text{rec} v_e \rangle \propto T_e^{-1/2}$ is the recombination coefficient and $n_e$ is the electron number density (= proton density for fully ionized hydrogen).

Solving for the **Strömgren radius**:

$$\tag{5.4.9} \boxed{R_S = \left(\frac{3Q_*}{4\pi n_e^2 \, \alpha(T_e)}\right)^{1/3} \propto Q_*^{1/3} n_e^{-2/3} T_e^{1/6}}$$

{{< callout type="remark" >}}
The thickness of the ionization boundary is ~one recombination mean free path: $\ell \sim 1/(n_e \sigma_\text{rec})$. For typical HII region densities ($n_e \sim 10^7$ m$^{-3}$), this is much smaller than $R_S$, so the sharp boundary is an excellent approximation.

A typical O5 star has $Q_* \sim 10^{49}$ ionizing photons/s, and with $n_e \sim 10^8$ m$^{-3}$, gives $R_S \sim 10$ pc. These ionized HII regions are beautiful, observable as emission nebulae (Orion Nebula, Eagle Nebula, etc.).
{{< /callout >}}
