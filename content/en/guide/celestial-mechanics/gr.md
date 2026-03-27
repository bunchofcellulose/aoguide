---
title: General Relativity
weight: 8
---

General Theory of Relativity is a theory of gravitation that was developed by Albert Einstein in the year 1915. It describes gravity not as a force, but as a curvature of spacetime caused by the presence of mass and energy. The theory has been confirmed by numerous experiments and observations, and has become a cornerstone of modern physics. In this section, we will explore some of the key concepts and phenomena related to general relativity, including orbits in curved spacetime, gravitational waves, and the precession of apsis.

{{< callout type="person" >}}
[Albert Einstein](https://en.wikipedia.org/wiki/Albert_Einstein) (1879-1955) was a German-born theoretical physicist who developed the theory of relativity, one of the two pillars of modern physics (alongside quantum mechanics). He is best known for his mass-energy equivalence formula $E=mc^2$, which has been dubbed "the world's most famous equation". Einstein's work has had a profound impact on our understanding of the universe, and he is widely regarded as one of the greatest scientists in history.

Aside from the theory of special and general relativity, Einstein made significant contributions to the development of quantum mechanics, statistical mechanics, and cosmology. He received the Nobel Prize in Physics in 1921 for his explanation of the photoelectric effect, which was a key step in the development of quantum theory. Einstein's legacy continues to influence physics and our understanding of the universe to this day.
{{< /callout >}}

{{< callout type="trivia" >}}
The four tests of general relativity are:

1. The perihelion precession of Mercury's orbit
2. The deflection of light by the Sun
3. The gravitational redshift of light
4. The Shapiro time delay of light passing near a massive object

The test for the deflection of light by the Sun was first performed during a solar eclipse in 1919 by Sir Arthur Eddington, and provided one of the first pieces of evidence in support of general relativity. The other tests have also been confirmed by various experiments and observations over the years, further solidifying the theory's status as a cornerstone of modern physics.
{{< /callout >}}

## Orbits in General Relativity

Orbits in general relativity are more complex than those in Newtonian mechanics due to the curvature of spacetime. The equations governing the motion of bodies in a gravitational field are derived from Einstein's field equations, which relate the curvature of spacetime to the energy and momentum of matter and radiation. Here, we shall explore the properties of orbits in general relativity, including the existence of stable and unstable circular orbits.

Consider a system of a massive central mass $M$ being orbited by a smaller mass $m$, such that the central body is essentially at rest. The energy analogue in general relativity is given by

$$ \frac{1}{2} \dot{r}^2 + \frac{h^2}{2r^2} - \frac{GM}{r} - \frac{GMh^2}{c^2 r^3} = \epsilon $$

Here $\epsilon$ is a term related to the energy of the system, and $h$ is the specific angular momentum of the orbiting body.

{{< callout type="remark" >}}
The above equation is derived from the Schwarzschild metric, which describes the spacetime geometry around a non-rotating, spherically symmetric mass. The additional term $-\frac{GMh^2}{c^2 r^3}$ compared to the Newtonian case arises due to the curvature of spacetime and leads to significant differences in the behavior of orbits, especially near massive bodies like black holes.

The Schwarzschild metric was the first exact solution to Einstein's field equations, found by Karl Schwarzschild in 1916. It is given by

$$ ds^2 = -\left( 1 - \frac{r_s}{r} \right) c^2 dt^2 + \left( 1 - \frac{r_s}{r} \right)^{-1} dr^2 + r^2 d\Omega^2 $$

where $d\Omega^2$ is the metric on the unit sphere. The Schwarzschild radius $r_s = \frac{2GM}{c^2}$ is a critical radius at which the escape velocity equals the speed of light, and it defines the event horizon of a black hole.

We shall talk more about metrics when discussing cosmology.
{{< /callout >}}

For a circular orbit, $\dot{r} = 0$, which gives the radius of the orbit as

$$\tag{3.7.9} r = \frac{h^2}{2GM} \left[ 1 \pm \sqrt{1 -\frac{12G^2M^2}{c^2h^2}} \right] $$

We see that for a given angular momentum $h$, two circular orbits are possible. Introducing $a = h/c$ and the schwarschild radius $r_s = \frac{2GM}{c^2}$,

$$ r = \frac{a^2}{r_s} \left( 1 \pm \sqrt{1 - \frac{3r_s^2}{a^2}} \right) $$

Therefore for a circular orbit, $a > \sqrt{3} r_s$. This puts a limit on the minimum angular momentum of the body ($h_\text{min} = \sqrt{3} r_s c$).

The inner orbit

$$ r_\text{inner} = \frac{a^2}{r_s} \left( 1 - \sqrt{1 - \frac{3r_s^2}{a^2}} \right) $$

is unstable, while the outer orbit

$$ r_\text{outer} = \frac{a^2}{r_s} \left( 1 + \sqrt{1 - \frac{3r_s^2}{a^2}} \right) $$

is stable. The stability of the orbits can be determined by analyzing the second derivative of the effective potential, which shows that the inner orbit corresponds to a local maximum (unstable) and the outer orbit corresponds to a local minimum (stable).

Therefore the minimum radius of a stable circular orbit is when $a^2 = 3r_s^2$

$$\tag{3.7.10} r = \frac{a^2}{r_s} = 3r_s = \frac{6GM}{c^2} $$

An orbit at this radius is known as the innermost stable circular orbit (ISCO). This means that for a non-rotating black hole, any matter that comes within this radius will inevitably spiral into the black hole, while matter outside this radius can potentially form an accretion disk and emit radiation. The ISCO is an important concept in astrophysics, as it determines the inner edge of the accretion disk around a black hole and has implications for the emission of X-rays and other high-energy radiation from the vicinity of black holes.

{{< callout type="trivia" >}}
A very interesting consequence of the existence of the ISCO is that it leads to a maximum possible efficiency for energy extraction from accretion onto a black hole. For a non-rotating black hole, the maximum efficiency is about 6%, meaning that up to 6% of the rest mass energy of the infalling matter can be converted into radiation. For rotating black holes, the efficiency can be much higher, up to about 42% for a maximally rotating Kerr black hole.
{{< /callout >}}

In the limit $a \gg r_s$,

$$\tag{3.7.11} r_\text{outer} = \frac{2a^2}{r_s} = \frac{h^2}{GM}\,,\qquad\qquad r_\text{inner} = \frac{3}{2} r_s = \frac{3GM}{c^2} $$

From the equation, we see that circular orbits with radius smaller than $\frac{3}{2} r_s$ are not possible. An object that has crossed this boundary can still escape the black hole if it has enough energy, but it cannot maintain a stable orbit. It must accelerate to escape, and if it fails to do so, it will eventually spiral into the black hole.

Moreover, the orbit with radius $\frac{3}{2} r_s$ is known as the photon sphere, and it represents the closest distance at which light can orbit a massive body in a circular path (in fact, this is the only circular orbit possible for massless particles). This is an unstable orbit, and any perturbation will cause the photon to either fall into the black hole or escape to infinity. The photon sphere is a unique feature of the spacetime around a black hole and has important implications for the behavior of light and the appearance of black holes.

{{< callout type="remark" >}}
The existence of the photon sphere also leads to interesting phenomena such as gravitational lensing, where light from a background source can be bent around a massive object, creating multiple images or even a ring-like structure known as an Einstein ring. This will be discussed in more detail later.
{{< /callout >}}

## Precession of apsis in General Relativity

It was noted in the mid-19th century by Urbain Le Verrier that the apsis of Mercury's orbit precesses at a rate of $43$ arcseconds per century, which could not be explained by Newtonian mechanics. This was one of the first pieces of evidence for general relativity, which could explain this anomalous precession. We shall show how to calculate this precession using two methods: the precession of the LRL vector, and using the orbit equation in general relativity.

{{< callout type="trivia" >}}
A similar deviation from predicted orbit was first observed in the orbit of Uranus, which led to the discovery of Neptune, and then also led to the discovery of Pluto. A similar explanation for the precession of Mercury's orbit was proposed by Le Verrier, which involved the existence of an intra-Mercurial planet named Vulcan. However, no such planet was ever observed, and the explanation was eventually discarded in favor of general relativity.
{{< /callout >}}

{{< callout type="image" >}}
{{< gif "celmech/precession.gif" "Precession of apsis in General Relativity" "The apsis of the orbit precesses over time if considering effects of general relativity. (Source: Wikipedia)" >}}
{{< /callout >}}

### Precession of LRL vector under a perturbed potential

Consider a small perturbation $h(r)$ to the potential energy $V(r)$, such that

$$ V(r) = -\frac{k}{r} + h(r) $$

Since the force is no longer inverse-square, the LRL vector is no longer conserved, and precesses, leading to precessiong of apsis.

$$ \frac{d\mathbf{A}}{dt} = - \frac{d h(r)}{dt} \, \hat{\mathbf{r}} \times \mathbf{L} = L \frac{d}{dt} h(r) \: \hat{\mathbf{\varphi}} $$

Since $\mathbf{L}$ and $E$ are still conserved, the magnitude of $\mathbf{A}$ remains constant. Writing $L = mr^2 \dot{\theta}$,

$$ \frac{d \mathbf{A}}{d \theta} = -m \frac{d}{du} h(u) \hat{\mathbf{\varphi}} $$

where $u = 1/r$. The average precession of the apsis

$$ \Delta \varphi \approx \frac{|\Delta \mathbf{A}|}{A} = \frac{m}{A} \int_0^{2 \pi} \frac{d}{du} h(u) d \theta $$

The rate of precession is therefore given by

$$\tag{3.7.4} \dot{\varphi} = \frac{m}{AT} \int_0^{2 \pi} \frac{d}{du} h(u) d \theta $$

If the perturbation is small, the orbit during one revolution can be approximated as Keplerian

$$ u = \frac{mk}{L^2} \left[ 1 + \frac{A}{mk} \cos \theta \right] $$

and hence the integral can be evaluated.

For example, the potential due to a point mass in general relativity is given by

$$\tag{3.7.5} V(r) = - \frac{GMm}{r} - \frac{GML^2}{mc^2r^3}$$

Evaluating the integral gives

$$\tag{3.7.6} \Delta \varphi = \frac{6 \pi G^2M^2m^2}{c^2L^2}$$

### Using the orbit equation

The orbit equation in general relativity is given by

$$ \frac{d^2 u}{d \theta^2} + u = \frac{GMm^2}{L^2} + \frac{3GM}{c^2} u^2 $$

Defining a dimensionless $w = \frac{L^2}{GMm^2} u$ and $\alpha = \frac{2G^2M^2m^2}{c^2L^2} \:\: (\ll 1)$,

$$ \frac{d^2 w}{d \theta^2} + w = 1 + \alpha w^2 $$

Since $\alpha$ is very small, we can use perturbation methods to find an approximate solution for $w$. In the first order, $w (\alpha)$ can be expanded in terms of a power series as

$$ w = w_0 + \alpha w_1 $$

$w_0$ just gives the newtonian solution

$$ \frac{d^2 w_0}{d \theta^2} + w_0 = 1 \implies w_0 = 1 + e \cos \theta $$

For $w_1$, we get

$$ \frac{d^2 w_1}{d \theta^2} + w_1 \approx w_0^2 = 1 + \frac{e^2}{2} + 2 e \cos \theta +\frac{e^2}{2} \cos 2 \theta $$

This gives the solution for $w_1$ as

$$ w_1 = 1 + \frac{e^2}{2} + e \theta \sin \theta - \frac{e^2}{6} \cos 2 \theta $$

Putting everything together and neglecting the small terms, we get

$$ w \approx 1 + e \cos \left[ (1 - \alpha) \, \theta \right] $$

The period of the ellipse is not $2 \pi$, and hence precesses at a rate of

$$ \Delta \varphi = 2\pi - \frac{2 \pi}{1 - \alpha} \approx 2\pi \alpha = \frac{6\pi G^2 M^2 m^2}{c^2L^2} $$

which matches the result which we obtained via the precession of the LRL vector.

## Gravitational Waves

Gravitational waves are waves of spacetime curvature that propagate at the speed of light and are produced by the relative motion of gravitating masses. They were predicted by Einstein in 1916 as a consequence of his general theory of relativity, and were first directly detected by the LIGO and Virgo collaborations in 2015. The sources of gravitational waves include binary systems of compact objects (like black holes and neutron stars), supernovae, and the early universe.

{{< callout type="trivia" >}}
The first evidence of graviational waves came from the observation of the Hulse-Taylor binary pulsar in 1974, which showed that the orbit of the pulsar was decaying at a rate consistent with the emission of gravitational waves. This discovery earned Hulse and Taylor the Nobel Prize in Physics in 1993. The direct detection of gravitational waves by LIGO in 2015 was a groundbreaking achievement that confirmed a major prediction of general relativity and opened up a new era of gravitational wave astronomy.
{{< /callout >}}

Consider two massive bodies $M_1$ and $M_2$ orbiting each other, with position vectors $\mathbf{r_1}$ and $\mathbf{r_2}$ relative to the center of mass. We define $M = M_1 + M_2$ and $m = \frac{M_1 M_2}{M_1 + M_2}$.

According to general theory of relativity, accelerated masses with non zero quadrouple moments radiate gravitataional waves (GWs) and lose energy. For small enough velocities, the emitted GWs

- have a frequency twice as large as the orbital frequency
- can be characterized by a luminosity, which is dominated by the expression

$$\tag{3.7.12} P = \frac{32}{5} \frac{G}{c^5}m^2 a^4 \Omega^6 $$

where $a$ is the orbital separation and $\Omega$ is the angular velocity of each mass.

The energy of the system is $E = - \frac{GMm}{2a}$. Differentiating, we get

$$\tag{3.7.13} \left( \frac{d \Omega}{dt} \right)^3 = \left( \frac{96}{5} \right)^3 \frac{\Omega^{11}}{c^5} (GM_c)^5 $$

where we define the chirp mass $M_c = m^{3/5} M^{2/5}$.

Now, $f_\text{GW} = 2f = \frac{\Omega}{\pi}$ gives

$$\tag{3.7.14} f_\text{GW}^{-8/3} (t) = \frac{(8 \pi)^{8/3}}{5} \left( \frac{GM_c}{c^3} \right)^{5/3} (t_0 - t) $$

where $t_0$ is a constant of integration.

{{< tabs >}}
    {{< tab name="P1" >}}
    [Problem](https://ipho.olimpicos.net/pdf/IPhO_2018_Q1.pdf). This problem asks you to calculate the power of the GW150914 gravitational wave (the first gravitational wave detected by LIGO) and thus estimate the sizes and masses of the objects that produced it.
    {{< /tab >}}

    {{< tab name="Solution" >}}
    [Solution](https://ipho.olimpicos.net/pdf/IPhO_2018_S1.pdf)
    {{< /tab >}}

    {{< tab name="IPhO 2018" >}}{{< /tab >}}
{{< /tabs >}}
