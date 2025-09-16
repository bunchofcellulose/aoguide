---
title: The Friedmann Equations
weight: 4
---

## The Friedmann Equation

The equation governing the expansion of the universe is the Friedmann equation:

$$\tag{5.4.1} \boxed{\left( \frac{\dot{a}}{a} \right)^2 = \frac{8\pi G}{3 c^2} \varepsilon (t) - \frac{\kappa c^2}{R_0^2} \frac{1}{a(t)^2}}$$

Here we have the scale factor $a(t)$, the curvature $\kappa$, the current radius of curvature $R_0$, and the energy density $\varepsilon(t)$.

The Friedmann equation is derived from the Einstein field equations of general relativity, which describe how matter and energy in the universe influence its geometry. However, it can be approximately derived from Newtonian physics by considering a homogeneous and isotropic universe.

The Hubble parameter $H(t)$ is defined as

$$\tag{5.4.2} \boxed{H(t) = \frac{\dot{a}}{a}}$$

The present value of the Hubble parameter (at $t = t_0$) is called the Hubble constant $H_0$, and is approximately equal to $70 \, \text{km/s/Mpc}$.

We define the critical energy density $\varepsilon_\text{c}$ as the energy density of a flat universe ($\kappa = 0$). It is equal to

$$\tag{5.4.3} \varepsilon_\text{c}(t) = \frac{3 H(t)^2}{8 \pi G}$$

The current observed value of the critical energy density is $\varepsilon_{\text{c},0} \approx 5.2 \mathrm{\,GeV\,m^{-3}}$.

The density parameter $\Omega(t)$ is defined as

$$\tag{5.4.4} \Omega(t) = \frac{\varepsilon(t)}{\varepsilon_\text{c}(t)}$$

{{< callout type="remark" >}}
Using this, the Friedmann equation can be rewritten as

$$ 1 - \Omega(t) = -\frac{\kappa c^2}{R_0^2 a(t)^2 H(t)^2} $$

The RHS can't change its sign since $\kappa$ is a constant, hence if $\Omega$ was less than 1 at some time, it will always be less than 1. From this relation, we also get that by measuring $H_0$ and $\Omega_0$, we can find $\kappa$ and $R \: (= a(t)\, R_0)$.

From this, we can also infer that for a flat universe ($\kappa = 0$), $\Omega(t) = 1 \implies \varepsilon(t) = \varepsilon_\text{c}(t)$; for a positively curved universe ($\kappa = +1$), $\Omega(t) > 1 \implies \varepsilon(t) > \varepsilon_\text{c}(t)$; and for a negatively curved universe ($\kappa = -1$), $\Omega(t) < 1 \implies \varepsilon(t) < \varepsilon_\text{c}(t)$.
{{< /callout >}}

To simplify the notation, we introduce the density parameter related to the curvature $\Omega_\kappa(t)$ as

$$\tag{5.4.5} \Omega_\kappa(t) = -\frac{\kappa c^2}{R_0^2 \, a(t)^2 \, H(t)^2}$$

Then we can rewrite the Friedmann equation as

$$\tag{5.4.6} \Omega(t) + \Omega_\kappa(t) = 1$$

The sum of all the density parameters in the universe is equal to 1 at all times.

## Fluid and Acceleration Equation

The universe can be modelled as a perfect fluid, one which is incompressible and has no viscosity. Thus it can be described by the fluid equation, which is

$$\tag{5.4.7} \boxed{\dot{\varepsilon} + 3 \frac{\dot{a}}{a} (\varepsilon + P) = 0}$$

where $P$ is the pressure of the fluid, associated with the material filling the universe. This can be derived from thermodynamics, and is a consequence of the conservation of energy and momentum in a homogeneous and isotropic universe.

The acceleration equation is

$$\tag{5.4.8} \boxed{\frac{\ddot{a}}{a} = -\frac{4 \pi G}{3c^2} (\varepsilon + 3P)}$$

All matter has positive pressure and hence causes the rate of expansion to slow down. However, if the pressure is negative, it can cause the expansion to accelerate. This is the case for dark energy, which has a negative pressure and is responsible for the observed acceleration of the universe's expansion. One of the models of dark energy is the cosmological constant $\Lambda$, which is a constant energy density filling space homogeneously.

## Equation of State

An equation of state is a mathematical relation between the pressure and the energy density of the 'stuff' that fills up the universe. For perfect fluids, it can be expressed in a simple linear form as

$$\tag{5.4.9} \boxed{P = w \, \varepsilon}$$

where $w$ is a dimensionless number.

- For non-relativistic matter (including dark matter), $w = 0$.
- For radiation and relativistic matter, $w = \frac{1}{3}$.
- $w < -\frac{1}{3}$ will provide a positive acceleration to the universe ($\ddot{a} > 0$). Such a component is called 'dark energy'.
- The cosmological constant $\Lambda$ is a special case of dark energy, where $w = -1$.

{{< callout type="remark" >}}
For adiabatic perturbations in a gas with pressure $P$ and energy density $\varepsilon$, the speed of sound $c_s$ is

$$c_s^2 = c^2 \, \frac{\partial P}{\partial \varepsilon} = w c^2$$

Since the speed of sound is always less than the speed of light, thus for all components of the universe we must have $w < 1$.
{{< /callout >}}

The total pressure and energy density of the universe can be expressed as

$$\tag{5.4.10} \varepsilon = \sum_w \varepsilon_w$$
$$\tag{5.4.11} P = \sum_w P_w = \sum_w w \varepsilon_w$$

From the fluid equation, we get

$$\tag{5.4.12} \boxed{\varepsilon_w (t) = \varepsilon_{w,0} \, a(t)^{-3(1+w)}}$$

where $\varepsilon_{w,0}$ is the energy density of the component at the present time.

- For matter ($w = 0$), $\varepsilon_\text{m} \propto a^{-3}$.
- For radiation ($w = \frac{1}{3}$), $\varepsilon_\text{r} \propto a^{-4}$.
- For cosmological constant $\Lambda$ ($w = -1$), $\varepsilon_\Lambda \propto a^0$.

Since the energy density of radiation is propotional to $T^4$, and also depends on the scale factor as $a^{-4}$, we can relate the temperature of the universe to the scale factor as

$$\tag{5.4.13}  T(t) \propto \frac{1}{a(t)} \implies T(t) = T_0 \, a(t)^{-1}$$

where $T_0$ is the present temperature of the universe.

## Cosmological Constant

The cosmological constant $\Lambda$ is a term added to Einstein's field equations of General Relativity to account for the observed accelerated expansion of the universe.

{{< callout type="trivia" >}}
The cosmological constant has a long history. It was first introduced by Einstein into his field equations as a mechanism to obtain a solution that would lead to a static universe. However, after Hubble's observation that the universe is expanding, Einstein removed $\Lambda$ from his equation and called it his "greatest blunder."

In the 1980s, several proposals of a negative pressure field were made, that could drive cosmic inflation in the very early universe. During the 1980s, most cosmological research focused on models with critical density in matter. These models were found to be successful at forming realistic galaxies and clusters, but some problems appeared in the late 1980s: in particular, the model required a value for the Hubble constant lower than preferred by observations, and the model under-predicted observations of large-scale galaxy clustering.

Finally, the first direct evidence for dark energy came from supernova observations in 1998 of accelerated expansion in Riess et al. and in Perlmutter et al., and the $\Lambda$CDM model then became the leading model.
{{< /callout >}}

Adding $\Lambda$ into our equations gives

$$\left( \frac{\dot{a}}{a} \right)^2 = \frac{8\pi G}{3 c^2} \varepsilon (t) - \frac{\kappa c^2}{R_0^2 \, a(t)^2} + \frac{\Lambda}{3}$$
$$\dot{\varepsilon} + 3 \frac{\dot{a}}{a} (\varepsilon + P) = 0$$
$$\frac{\ddot{a}}{a} = -\frac{4 \pi G}{3c^2} (\varepsilon + 3P) + \frac{\Lambda}{3}$$

The cosmological constant acts like a fluid with $w = -1$, and has its own associated energy density and pressure, both of which are constant over space and time.

$$\tag{5.4.14} \varepsilon_\Lambda = \frac{\Lambda c^2}{8 \pi G}$$
$$\tag{5.4.15} P_\Lambda = -\varepsilon_\Lambda = -\frac{\Lambda c^2}{8 \pi G}$$

Let $\Omega_\text{m}$, $\Omega_\text{r}$ and $\Omega_\Lambda$ be the density parameters for matter, radiation and dark energy respectively. Then the Friedmann equation can be rewritten as

$$\tag{5.4.16} \boxed{\Omega_\text{m} + \Omega_\text{r} + \Omega_\Lambda + \Omega_\kappa = 1}$$

{{< callout type="remark" >}}
The cosmological constant is just one type of dark energy, one which fills the universe with a constant unchanging energy density. Other models of dark energy include quintessence, which is a dynamic field that changes over time and space, and modified gravity theories, which propose changes to the laws of gravity on cosmological scales.

The current standard model of cosmology is known as $\Lambda$CDM, which includes the cosmological constant $\Lambda$, cold dark matter (CDM) and ordinary matter as its main components. The present time values of the density parameters are:

- $\Omega_{\text{m}, 0} \approx 0.3$
- $\Omega_{\text{r}, 0} \approx 8.4 \times 10^{-5}$
- $\Omega_{\Lambda, 0} \approx 0.7$
- $\Omega_{\kappa, 0} \approx 0$

{{< /callout >}}

## Deceleration Parameter

Taylor expanding the scale factor gives

$$
\begin{align*}
a(t) &= a_0 + \dot{a}_0 (t - t_0) + \frac{1}{2} \ddot{a}_0 (t - t_0)^2 + \ldots \\
&= 1 + H_0 (t - t_0) - \frac{1}{2} q_0 H_0^2 (t - t_0)^2 + \ldots
\end{align*}
$$

Here $q_0$ is the deceleration parameter, defined as

$$\tag{5.4.17} q_0 = - \left( \frac{\ddot{a}}{a \, H^2} \right)_{t=t_0} = \frac{1}{2} \sum_w \Omega_{w,0} (1+3w)$$

## Model Universes

We will now look at a few particular solutions to the Friedmann equations.

### Empty Curved Universe

For an empty curved universe, the Friedmann equation becomes

$$\tag{5.4.18} \dot{a}^2 = -\frac{\kappa c^2}{R_0^2}$$

The solutions to this equation are $\kappa = 0$ and $\dot{a} = 0$, corresponding to a static, empty and spatially flat universe, and $\kappa = -1$ and $\dot{a} = \pm \frac{c}{R_0}$, corresponding to an expanding or contracting universe.

### Flat Universe

For a flat universe ($\kappa = 0$) containing only a single component with equation of state coefficient of $w$, the Friedmann equation becomes

$$\tag{5.4.19} \dot{a}^2 = \frac{8 \pi G \varepsilon_0}{3 c^2} a^{-(1+3w)}$$

This gives the scale factor (for $w \neq -1$) as

$$\tag{5.4.20} \boxed{a(t) = \left( \frac{t}{t_0} \right)^{\frac{2}{3(1+w)}}}$$

where $t_0 = \frac{1}{1+w} \left( \frac{c^2}{6 \pi G \varepsilon_0} \right)^{\frac{1}{2}}$ is the age of the universe. For $w = -1$, we get an exponential solution for the scale factor.

The Hubble parameter is given by

$$\tag{5.4.21} H(t) = \frac{2}{3(1+w)} \frac{1}{t}$$

Hence $t_0 = \frac{2}{3(1+w)} H_0^{-1}$. The energy density is given by

$$\tag{5.4.22} \varepsilon(t) = \varepsilon_0 \, a(t)^{-3(1+w)} = \varepsilon_0 \, \left( \frac{t}{t_0} \right)^{-2}$$

Moreover since the universe is flat, $\varepsilon(t) = \varepsilon_\text{c}(t) = \frac{3c^2}{8 \pi G} H(t)^2$. From this we get

$$\tag{5.4.23} \varepsilon(t) = \frac{1}{6\pi (1+w)^2} \frac{c^2}{G} \frac{1}{t^2} = \frac{\varepsilon_\text{p}}{6\pi (1+w)^2} \left( \frac{t}{t_\text{p}} \right)^{-2}$$

where $\varepsilon_\text{p} = \frac{c^7}{\hbar G^2} \approx 2.9 \times 10^{126} \, \mathrm{J\,m^{-3}}$ is the Planck energy density and $t_\text{p} = \sqrt{\frac{\hbar G}{c^5}} \approx 5.4 \times 10^{-44} \, \mathrm{s}$ is the Planck time.

The time of emission of light which is observed to have a redshift of $z$ at the present time is given by

$$\tag{5.4.24} t_e = \frac{2}{3H_0(1+w)}(1+z)^{-\frac{3}{2}(1+w)}$$

This can be rearranged for the redshift as

$$\tag{5.4.25} 1 + z = \left( \frac{t_e}{t_0} \right)^{-\frac{2}{3(1+w)}}$$

The proper distance to the object at the present time is given by

$$\tag{5.4.26} d_p (t_0) = \frac{c}{H_0} \frac{2}{3(1+w)} \left[ 1 - \left(\frac{t_e}{t_0}\right)^{\frac{1+3w}{3+3w}} \right]$$

The proper distance to the object at the time of emission is $d_p(t_e) =\frac{ d_p(t_0) }{(1+z)}$.

All of this can be summarized into the following tables:

{{< callout type="table" >}}

| Quantity | Empty $\kappa = -1$ | Single Component $\kappa = 0$ |
|--|--|--|
| $a(t)$ | $t/t_0$ | $(t/t_0)^{\frac{2}{3(1+w)}}$ |
| $H(t)$ | $t^{-1}$ | $\frac{2}{3(1+w)} \frac{1}{t}$ |
| $\varepsilon (t)$ | $0$ | $\varepsilon_0 \, a(t)^{-3(1+w)} = \varepsilon_0 \, ( t / t_0)^{-2}$ |
| $t_0$ | $\frac{R_0}{c}$ | $\frac{1}{1+w} \left( \frac{c^2}{6 \pi G \varepsilon_0} \right)^{1/2}$ |
| $H_0$ | $t_0^{-1}$ | $\frac{2}{3(1+w)} \frac{1}{t_0}$ |
| $d_\text{hor}$ | - | $\frac{c}{H_0} \frac{2}{1+3w}$ |
| $t_e$ | $t_0 \, (1+z)^{-1}$ | $t_0 \, (1+z)^{-\frac{3}{2}(1+w)}$ |
| $1+z$ | $(t_e / t_0)^{-1}$ | $(t_e / t_0)^{-\frac{2}{3(1+w)}}$ |
| $d_p(t_0)$ | $\frac{c}{H_0} \ln (1+z)$ | $d_\text{hor} \left[ 1 - (1+z)^{-\frac{1+3w}{2}} \right]$ |

{{< /callout >}}

{{< callout type="table" >}}

| Quantity | Matter | Radiation | $\Lambda$ |
|--|--|--|--|
| w | $0$ | $\frac{1}{3}$ | $-1$ |
| $a(t)$ | $(t/t_0)^{2/3}$ | $(t/t_0)^{1/2}$ | $e^{H_0 (t - t_0)}$ |
| $H(t)$ | $\frac{2}{3t}$ | $\frac{1}{2t}$ | $\sqrt{\frac{\Lambda}{3}}$ |
| $\varepsilon (t)$ | $\varepsilon_0 \, a(t)^{-3}$ | $\varepsilon_0 \, a(t)^{-4}$ | $\varepsilon_0$ |
| $t_0$ | $\frac{2}{3 H_0}$ | $\frac{1}{2H_0}$ | - |
| $d_\text{hor}$ | $2 d_\text{H}$ | $d_\text{H}$ | - |
| $d_\text{EH}$ | - | - | $d_\text{H}$ |
| $d_p(t_0)$ | $d_\text{hor} \left[ 1 - (1+z)^{-1/2} \right]$ | $d_\text{hor} \left[ 1 - (1+z)^{-1} \right]$ | $d_\text{H} \, z$ |

{{< /callout >}}

A cosmological constant dominated universe is infinitely old, and has an infinite event horizon distance. For an object whose light is being observed at current time having redshift $z$, its proper distance at the time of emission was

$$d_p(t_e) = \frac{c}{H_0} \frac{z}{1 + z}$$

As $z \to \infty$, $d_p(t_e)$ approaches $\frac{c}{H_0}$, which is also the event horizon distance.

A universe with $\Lambda > 0$ is called a de Sitter universe. The de Sitter universe is a solution to Einstein's field equations with a positive cosmological constant, and describes a universe that is expanding exponentially.

A universe with $\Lambda < 0$ is called an anti-de Sitter universe. The anti-de Sitter universe is a solution to Einstein's field equations with a negative cosmological constant, and describes a universe that is contracting exponentially.

A universe with $\Lambda = 0$ is called a Minkowski or flat universe. The Minkowski universe is a solution to Einstein's field equations with zero cosmological constant, and describes a universe that is flat and static. This is the first case we discussed.

A flat matter dominated universe is also called an Einstein-de Sitter universe.

{{< callout type="remark" >}}
Except the Minkowski or cosmological constant dominated universe, each universe has an age. This is the time elapsed since its creation, when the scale factor was zero. This point is called the 'Big Bang'.
{{< /callout >}}

## Problems

{{< tabs >}}
    {{< tab name="P1" >}}
    Consider a radiation dominated universe, such that $\Omega_r = 1$. Find the number of photons in the observable universe as a function of time, from the big bang
    {{< /tab >}}

    {{< tab name="Solution" >}}
    From equation (5.4.23) we get that the energy density as a function of time is

    $$ \varepsilon_r(t) = \frac{3 \varepsilon_\text{p}}{32} \left( \frac{t}{t_\text{p}} \right)^{-2} $$

    From this we can get the temperature of the universe as a function of time using equation (2.1.31)

    $$ \varepsilon (t) = a T(t)^4 $$
    $$ \implies T(t) = \left( \frac{45}{32 \pi^2} \right)^{1/4} T_\text{p} \left( \frac{t}{t_\text{p}} \right)^{-1/2} $$

    where $T_\text{p} = \left( \frac{c^5}{\hbar G} \right)^{1/4} \approx 1.4 \times 10^{32} \, \text{K}$ is the Planck temperature.

    To get the photon number density, we use equation (2.1.33)

    $$ n(t) = \beta \, T(t)^3 $$

    To get the total number of photons, we first have to find the volume of the observable universe. For that we take the radius of the universe to be the particle horizon.

    $$ V(t) = \frac{4}{3} \pi d_\text{hor} (t)^3 = \frac{32 \pi c^3}{3} t^3 $$

    Hence the total number of photons in the observable universe at some time $t$ after the big bang is

    $$ N(t) = n(t) V(t) \approx \boxed{1.9 \, (t / t_\text{p})^{3/2}} $$

    {{< /tab >}}
{{< /tabs >}}
