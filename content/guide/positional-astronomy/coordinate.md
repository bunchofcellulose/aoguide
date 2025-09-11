---
title: Coordinate Systems
weight: 2
---

In order to specify the position of objects in the sky, we need a way to be able to describe their exact location. This can be done by setting up a coordinate system, such that each point in the sky can be described by a pair of numbers. There are several coordinate systems used in astronomy, each with its own advantages and disadvantages. In this chapter, we will cover the most commonly used ones: horizontal (alt-az), equatorial, ecliptic and galactic.

## Horizontal (Alt-Az) Coordinate System

Any point in the sky can be described by its altitude $a$ and azimuth $A$. The horizontal coordinate system is based on the observer's local horizon, with the zenith (the point directly above the observer) at $90^\circ$ altitude and the nadir (the point directly below the observer) at $-90^\circ$ altitude.

An arc passing through the zenith and perpendicular to the horizon is called a vertical circle. The altitude $a$ of a point $X$ is the angle between the horizon and the point, as measured along the vertical circle passing through that point. The zenith angle $z$ is the angle between the zenith and the point, equal to the complement of the altitude

$$\tag{1.2.1} z = 90^\circ - a$$

The altitude is positive above the horizon and negative below it, ranging from $-90^\circ$ at the nadir to $90^\circ$ at the zenith.

The azimuth $A$ of a point $X$ is the angle between the north cardinal point and the projection of the point $X$ onto the horizontal plane. The azimuth starts from $0^\circ$ at the north point and increases eastwards, $90^\circ$ at the east point, $180^\circ$ at the south point, and $270^\circ$ at the west point. In the southern hemisphere, azimuth is measured from the south point eastwards.

{{< callout type="image" >}}
{{< svg "pos/altaz.svg" "Altitude-Azimuth Coordinate System" "The altitude-azimuth coordinate system is based on the observer's local horizon." >}}
{{< /callout >}}

The coordinates of a point in the horizontal coordinate system are given by the pair $(a, A)$, where $a$ is the altitude and $A$ is the azimuth. These change with the observer's location and the time of observation.

## Equatorial Coordinate System

The equatorial coordinate system is based on the celestial equator, which is the projection of the Earth's equator onto the celestial sphere. The coordinates in this system are right ascension (RA/$\alpha$), hour angle (HA/$h$) and declination (Dec/$\delta$).

An arc passing through the north celestial pole and perpendicular to the celestial equator is called an hour circle. The declination $\delta$ of a point $X$ is the angle between the celestial equator and the point, as measured along the hour circle passing through that point. It is positive above the celestial equator and negative below it ranging from $-90^\circ$ at the south celestial pole to $90^\circ$ at the north celestial pole.

The hour angle $h$ of a point $X$ is the angle between the observer's meridian (the hour circle passing through the observer's zenith) and the hour circle passing through the point $X$. The hour angle is positive when the point is west of the observer's meridian and negative when it is east of it, ranging from $-12^h$ to $12^h$, with $0^h$ at the observer's meridian.

The hour angle can also be interpreted as the time since the point $X$ last crossed the observer's meridian, or the time since its upper culmination.

{{< callout type="remark" >}}
The Earth rotates $360^\circ$ in $24$ hours, so the hour angle increases by $15^\circ$ per hour. To convert between degrees and hours, we use the conversion factor $1^h = 15^\circ$.
{{< /callout >}}

The hour angle of a point changes with the observer's location and the time of observation. This is due to the fact that the hour angle is defined with respect to the observer's meridian. To remove this dependence, the right ascension (RA) is introduced.

We first define the equinoxes: the equinoxes are the two points where the ecliptic intersects the celestial equator. The vernal equinox ♈︎ (also known as the first point of Aries) is the point where Sun (moving along the ecliptic) crosses the celestial equator from south to north. The autumnal equinox ♎︎ (also known as the first point of Libra) is the point where Sun crosses the celestial equator from north to south. These two points are fixed on the celestial sphere and do not depend on the observer's location or the time of observation.

The right ascension $\alpha$ of a point $X$ is the angle between the vernal equinox and the projection of the point $X$ onto the celestial equator. The right ascension starts from the vernal equinox at $0^h$ and increases eastwards (opposite to the direction of increasing hour angle), $6^h$ at the summer solstice, $12^h$ at the autumnal equinox, and $18^h$ at the winter solstice.

The conversion from hour angle to right ascension will be discussed in chapter 1.3.

The RA/Dec coordinates of a point are given by the pair $(\alpha, \delta)$, where $\alpha$ is the right ascension and $\delta$ is the declination. These coordinates do not depend on the location of the observer or the time of observation, as they are defined with respect to the celestial equator and the vernal equinox, which are fixed points on the celestial sphere.

### Culmination

A star is said to culminate when it is at the observer's meridian.

The upper culmination occurs when the star is at its highest point in the sky, which corresponds to the moment when the star's hour angle is $0^h$. At this point, the altitude of the star is at its maximum, and it is directly south of the observer in the northern hemisphere (or directly north in the southern hemisphere).

The lower culmination occurs when the star is at its lowest point in the sky, which corresponds to the moment when the star's hour angle is $12^h$. At this point, the altitude of the star is at its minimum, and it is directly north of the observer in the northern hemisphere (or directly south in the southern hemisphere).

The maximum altitude or minimum zenith distance of a star (during upper culmination) can be calculated using the formula:

$$\tag{1.2.2} a_{\text{max}} = 90^\circ - |\phi - \delta| $$
$$\tag{1.2.3} z_{\text{min}} = |\phi - \delta| $$

where $\phi$ is the observer's latitude, and $\delta$ is the star's declination. If $a_{\text{max}} < 0$, the star will never rise above the horizon for the observer. If $\phi > \delta$, the star will culminate south of zenith, and if $\phi < \delta$, it will culminate north of zenith.

The minimum altitude or maximum zenith distance of a star (during lower culmination) can be calculated using the formula:

$$\tag{1.2.4} a_{\text{min}} = \phi + \delta - 90^\circ $$
$$\tag{1.2.5} z_{\text{max}} = 180^\circ - (\phi + \delta) $$

If $a_{\text{min}} > 0$, the star is circumpolar and will never set, as discussed in the following section.

### Circumpolar Stars

A star is said to be circumpolar if it never sets below the horizon. For a star to be circumpolar, we must have

$$\tag{1.2.6} \phi + \delta \geq 90^\circ $$

where $\phi$ is the observer's latitude and $\delta$ is the star's declination. This can be derived from the $a_\text{min} > 0$ condition from the previous section.

Some stars never rise above the horizon. For a star to never rise above the horizon, we must have

$$\tag{1.2.7} \phi - \delta \leq -90^\circ $$

where $\phi$ is the observer's latitude and $\delta$ is the star's declination. This can be derived from the $a_\text{max} < 0$ condition from the previous section.

## Ecliptic Coordinate System

The ecliptic coordinate system is based on the ecliptic plane, which is the plane of the Earth's orbit around the Sun. The coordinates in this system are the ecliptic longitude $\lambda$ and the ecliptic latitude $\beta$.

The ecliptic longitude $\lambda$ of a point $X$ is the angle between the vernal equinox and the projection of the point onto the ecliptic plane. The ecliptic longitude starts from the vernal equinox at $0^\circ$ and increases eastwards, $90^\circ$ at the summer solstice, $180^\circ$ at the autumnal equinox, and $270^\circ$ at the winter solstice.

The ecliptic latitude $\beta$ of a point $X$ is the angle between the point and the ecliptic plane. The ecliptic latitude is positive northwards from the ecliptic plane and ranges from $-90^\circ$ at the south ecliptic pole to $90^\circ$ at the north ecliptic pole.

The ecliptic coordinates of a point are given by the pair $(\lambda, \beta)$, where $\lambda$ is the ecliptic longitude and $\beta$ is the ecliptic latitude. These coordinates do not depend on the location of the observer or the time of observation, as they are defined with respect to the ecliptic plane and the vernal equinox, which are fixed points on the celestial sphere. This coordinate system is particularly useful for describing the positions of objects in the solar system, as their orbits are generally close to the ecliptic plane.

The geocentric ecliptic coordinates are the ecliptic coordinates of a point as seen from the center of the Earth, while the heliocentric ecliptic coordinates are the ecliptic coordinates of a point as seen from the center of the Sun. The two coordinate systems are equal only if the object is very far away. The geocentric coordinates moreover depend on Earth's position in its orbit around the Sun, while the heliocentric coordinates do not.

## Galactic Coordinate System

The galactic coordinate system is based on the plane of the Milky Way galaxy. The coordinates in this system are galactic longitude $l$ and galactic latitude $b$.

The galactic longitude $l$ of a point $X$ is the angle between the galactic center and the projection of the point onto the galactic plane. The galactic longitude is measured eastwards from the Sun and starts from $0^\circ$ at the galactic center, $90^\circ$ at the first galactic quadrant, $180^\circ$ at the second galactic quadrant, and $270^\circ$ at the third galactic quadrant.

The galactic latitude $b$ of a point $X$ is the angle between the point and the galactic plane, measured northwards from the galactic plane. It ranges from $-90^\circ$ at the south galactic pole to $90^\circ$ at the north galactic pole.

The north galactic pole (NGP) is the point in the sky that is perpendicular to the plane of the Milky Way galaxy. Its equatorial coordinates are $(\alpha_G, \delta_G) = (12^h 51.4^m, 27^\circ 8')$.

The zero point of galactic longitude $L$ is defined as the direction towards the galactic center, located in the constellation Sagittarius. The zero point of galactic latitude is defined as the plane of the Milky Way galaxy. It is such that the angle $\theta = \angle PGL \approx 123.0^\circ$, where $PGL$ is the position of the galactic north pole in the equatorial coordinate system.

## Transformation Between Coordinate Systems

The easiest way to transform between coordinate systems is to draw a spherical diagram and apply the identities of spherical trigonometry.

### Horizontal and Equatorial

To interconvert between horizontal coordinates $(a, A)$ and equatorial coordinates $(h, \delta)$, given the observer's latitude $\phi$, we use the following identities:

$$
\tag{1.2.8}
\begin{align*}
\sin A \cos a &= \sin h \cos \delta \\
\cos A \cos a &= -\cos h \cos \delta \sin \phi + \sin \delta \cos \phi \\
\sin a &= \cos h \cos \delta \cos \phi + \sin \delta \sin \phi
\\ \\ \tag{1.2.9}
\sin h \cos \delta &= \sin A \cos a \\
\cos h \cos \delta &= -\cos A \cos a + \sin a \cos \phi \\
\sin \delta &= \cos a \cos A \cos \phi + \sin a \sin \phi
\end{align*}$$

### Equatorial and Ecliptic

To interconvert between equatorial coordinates $(\alpha, \delta)$ and ecliptic coordinates $(\lambda, \beta)$, we use the following identities:

$$
\tag{1.2.10}
\begin{align*}
\sin \alpha \cos \delta &= - \sin \beta \sin \varepsilon + \cos \beta \cos \varepsilon \sin \lambda \\
\cos \alpha \cos \delta &= \cos \beta \cos \lambda \\
\sin \delta &= \sin \beta \cos \varepsilon + \cos \beta \sin \varepsilon \sin \lambda
\\ \\ \tag{1.2.11}
\sin \lambda \cos \beta &= \sin \delta \sin \varepsilon + \cos \delta \cos \varepsilon \sin \alpha \\
\cos \lambda \cos \beta &= \cos \delta \cos \alpha \\
\sin \beta &= \sin \delta \cos \varepsilon - \cos \delta \sin \varepsilon \sin \alpha
\end{align*}$$

where $\varepsilon \approx 23.44^\circ$ is the axial tilt of the Earth.

### Equatorial to Galactic

To convert from equatorial coordinates $(\alpha, \delta)$ to galactic coordinates $(l, b)$, we use the following identities:

$$
\tag{1.2.12}
\begin{align*}
\sin (\theta - l) \cos b &= \cos \delta \sin (\alpha - \alpha_G) \\
\cos (\theta - l) \cos b &= - \cos \delta \cos \delta_G \cos (\alpha - \alpha_G) + \sin \delta \sin \delta_G \\
\sin b &= \cos \delta \cos \delta_G \cos (\alpha - \alpha_G) + \sin \delta \sin \delta_G
\end{align*}$$

where $\theta \approx 123.0^\circ$ is the angle between the galactic north pole and the vernal equinox, and $(\alpha_G, \delta_G) = (12^h 51.4^m, 27^\circ 8')$ are the coordinates of the galactic north pole in the equatorial coordinate system.

## Problems

{{< tabs items="P1" >}}
    {{< tab >}}

    Derive all the coordinate system transformation identities stated in the section above using spherical trigonometry.

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P2,Solution" >}}
    {{< tab >}}

    Find the hour angle of an object $X$ with declination $\delta$, when it rises and sets for an observer at latitude $\phi$. From this find the time the object is above the horizon.

    {{< /tab >}}
    {{< tab >}}

    At the time of rising or setting, the altitude of the object is $a = 0^\circ$. Using the equation (1.2.8.3):

    $$\sin a = \cos h \cos \delta \cos \phi + \sin \delta \sin \phi$$
    $$\tag{1.2.13} \implies \boxed{\cos h = - \tan \delta \tan \phi}$$

    This is a very important result and is used often in positional astronomy. For rising, $h$ is negative, and for setting, $h$ is positive. The time the object is above the horizon is given by

    $$\Delta t = h_\text{set} - h_\text{rise} = 2 \cos^{-1} (- \tan \delta \tan \phi)$$

    where $\Delta t$ is in hours.

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P3,Solution" >}}
    {{< tab >}}

    Find the azimuth of an object $X$ with declination $\delta$, when it rises and sets for an observer at latitude $\phi$.

    {{< /tab >}}
    {{< tab >}}

    At the time of rising or setting, the altitude of the object is $a = 0^\circ$. Using the equation (1.2.8.2) and (1.2.13):

    $$\cos A \cos a = - \cos h \cos \delta \sin \phi + \sin \delta \cos \phi$$
    $$\implies \cos A = \tan \phi \tan \delta \cos \delta \sin \phi + \sin \delta \cos \phi$$
    $$\tag{1.2.14} \implies \boxed{\cos A = \frac{\sin \delta}{\cos \phi}}$$

    This result too is often used in solving problems. The azimuth at rising is between $0^\circ$ and $180^\circ$, and at setting is between $180^\circ$ and $360^\circ$.

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P3,Solution" >}}
    {{< tab >}}

    Calculate the azimuths of the star Procyon ($\delta = 5^\circ$ N) when its zenith distance is $80^\circ$ as seen by an observer in latitude $56^\circ$ N.

    {{< /tab >}}
    {{< tab >}}

    A zenith distance of $80^\circ$ corresponds to an altitude of $10^\circ$. Using the equation (1.2.9.3):

    $$\sin \delta = \cos a \cos A \cos \phi + \sin a \sin \phi$$
    $$\implies \cos A = \frac{\sin \delta - \sin a \sin \phi}{\cos a \cos \phi}$$
    $$= \frac{\sin 10^\circ \sin 56^\circ - \sin 5^\circ}{\cos 10^\circ \cos 56^\circ}$$
    $$\approx -0.103$$

    Thus the possible azimuths are $A  = 96^\circ$ or $A = 264^\circ$.

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P4,Solution" >}}
    {{< tab >}}

    Given that $h_1$, $h_2$ are the hour angles of a star of declination $\delta$ on the prime vertical west and at setting respectively for an observer in north latitude, show that

    $$\cos h_1 \cos h_2 + \tan^2 \delta = 0$$

    {{< /tab >}}
    {{< tab >}}

    From equation (1.2.13), at the time of setting the hour angle is given by

    $$\tag{1} \cos h_2 = - \tan \delta \tan \phi$$

    When the star is on the prime vertical west, its azimuth is $A = 270^\circ$. Using the equation (1.2.8.2)

    $$\cos A \cos a = - \cos h \cos \delta \sin \phi + \sin \delta \cos \phi$$
    $$\implies 0 = - \cos h_1 \cos \delta \sin \phi + \sin \delta \cos \phi$$
    $$\tag{2} \implies \cos h_1 = \tan \delta \cot \phi$$

    Thus from (1) and (2) we get

    $$\boxed{\cos h_1 \cos h_2 + \tan^2 \delta = 0}$$

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P5,Solution" >}}
    {{< tab >}}

    A star has declination $\delta$ and is seen by an observer located in the northern hemisphere at latitude $\phi < \delta$. Find the maximum azimuth of the star as seen by the observer.

    {{< /tab >}}
    {{< tab >}}

    Since $\phi < \delta$, the star has both its upper culmination and lower culmination in the north of zenith, and thus can never achieve all values of the azimuth. To find the maximum azimuth, we draw a spherical triangle with vertices at the north celestial pole $P$, the zenith $Z$ and the star $X$. We know two sides and two angles of the triangle

- $PZ = 90^\circ - \phi$
- $PX = 90^\circ - \delta$
- $\angle PZX = A$
- $\angle ZXP = 90^\circ$

    Using sine rule, we have

    $$\frac{\sin A}{\sin (90^\circ - \delta)} = \frac{\sin 90^\circ}{\sin (90^\circ - \phi)}$$
    $$\implies \sin A = \frac{\cos \delta}{\cos \phi}$$

    Thus the maximum azimuth seen is $\boxed{A = \sin^{-1} (\cos \delta \sec \phi)}$

    {{< /tab >}}
{{< /tabs >}}

{{< tabs items="P6,Solution" >}}
    {{< tab >}}

    Regulus (α Leo) is the brightest star in the constellation Leo. It appears to be a single star to the naked eye, but is actually a quadruple star system, composed of four stars that are organized into two pairs. One of the stars, Regulus A, has equatorial coordinates $(\alpha, \delta) = (10^h 8^m, 11^\circ 58' \text{ N})$. Calculate the ecliptic coordinates of Regulus A.

    {{< /tab >}}
    {{< tab >}}

    We are given that $\delta = 11^\circ 58'$ and $\alpha = 10^h 8^m$. Thus using the equations (1.2.11), we have

    $$
    \begin{align*}
    \sin \lambda \cos \beta &\approx 0.5038 \\
    \cos \lambda \cos \beta &\approx -0.8640 \\
    \sin \beta &\approx 0.0075
    \end{align*}
    $$

    From these, we get $\boxed{(\lambda, \beta) = (9^h 59^m, 0^\circ 26')}$. Since the ecliptic latitude is very small, we conclude that Regulus A lies very close to the ecliptic plane.

    {{< /tab >}}
{{< /tabs >}}
