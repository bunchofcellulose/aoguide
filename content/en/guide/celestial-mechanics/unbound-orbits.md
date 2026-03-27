---
title: Unbound Orbits
weight: 3
---

We now move on to *unbound* orbits. Unlike what you might think, they aren't unphysical; examples include comets originating from the Oort cloud, or perhaps even having interstellar origin. You can check [this wiki page](https://en.wikipedia.org/wiki/List_of_parabolic_and_hyperbolic_comets) for particular examples.

As we proved in chapter 3.1, trajectories having energy greater than or equal to zero are *unbound*. We also saw that these trajectories have eccentricities greater than or equal to 1, and thus are parabolic or hyperbolic in nature. We'll briefly go over both of them. You should at least have some knowledge of these conic sections before proceeding further.

## Parabolic trajectory

A parabolic trajectory is one where the orbiting body makes the shape of a parabola. This happens when the body has just enough energy to escape the gravitational pull of the other body, but still passes close enough to it to be deflected by its gravity. The trajectory is unbound, and the body will escape to infinity.

A parabola is a conic section with eccentricity equal to 1. The *vertex point* is the point of closest approach and is closest to the focus. If the distance to the *focus* from the vertex of the parabola is $r_p = a$, the length of the semi-latus rectum is $p = 2a$. The equation of the parabolic trajectory is then:

$$\tag{3.3.1} r = \frac{2a}{1 + \cos \theta}$$

The angular momentum of such a trajectory is $h = \sqrt{2 \mu a}$ from eqn. $(3.1.10)$. Because the total energy of a parabolic trajectory is zero, the potential energy must cancel out the kinetic energy. Using this we get that the velocity at any point, at a distance $r$ from the focus, is equal to the escape velocity (if it was moving in a circle of radius $r$):

$$\tag{3.3.2} v = \sqrt{\frac{2\mu}{r}}$$

The velocity at the point of closest approach is

$$\tag{3.3.3} v_p = \sqrt{\frac{2\mu}{r_p}} = \sqrt{\frac{2\mu}{a}}$$

Parabolic trajectories have eccentricity exactly equal to 1 and energy exactly equal to 0. Thus in practice, they are not very common, since any small perturbation can make the trajectory either elliptical or hyperbolic. Thus, most comets that are observed to have parabolic trajectories are actually on very elongated elliptical orbits.

## Hyperbolic trajectory

A hyperbolic trajectory is one where the orbiting body makes the shape of a hyperbola. This happens when the body has enough energy to escape the gravitational pull of the other body, but still passes close enough to it to be deflected by its gravity. The trajectory is unbound, and the body will escape to infinity.

A hyperbola is a conic section with eccentricity greater than 1. The *vertex point* is the point of closest approach and is closest to the focus. Let the semi-major axis of the hyperbola be $a$. By convention, we define it to be a negative quantity. This is done so that the equations match with those of an elliptical orbit. The distance of vertex from focus is

$$\tag{3.3.4} r_p = (-a) (e - 1) = a(1-e) $$

The semi-latus rectum is

$$ p = (-a)(e^2 - 1) = a(1 - e^2) $$

The equation of the hyperbolic trajectory is

$$ r = \frac{a(1-e^2)}{1 + e \cos \theta} $$

Both of which are identical to the formulas for ellipses. We see that the true anomaly can only take values between $-\cos^{-1} \left(\frac{-1}{e}\right)$ and $\cos^{-1} \left(\frac{-1}{e}\right)$. This wasn't an issue earlier, because $e$ was less than 1 for a bound orbit. Note that the bound for a parabola is $(-\pi, \pi)$

The angular momentum of the system is $h = \sqrt{\mu a (1 - e^2)}$, and the total energy is given by $\varepsilon = -\frac{\mu}{2a}$. Note that the energy is positive, due to $a$ being negative. The velocity of the body at a distance $r$ from the focus is given by

$$\tag{3.3.5} v^2 = \mu \left( \frac{2}{r} + \frac{1}{a} \right)$$

The velocity at the point of closest approach is

$$\tag{3.3.6} v_p = \sqrt{\mu \left( \frac{2}{r_p} + \frac{1}{a} \right)} = \sqrt{\frac{\mu}{a} \left( \frac{1+e}{1-e} \right)}$$

The velocity at infinity is

$$\tag{3.3.7} v_\infty = \sqrt{\frac{\mu}{a} \left( \frac{1-e}{1+e} \right)}$$

Hyperbolic trajectories are very common. For example, the Voyager 1 and Voyager 2 spacecrafts are on hyperbolic trajectories, and will eventually leave the Solar System. Planetary flybys are also examples of hyperbolic trajectories, where a spacecraft approaches a planet, gets deflected by its gravity, and then leaves the planet's sphere of influence.

{{< callout type="remark" >}}
The impact parameter $b$ is defined as the distance of closest approach if the trajectory was a straight line. It is related to the eccentricity by $b = a \sqrt{e^2 - 1}$ (it is equal to the semi-minor axis of the hyperbola). The impact parameter is often used in scattering problems, where a particle approaches a target and gets deflected, as in the problem below.
{{< /callout >}}

{{< tabs >}}
    {{< tab name="P1" >}}
    Consider a rogue planet of mass $m$ approaching a star of mass $M$, and getting deflected due to its gravity. Far away from the star, the planet has a speed $v_0$ and an impact parameter $b$. Find the speed of the planet at infinity after the encounter, and the angle of deflection.
    {{< /tab >}}

    {{< tab name="Solution" >}}
    We can solve this by conservation of energy $\varepsilon$, angular momentum $\mathbf{h}$, and the eccentricity vector $\mathbf{e}$.
    {{< /tab >}}
{{< /tabs >}}

## Variants of Kepler's Equation

In a parabolic trajectory, Barker's equation relates the time of flight $t$ to the true anomaly $\theta$. If the time of periapsis is $\tau$, then

$$\tag{3.3.8} t - \tau = \sqrt{\frac{2a^3}{\mu}} \left( \tan \frac{\theta}{2} + \frac{1}{3} \tan^3 \frac{\theta}{2} \right)$$

This can be derived by the conservation of energy as follows:

$$\begin{aligned}
\varepsilon = 0 = \frac{v^2}{2} - \frac{\mu}{r} &\implies v = \sqrt{\frac{2\mu}{r}} \\
&\implies \frac{dr}{dt} = \sqrt{\frac{2\mu}{r} - \frac{h^2}{r^2}} \\
&\implies dt = \frac{dr}{\sqrt{\frac{2\mu}{r} - \frac{h^2}{r^2}}} \\
&\implies t - \tau = \int_{r_p}^r \frac{dr}{\sqrt{\frac{2\mu}{r} - \frac{h^2}{r^2}}} \\
&\implies t - \tau = \sqrt{\frac{2a^3}{\mu}} \left( \tan \frac{\theta}{2} + \frac{1}{3} \tan^3 \frac{\theta}{2} \right) \\
\end{aligned}$$

In going from line 1 to 2, we used the fact that the velocity can be decomposed into a radial component and a tangential component, and the tangential component is given by $v_\theta = \frac{h}{r}$. In going from line 4 to 5, we used the substitution $r = \frac{2a}{1 + \cos \theta}$.

In a hyperbolic trajectory, the hyperbolic Kepler's equation relates the mean anomaly $M$ to the hyperbolic anomaly $H$:

$$\tag{3.3.9} M = e \sinh H - H$$

where the mean anomaly is defined as $M = \sqrt{\frac{\mu}{-a^3}} (t - \tau)$. The true anomaly and hyperbolic anomaly are related by

$$\tag{3.3.10} \tan \frac{\theta}{2} = \sqrt{\frac{e + 1}{e - 1}} \tanh \frac{H}{2}$$

These equations can be derived in a similar fashion to the ordinary Kepler's equation, but with a few changes. The area of the hyperbolic sector is given by $A = \frac{1}{2} ab H$, while the area of the triangle formed by the radius vector and the asymptote is given by $A' = \frac{1}{2} ab \sinh H$. The mean anomaly is defined as $M = \sqrt{\frac{\mu}{-a^3}} (t - \tau)$, and the true anomaly and hyperbolic anomaly are related by $\tan \frac{\theta}{2} = \sqrt{\frac{e + 1}{e - 1}} \tanh \frac{H}{2}$.

## Radial trajectories

A radial parabolic trajectory is a degenerate case of a parabolic trajectory, where the eccentricity $e$ is still equal to 1, however the angular momentum of the system is zero. The trajectory is a straight line, and the two bodies move away from each other, the velocity tending to zero as they get infinity far away from each other. It is classified as a parabolic trajectory since the total energy of the system is zero.

The relative velocity of the two objects is always the escape velocity. The bodies could either be moving towards each other, or away from each other. In the former case, the two bodies will eventually collide, while in the latter case, they will move away from each other, and eventually come to rest at infinity.

The position of the body can be solved as a function of time by using conservation of energy. Let $t=0$ correspond to the time of closest approach, then

$$\tag{3.3.11} r = \sqrt[3]{\frac{9\mu t^2}{2}}$$

A radial hyperbolic trajectory is a degenerate case of a hyperbolic trajectory, where the eccentricity $e$ is equal to 1 and the angular momentum of the system is zero. The trajectory is a straight line, and the two bodies move away from each other, having a finite velocity at infinity. It is classified as a hyperbolic trajectory since the total energy of the system is positive.

The relative speed of the two objects is always greater than the escape velocity. How does the position of the body change with time now?

{{< tabs >}}
    {{< tab name="P2" >}}
    Find the position of a body moving in a radial hyperbolic trajectory as a function of time, $r(t)$, given that the time of closest approach is $t=0$, and the velocity at infinity is $v_\infty$.
    {{< /tab >}}

    {{< tab name="Solution" >}}
    We can solve this by conservation of energy $\varepsilon$.

    $$\begin{aligned}
    \varepsilon = \frac{v_\infty^2}{2} = \frac{v^2}{2} - \frac{\mu}{r} &\implies v = \sqrt{v_\infty^2 + \frac{2\mu}{r}} \\
    &\implies \frac{dr}{dt} = \sqrt{v_\infty^2 + \frac{2\mu}{r}} \\
    &\implies dt = \frac{dr}{\sqrt{v_\infty^2 + \frac{2\mu}{r}}} \\
    &\implies t = \int_{0}^r \frac{dr}{\sqrt{v_\infty^2 + \frac{2\mu}{r}}} \\
    \end{aligned}$$

    The integral can be carried out, and we get

    $$\tag{3.3.12} t = \frac{r}{v_\infty} \sqrt{1 + \frac{2\mu}{v_\infty^2 r}} - \frac{2\mu}{v_\infty^3} \ln \left( \sqrt{1 + \frac{2\mu}{v_\infty^2 r}} + 1 \right)$$
    {{< /tab >}}
{{< /tabs >}}
