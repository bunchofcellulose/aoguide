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
