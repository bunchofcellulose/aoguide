---
title: Coordinate Systems
weight: 2
---

In order to specify the position of objects in the sky, we need a way to be able to describe their exact location. This can be done by setting up a coordinate system, such that each point in the sky can be described by a pair of numbers. There are several coordinate systems used in astronomy, each with its own advantages and disadvantages. In this section, we will cover the most commonly used coordinate systems: horizontal (alt-az), equatorial, ecliptic and galactic.

## Horizontal (Alt-Az) Coordinate System

Any point in the sky can be described by its altitude and azimuth. The horizontal coordinate system is based on the observer's local horizon, with the zenith (the point directly above the observer) at $90^\circ$ altitude and the nadir (the point directly below the observer) at $-90^\circ$ altitude.

Any arc passing through the zenith and perpendicular to the horizon is called a vertical circle. The altitude $a$ of a point $X$ is the angle between the horizon and the point, as measured along the vertical circle passing through the point and the zenith. The zenith angle $z$ is the angle between the zenith and the point, which is equal to $90^\circ - a$. The altitude is positive above the horizon and negative below it. It ranges from $-90^\circ$ at the nadir to $90^\circ$ at the zenith.

The azimuth $A$ of a point $X$ is the angle between the north direction and the projection of the point onto the horizontal plane, measured eastwards from north. The azimuth ranges from $0^\circ$ at the north point, $90^\circ$ at the east point, $180^\circ$ at the south point, and $270^\circ$ at the west point. In the southern hemisphere, azimuth is measured from the south point eastwards.

The coordinates of a point in the horizontal coordinate system are given by the pair $(a, A)$, where $a$ is the altitude and $A$ is the azimuth. These change with the observer's location and the time of observation, as the position of celestial objects changes due to the rotation of the Earth.

## Equatorial Coordinate System

The equatorial coordinate system is based on the celestial equator, which is the projection of the Earth's equator onto the celestial sphere. The coordinates in this system are right ascension (RA/$\alpha$), hour angle (HA/$h$) and declination (Dec/$\delta$).

Any arc passing through the north celestial pole and perpendicular to the celestial equator is called an hour circle. The declination $\delta$ of a point $X$ is the angle between the celestial equator and the point, as measured along the hour circle passing through the point. It is positive above the celestial equator and negative below it. The declination ranges from $-90^\circ$ at the south celestial pole to $90^\circ$ at the north celestial pole.

The hour angle $h$ of a point $X$ is the angle between the observer's meridian (the hour circle passing through the observer's zenith) and the hour circle passing through the point, measured westwards from the observer's meridian. The hour angle is positive when the point is west of the observer's meridian and negative when it is east of it. The hour angle ranges from $-12$ hrs to $12$ hrs, with $0$ hrs at the observer's meridian.

The HA/Dec coordinates of a point change with the observer's location and the time of observation, as the position of celestial objects changes due to the rotation of the Earth. This is due to the fact that the hour angle is defined with respect to the observer's meridian. To remove this dependence, the right ascension (RA) can be used instead of the hour angle.

We first define the vernal equinox ♈︎ (also known as the first point of Aries) as the point where the ecliptic intersects the celestial equator, going from south to north. The autumnal equinox ♎︎ (also known as the first point of Libra) is the point where the ecliptic intersects the celestial equator, going from north to south.

The right ascension $\alpha$ of a point $X$ is the angle between the vernal equinox and the projection of the point onto the celestial equator, measured eastwards from the vernal equinox (opposite to the direction of measurement of the hour angle). The right ascension is positive eastwards from the vernal equinox and ranges from $0$ hrs at the vernal equinox, $6$ hrs at the summer solstice, $12$ hrs at the autumnal equinox, and $18$ hrs at the winter solstice.

The RA/Dec coordinates of a point are given by the pair $(\alpha, \delta)$, where $\alpha$ is the right ascension and $\delta$ is the declination. These coordinates do not depend on the location of the observer or the time of observation, as they are defined with respect to the celestial equator and the vernal equinox, which are fixed points on the celestial sphere.

### Circumpolar Stars

A star is said to be circumpolar if it never sets below the horizon for a given observer. For a star to be circumpolar, we must have

$$ \phi + \delta \geq 90^\circ $$

where $\phi$ is the observer's latitude and $\delta$ is the star's declination. If this condition is satisfied, the star will always be above the horizon, and its altitude will always be positive.

Some stars also never rise above the horizon. For a star to never rise above the horizon, we must have

$$ \phi - \delta \leq -90^\circ $$

where $\phi$ is the observer's latitude and $\delta$ is the star's declination. If this condition is satisfied, the star will always be below the horizon, and its altitude will always be negative.

### Culmination

A star is said to culminate when it is at the observer's meridian. There are two types of culmination: upper culmination and lower culmination.

The upper culmination occurs when the star is at its highest point in the sky, which corresponds to the moment when the star's hour angle is $0$ hrs. At this point, the altitude of the star is at its maximum, and it is directly south of the observer in the northern hemisphere (or directly north in the southern hemisphere).

The lower culmination occurs when the star is at its lowest point in the sky, which corresponds to the moment when the star's hour angle is $12$ hrs. At this point, the altitude of the star is at its minimum, and it is directly north of the observer in the northern hemisphere (or directly south in the southern hemisphere).

The maximum altitude or minimum zenith distance of a star (during upper culmination) can be calculated using the formula:

$$ a_{\text{max}} = 90^\circ - |\phi - \delta| $$
$$ z_{\text{min}} = |\phi - \delta| $$

where $\phi$ is the observer's latitude, and $\delta$ is the star's declination. If $a_{\text{max}} < 0$, the star will never culminate above the horizon. If $\phi > \delta$, the star will culminate in the south of zenith, and if $\phi < \delta$, it will culminate in the north of zenith.

The minimum altitude or maximum zenith distance of a star (during lower culmination) can be calculated using the formula:

$$ a_{\text{min}} = \phi + \delta - 90^\circ $$
$$ z_{\text{max}} = 180^\circ - (\phi + \delta) $$

If $a_{\text{min}} < 0$, the star will never culminate below the horizon.

## Ecliptic Coordinate System

The ecliptic coordinate system is based on the ecliptic plane, which is the plane of the Earth's orbit around the Sun. The coordinates in this system are ecliptic longitude ($\lambda$) and ecliptic latitude ($\beta$).

The ecliptic longitude $\lambda$ of a point $X$ is the angle between the vernal equinox and the projection of the point onto the ecliptic plane, measured eastwards from the vernal equinox. The ecliptic longitude is positive eastwards from the vernal equinox and ranges from $0^\circ$ at the vernal equinox, $90^\circ$ at the summer solstice, $180^\circ$ at the autumnal equinox, and $270^\circ$ at the winter solstice.

The ecliptic latitude $\beta$ of a point $X$ is the angle between the point and the ecliptic plane, measured northwards from the ecliptic plane. The ecliptic latitude is positive northwards from the ecliptic plane and ranges from $-90^\circ$ (the south ecliptic pole) to $90^\circ$ (the north ecliptic pole).

The ecliptic coordinates of a point are given by the pair $(\lambda, \beta)$, where $\lambda$ is the ecliptic longitude and $\beta$ is the ecliptic latitude. These coordinates do not depend on the location of the observer or the time of observation, as they are defined with respect to the ecliptic plane and the vernal equinox, which are fixed points on the celestial sphere.

The geocentric ecliptic coordinates are the ecliptic coordinates of a point as seen from the center of the Earth, while the heliocentric ecliptic coordinates are the ecliptic coordinates of a point as seen from the center of the Sun. The two coordinate systems are equal only if the object is very far away. The geocentric coordinates moreover depend on Earth's position in its orbit around the Sun.

## Galactic Coordinate System

The galactic coordinate system is based on the plane of the Milky Way galaxy. The coordinates in this system are galactic longitude ($l$) and galactic latitude ($b$).

The galactic longitude $l$ of a point $X$ is the angle between the galactic center and the projection of the point onto the galactic plane, measured eastwards from the galactic center. The galactic longitude is positive eastwards from the galactic center and ranges from $0^\circ$ at the galactic center, $90^\circ$ at the first galactic quadrant, $180^\circ$ at the second galactic quadrant, and $270^\circ$ at the third galactic quadrant.

The galactic latitude $b$ of a point $X$ is the angle between the point and the galactic plane, measured northwards from the galactic plane. The galactic latitude is positive northwards from the galactic plane and ranges from $-90^\circ$ (the south galactic pole) to $90^\circ$ (the north galactic pole).

The north galactic pole (NGP) is the point in the sky that is perpendicular to the plane of the Milky Way galaxy, and is located at the coordinates $(\alpha_G, \delta_G) = (12^h 51.4^m, 27^\circ 8')$ in the equatorial coordinate system.

The zero point $L$ of galactic longitude is defined as the direction towards the galactic center, which is located in the constellation Sagittarius. The zero point of galactic latitude is defined as the plane of the Milky Way galaxy. It is such that the angle $\theta = \angle PGL \approx 123.0^\circ$, where $PGL$ is the position of the galactic north pole in the equatorial coordinate system.

## Transformation Between Coordinate Systems

The easiest way to transform between coordinate systems is to draw a spherical diagram and apply formulae of spherical trigonometry.

### Horizontal and Equatorial

To interconvert between horizontal coordinates $(a, A)$ and equatorial coordinates $(h, \delta)$, given the observer's latitude $\phi$, we use the following formulae:

$$\begin{align*}
\sin A \cos a &= \sin h \cos \delta \\
\cos A \cos a &= \cos h \cos \delta \sin \phi - \sin \delta \cos \phi \\
\sin a &= \cos h \cos \delta \cos \phi + \sin \delta \sin \phi
\\ \\
\sin h \cos \delta &= \sin A \cos a \\
\cos h \cos \delta &= \cos A \cos a + \sin a \cos \phi \\
\sin \delta &= - \cos a \cos A \cos \phi + \sin a \sin \phi
\end{align*}$$

### Equatorial and Ecliptic

To interconvert between equatorial coordinates $(\alpha, \delta)$ and ecliptic coordinates $(\lambda, \beta)$, we use the following formulae:

$$\begin{align*}
\sin \alpha \cos \delta &= - \sin \beta \sin \varepsilon + \cos \beta \cos \varepsilon \sin \lambda \\
\cos \alpha \cos \delta &= \cos \beta \cos \lambda \\
\sin \delta &= \sin \beta \cos \varepsilon + \cos \beta \sin \varepsilon \sin \lambda
\\ \\
\sin \lambda \cos \beta &= \sin \delta \sin \varepsilon + \cos \delta \cos \varepsilon \sin \alpha \\
\cos \lambda \cos \beta &= \cos \delta \cos \alpha \\
\sin \beta &= \sin \delta \cos \varepsilon - \cos \delta \sin \varepsilon \sin \alpha
\end{align*}$$

where $\varepsilon$ is the axial tilt of the Earth, which is approximately $23.44^\circ$.

### Equatorial to Galactic

To convert from equatorial coordinates $(\alpha, \delta)$ to galactic coordinates $(l, b)$, we use the following formulae:

$$\begin{align*}
\sin (\theta - l) \cos b &= \cos \delta \sin (\alpha - \alpha_G) \\
\cos (\theta - l) \cos b &= - \cos \delta \cos \delta_G \ cos (\alpha - \alpha_G) + \sin \delta \sin \delta_G \\
\sin b &= \cos \delta \cos \delta_G \cos (\alpha - \alpha_G) + \sin \delta \sin \delta_G
\end{align*}$$

where $\theta = 123.0^\circ$ is the angle between the galactic north pole and the vernal equinox, and $(\alpha_G, \delta_G) = (12^h 51.4^m, 27^\circ 8')$ are the coordinates of the galactic north pole in the equatorial coordinate system.
