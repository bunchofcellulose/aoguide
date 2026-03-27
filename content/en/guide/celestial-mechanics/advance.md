---
title: Advanced Topics
weight: 7
---

## Laplace-Runge-Lenz Vector

For an inverse square law force of the form

$$\mathbf{F} = -\frac{k}{r^2} \hat{\mathbf{r}}$$

and the corresponding potential energy $V(r) = -k/r$, the Laplace-Runge-Lenz vector, or LRL vector is defined as

$$\tag{3.7.1} \boxed{ \mathbf{A} = \mathbf{p} \times \mathbf{L} - m k \hat{\mathbf{r}} } $$

$\mathbf{p}$ and $\mathbf{L}$ are the linear and angular momentum of the particle at any instant, and $\hat{\mathbf{r}}$ is the unit vector pointing from the center of mass to the particle. The constant parameter k describes the strength of the central force; it is equal to $GMm$ for gravitational forces.

The LRL vector is a scaled version of the eccentricity vector, $\mathbf{A} = mk \mathbf{e}$, and hence is a constant of motion. This means that $\mathbf{A}$ does not change with time, and is the same at all points along the orbit. The direction of $\mathbf{A}$ points along the major axis of the orbit, and its magnitude is related to the eccentricity of the orbit. For circular orbits, $\mathbf{A} = 0$, while for elliptical orbits, $\mathbf{A}$ is non-zero and points towards the periapsis.

The magnitude of the LRL vector is

$$\tag{3.7.2} A^2 = m^2 k^2 + 2mEL^2 $$

where E is the total energy of the system.

Together with the conservation of energy and angular momentum, the conservation of the LRL vector allows us to solve for the trajectory of a particle under an inverse-square central force, and also to determine the shape of the orbit (ellipse, parabola, or hyperbola).

{{< callout type="trivia" >}}
The Laplace–Runge–Lenz vector is named after Pierre-Simon de Laplace, Carl Runge and Wilhelm Lenz. Ironically, none of those scientists discovered it. The LRL vector has been re-discovered and re-formulated several times (by Hermann, Bernoulli, Hamilton, Gibbs and more). Various generalizations of the LRL vector have been defined, which incorporate the effects of special relativity, electromagnetic fields and even different types of central forces. It is also relevant in quantum mechanics, where it is used to explain the degeneracy of energy levels in the hydrogen atom.
{{< /callout >}}

{{< callout type="remark" >}}
the energy, three components of the angular momentum vector, and three components of the LRL vector are all constants of motion for a particle under an inverse-square central force. However, these 7 constants are not independent, as they satisfy the relation $A^2 = m^2 k^2 + 2mEL^2$ and $\mathbf{A} \cdot \mathbf{L} = 0$. Hence, there are only 5 independent constants of motion, which is equal to the number of degrees of freedom of the system. This is a manifestation of the fact that the system is superintegrable (what is that?).
{{< /callout >}}

{{< callout type="image" >}}
{{< svg "celmech/lrl.svg" "Laplace-Runge-Lenz Vector" "The Laplace-Runge-Lenz vector is a constant of motion for central force problems. (Source: Wikipedia)" >}}
{{< /callout >}}

{{< tabs >}}
{{< tab name="P1" >}}
Two satellites orbit Earth on the same plane along elliptic paths of eccentricities $e_1$ and $e_2$ respectively. The angle between their major axes is $\alpha$. The rate at which a line segment connecting a satellite and the Earth’s centre sweeps out an area is $L_1$ and $L_2$ respectively. What is the maximal relative velocity of the satellites? Provide also a simplified answer for $\alpha=90^\circ$ and $L_1=L_2$. The ratio of the orbital periods of the satellites is an irrational number. Earth’s mass is denoted by $M$, and the gravitational constant by $G$.
{{< /tab >}}

{{< tab name="Solution" >}}
The solution by [Sainavaneet](https://physicscup.ee/wp-content/uploads/2024/P4-best/3.Sainaveet.pdf) uses the LRL vector to find the maximum relative velocity of the two satellites.
{{< /tab >}}

{{< tab name="Physics Cup – TalTech 2024" >}}{{< /tab >}}
{{< /tabs >}}

{{< tabs >}}
{{< tab name="P2" >}}
At two different points in its orbit, a comet has velocities $\vec{v}_1$ and $\vec{v}_2$. If (i) $\vec{v}_1$ and $\vec{v}_2$ are orthogonal and (ii) $|\vec{v}_1| = 2|\vec{v}_2|$, what is the smallest possible eccentricity of the orbit?
{{< /tab >}}

{{< tab name="Solution" >}}
Refer to [Lotus Chen](https://physicscup.ee/wp-content/uploads/PC2021/P2/1.-Physics-Cup-2021-Problem-2-Lotus-Chen.pdf)'s neat solution using the LRL vector.
{{< /tab >}}

{{< tab name="Physics Cup – TalTech 2021" >}}{{< /tab >}}
{{< /tabs >}}

### Trajectory of the momentum vector

The conservation of the LRL vector $\mathbf{A}$ and angular momentum vector $\mathbf{L}$ is useful in showing that the momentum vector $\mathbf{p}$ moves on a circle under an inverse-square central force. The trajectory of the momentum vector $\mathbf{p}$ is called a hodograph.

$$ mk \hat{\mathbf{r}} = \mathbf{p} \times \mathbf{L} - \mathbf{A} $$

$$\implies (mk)^2 = A^2 + p^2L^2 + 2\mathbf{A} \cdot (\mathbf{p} \times \mathbf{L}) $$

Choosing $\mathbf{L}$ along the $z$-axis, and the major semiaxis as the $x$-axis, yields the locus equation for $\mathbf{p}$

$$\tag{3.7.3} p_x^2 + \left( p_y - \frac{A}{L} \right)^2 = \left( \frac{mk}{L} \right)^2 $$

Thus, the momentum vector $\mathbf{p}$ is confined to a circle of radius $mk/L$ centered on $(0,\, A/L)$.

{{< callout type="image" >}}
{{< svg "celmech/hodograph.svg" "Hodograph" "The hodograph is a useful tool for visualizing the momentum vector in central force problems. (Source: Wikipedia)" >}}
{{< /callout >}}

For unbounded orbits, $A > mk$ and hence the circle does not intersect the $p_x$-axis.

{{< tabs >}}
{{< tab name="P3" >}}
A satellite orbits a planet. At point $A$, its speed is $v_1$. At point $B$, its speed is $v_2$ and its velocity vector forms a right angle with the velocity vector at point $A$. At point $C$, the velocity is exactly opposite to the velocity at point $A$, with a magnitude of $v_3$. Find the eccentricity of the orbit. Also determine the exact numerical value of the eccentricity when $v_1=1\,\text{km/s}$, $v_2=2\,\text{km/s}$, and $v_3=3\,\text{km/s}$.
{{< /tab >}}

{{< tab name="Solution" >}}
Refer to the solution by [Alexandru Bordei](https://physicscup.ee/wp-content/uploads/2025/09/Alexandru.pdf) to see the use of hodographs in action.
{{< /tab >}}

{{< tab name="Physics Cup – TalTech 2025" >}}{{< /tab >}}
{{< /tabs >}}

## Orbit Equation

Consider a particle of mass $m$ moving under an arbitrary central potential $V(r)$. The angular momentum of the particle is conserved, and is given by

$$ L = mr^2 \dot{\theta} $$

The energy, which is also conserved, of the particle is given by the sum of its kinetic and potential energy

$$E = \frac{1}{2}mv^2 + V(r) = \frac{1}{2}m(\dot{r}^2 + r^2 \dot{\theta}^2) + V(r)$$

Differentiating with respect to time, and substituting the $L = mr^2 \dot{\theta}$, we get the equation of motion of the particle

$$ m\ddot{r} - \frac{L^2}{m r^3} = - \frac{dV}{dr} $$

Substituting $u = 1/r$ and simplifying, we get

$$\tag{3.7.7} \boxed{\frac{d^2 u}{d \theta^2} + u = -\frac{m}{L^2} \frac{d}{du} V(u)} $$

This is the orbit equation. Also referred to as Binet's equation, it describes the shape of the orbit $r(\theta)$ of a particle moving under a central force. If the shape of the trajectory is known, the force law can be determined by solving for $V(u)$.

For an inverse square force having potential $V(r) = -k/r = -ku$, the orbit equation $u(\theta)$ is given by

$$\tag{3.7.8} \frac{d^2 u}{d \theta^2} + u = -\frac{km}{L^2} $$

This is, if one can recognize, the equation of a conic section. The solution $u(\theta)$ is

$$ u = \frac{mk}{L^2} \left( 1 + e \cos (\theta - \theta_0) \right) $$

where $e$ (the eccentricity) and $\theta_0$ (the phase offset) are constants of integration. This confirms that the orbits under an inverse-square central force are indeed conic sections, with the center of force at one of the foci.

{{< callout type="remark" >}}
Let us clarify what bound, closed and stable orbits mean

- A **bound** orbit is one where the total energy $E < 0$. The particle cannot escape to infinity, and will always remain within a certain distance from the center of force.
- A **closed** orbit is one where the particle returns to its initial position after a finite period of time. Closed orbits are a subset of bound orbits, but not all bound orbits are closed. For example, in an inverse-square law force, elliptical orbits are closed, but parabolic and hyperbolic orbits are not.
- A **stable** orbit is one where small perturbations to the particle's position or velocity do not lead to large deviations from the original orbit. In other words, if the particle is slightly displaced from its orbit, it will oscillate around the original orbit rather than diverging away from it. Stability is a more general concept that can apply to both bound and unbound orbits.

Now, as it turns out, there exist only two types of central force potentials that produce closed orbits for all bound particles: the inverse-square law potential ($V(r) \propto -1/r$) and the radial harmonic oscillator potential ($V(r) \propto r^2$). This result is known as Bertrand's theorem.

As far as stability is concerned, all closed orbits must be stable to begin with. Hence, the inverse square law and radial harmonic oscillator potentials produce stable closed orbits.

Aside from these two, there are also closed circular orbits in any central force potential, but these are not stable in general. (in a potential $V(r) \propto r^n$, circular orbits are stable only if $n > -2$)
{{< /callout >}}

{{< tabs >}}
{{< tab name="P4" >}}
Daniel, a strange guy, finds a strange force as well. He finds it to be a central force proportional to $r^n$, where $r$ is the distance from the source of the force to the body affected by it (perhaps, think of it as a strange type of “gravity”). What value of $n$ could make it such that closed, stable, nearly circular orbits can occur by bodies under the influence of this force (that is, orbits without precession each period)?

$$\text{A.} \: 10 \qquad\qquad \text{B.} \: 11 \qquad\qquad \text{C.} \: 12 \qquad\qquad \text{D.} \: 13$$
{{< /tab >}}

{{< tab name="Solution" >}}
A central force proportional to $r^n$ would give a potential of the form

$$ V = k r^{n + 1} = k u^{-n - 1} $$

Using the binet equation,

$$ u'' + u = \frac{mk(n+1)}{L^2} u^{-n - 2} $$

Let the radius of a circular orbit be $u_0$. For a circular orbit, $u'' = 0$, which gives

$$ u_0^{n + 3} = \frac{mk(n+1)}{L^2} $$

To check for stability, we perturb the orbit a little. Substituting $u = u_0 + \eta$ and linearizing (ignoring quadratic and higher order terms), we get

$$ \eta'' + \eta = \frac{mk(n+1)}{L^2} (u_0^{-n - 2} \eta - (n + 2) u_0^{-n - 1} \eta) $$

This gives a linear equation for $\eta$, which can be analyzed for stability.

$$ \eta'' + (n + 3) \eta = 0 $$

This is an equation for a simple harmonic motion. Thus for small perturbations, the orbit oscillates about the circular orbit with frequency $\sqrt{n + 3}$. Therefore, for stability, we need $n + 3 > 0 \implies n > -3$.

For the orbit to be closed, we must have that the frequency of oscillation is a rational multiple of the orbital frequency. The orbital frequency is 1 (since $\theta$ increases by $2\pi$ in one orbit), and the oscillation frequency is $\sqrt{n + 3}$. Therefore, for closed orbits, $\sqrt{n + 3}$ must be a rational number.

The only option which satisfies both these conditions is $\textbf{D. 13}$.

{{< /tab >}}

{{< tab name="OAC Open 2025" >}}{{< /tab >}}
{{< /tabs >}}

## Poynting Robertson Effect

The Poynting-Robertson effect is a phenomenon that occurs when a small particle orbits a star and is subjected to the combined effects of radiation pressure and the Doppler shift of the incoming radiation. It causes the particle to lose angular momentum and spiral slowly towards the star.

The force of radiation acting on a particle of mass $m$ density $\rho$ and radius $R$ is $F_\text{rad} = P_\text{rad} \sigma_\text{pr}$, where $\sigma_\text{pr} = Q_\text{pr} \pi R^2$ is the cross section of the particle, $Q_\text{pr}$ is the radiation pressure coefficient, and $P_\text{rad}$ is the radiation pressure. The radiation pressure is given by

$$\tag{3.7.15} P_\text{rad} = \frac{L}{4 \pi r^2 c} $$

where $L$ is the luminosity of the star and $r$ is the distance from the star. For sun, the peak wavelength is $\lambda_{p} \approx 500 \mathrm{\,nm}$. For $R \gg \lambda_p$, where sun's gravity dominates over radiation pressure, the Poynting-Robertson effect acts as a brake on orbiting particles, decreasing their angular momenta so that they slowly spiral into the sun. In the frame of the orbiting particle, the phenomena of abberation causes slight displacement in the direction of the motion for photons striking the particle. This applies a torque on the particle, causing it to lose angular momentum.

$$ \mathbf{\tau} = \mathbf{r} \times \mathbf{F} = \frac{d \mathbf{L}}{dt} $$
$$ \tau = -rF*\text{rad} \sin \theta = -r \frac{LR^2 Q*\text{pr}}{4cr^2} \frac{v}{c} $$

The angular momenta of the orbiting particle is

$$ L = m \sqrt{GMr} \implies \frac{dL}{dt} = \frac{m}{2} \sqrt{\frac{GM}{r}} \frac{dr}{dt} $$

Hence we get that the radius of the particle's orbit decays as

$$ \frac{dr}{dt} = -\frac{1}{r} \frac{L}{2c^2} \frac{R^2 Q\_\text{pr}}{m} $$

The Poynting Robertson time scale is the time it takes for the particle to spiral into the sun

$$\tag{3.7.16} t_\text{pr} = \frac{a^2 c^2}{L} \frac{4 \pi}{3} \frac{\rho R}{Q_\text{pr}} $$

where $r = a$ is the initial radius of the particle's orbit.
