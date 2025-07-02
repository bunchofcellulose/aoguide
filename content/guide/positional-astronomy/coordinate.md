---
title: Coordinate Systems
weight: 2
---

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
