---
title: Advanced Topics
weight: 7
---

## Path of Stick's Shadow

Consider the path the shadow of a vertical stick traces out during a day, as the Sun moves across the sky. The shape traced out the by the shadow is a conic section - an ellipse, parabola, or hyperbola - depending on the position of the Sun relative to the observer.

Let the latitude of the observer be $\phi$ and the declination of the Sun be $\delta$. The length of the shadow of a unit length stick when the altitude of the Sun is $a$ is

$$ l = \frac{1}{\tan a} $$

We setup our coordinate system with the stick at the origin, the $x$-axis pointing east, and the $y$-axis pointing north. The angle the shadow makes with the north is just the azimuth of the Sun, $A$. Thus

$$ x = l \sin A = \frac{\sin A}{\tan a} $$
$$ y = l \cos A = \frac{\cos A}{\tan a} $$

Using transformation formulae, we get

$$\begin{align*}
\sin A \cos a &= \sin h \cos \delta \\
\cos A \cos a &= \cos h \cos \delta \sin \phi - \sin \delta \cos \phi \\
\sin a &= \cos h \cos \delta \cos \phi + \sin \delta \sin \phi
\end{align*}$$

Substituting these into the equations for $x$ and $y$, we get

$$ x = \frac{\sin h }{\cos \phi (\cos h + \tan \delta \tan \phi)} $$
$$ y = \frac{\cos h \tan \phi - \tan \delta}{\cos h + \tan \delta \tan \phi} $$

Eliminating the hour angle $h$, we get

$$ \frac{\tan^2 \delta}{\cos^2 \phi} y^2 = x^2 (1 - \tan^2 \phi \tan^2 \delta) - 2 \frac{\tan \phi}{\cos^2 \delta} x + \tan^2 \phi - \tan^2 \delta $$

which is the equation of a conic section. The type of conic section depends on the values of $\phi$ and $\delta$.

- Circle: $\phi = \frac{\pi}{2}$
- Line: $\delta = 0$
- Point: $\delta = \frac{\pi}{2}$
- Ellipse: $\phi + \delta > \frac{\pi}{2}$
- Parabola: $\phi + \delta = \frac{\pi}{2}$
- Hyperbola: $\phi + \delta < \frac{\pi}{2}$

If $\phi = \delta$, Sun passes through the zenith at noon, and there is no shadow.

## Analemma

Analemma is the shape created by plotting the position of the Sun in the sky at the same civil time each day over the course of a year. The shape resembles a figure-eight and is a result of the tilt of the Earth's axis and its elliptical orbit around the Sun.

The northernmost and southernmost points of the analemma are the solstices. Deviation from the arc joining these points is due to the difference between the true sun and the mean sun.

If the axial tilt $\varepsilon$ is zero, the analemma would become an arc of a great circle. If the eccentricity $e$ of the orbit is zero, it will become a perfect figure-eight. If both are zero, the analemma will be a single point.

The following requires knowledge of kepler's laws and orbital anomalies, covered in the Celestial Mechanics section.

When viewed from different locations and at different times of the day, the position of the analemma and its orientation changes, however the shape remains the same. Thus without loss of generality, assume the observer is at the north pole, and the sun's position is measured at noon. The altitude of the Sun will just be its declination $\delta$, and its azimuth will be the difference in the right ascension of the Sun and the Mean Sun. Since the Mean Sun moves at a constant rate, its right ascension is just its mean anomaly $M$. Let the ecliptic longitude of the Sun be $\lambda$, and its true anomaly be $\theta$. These two are related by

$$ \lambda = \theta - \theta_0 $$

where $\theta_0$ is the true anomaly of the vernal equinox. The true anomaly is related to the mean anomaly by

$$ \int_{\theta_0}^{\theta} \frac{d\theta}{(1 + e \cos \theta)^2} = \frac{M}{(1-e^2)^{3/2}} $$

where $e$ is the eccentricity of the orbit. This relation can be derived using Kepler's second law.

Using conversion formulae, we can get the declination and right ascension of the Sun in terms of the ecliptic longitude:

$$\begin{align*}
\sin \alpha \cos \delta &= \cos \varepsilon \sin \lambda \\
\cos \alpha \cos \delta &= \cos \lambda \\
\sin \delta &= \sin \varepsilon \sin \lambda \\
\end{align*}$$

Since the time period of the Sun and Mean Sun is the same, their mean anomaly too is the same. Thus the altitude and azimuth of the Sun is

$$ (a, A) = (\delta, \alpha - M) $$

Examining closely, we see that the azimuth $\alpha - M$ is just the equation of time, which is the difference between the true solar time and the mean solar time. Also we find that the altitude difference between the lowest and highest points of the analemma is equal to twice the axial tilt of the Earth, $2\varepsilon$.
