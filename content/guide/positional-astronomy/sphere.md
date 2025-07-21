---
title: The Sphere
weight: 1
prev: /guide/positional-astronomy/
---

## Geometry of the Sphere

The geometry of the sphere is made up of great circles, small circles and arcs of these figures. Distances along great circles are often measured as angles since, for convenience, the radius of the sphere is made unity.

A great circle is defined to be the intersection with the sphere of a plane containing the centre of the sphere. Since the centre is equidistant from all points on the sphere, the figure of intersection must be a circle by definition. If the plane does not pass through the centre, the intersection is a small circle. The great circles are the largest circles on the sphere and divide it into two equal hemispheres. The small circles are smaller than the great circles and do not divide the sphere into equal parts.

The two points equidistant at $90^\circ$ from a great circle are called the poles of the great circle.

{{< svg "pos/gc.svg" "Poles of a Great Circle" "Poles of a Great Circle" >}}

If three great circles intersect one another so that a closed fgiure is formed by three arcs of the great circles, it is called a spherical triangle provided that it possesses the following properties:

- Any two sides are together greater than the third side
- The sum of the three angles is greater than $180^\circ$
- Each spherical angle is less than $180^\circ$

The sides of a spherical triangle are expressed in angular measure.

{{< svg "pos/sphtri.svg" "Spherical Triangle" "Spherical Triangle ABC formed by the intersections of great circles" >}}

The sides of the triangle are denoted by $a$, $b$, and $c$ and the angles by $A$, $B$, and $C$. The sides are the arcs of the great circles, while the angles are the angles between the planes of the great circles. For example, angle $A$ is the angle $\angle BAC$ and side $a$ is the arc $BC$.

It is often useful to remember the following identity:

$$\boxed{1 ^c \approx 206265.4 '' \approx 57.3^\circ}$$

$$ 1^\circ = 60' = 3600'' $$

where $1 ^c$ is one radian of arc, $''$ is seconds of arc, $'$ is minutes of arc, and $^\circ$ is degrees of arc.

The shortest distance between two points on the surface of a sphere is along a great circle. This distance is called the arc of the great circle, and is measured in angular units. The angle subtended at the centre of the sphere by the arc is called the central angle.

Often we are interested in the sides or angles of spherical triangles. We use formulas for spherical trigonometry to find these values. The most commonly used formulas are the following:

- The Law of Cosines:
  
    $$\cos a = \cos b \cos c + \sin b \sin c \cos A$$
- The Law of Sines:

    $$\frac{\sin a}{\sin A} = \frac{\sin b}{\sin B} = \frac{\sin c}{\sin C}$$
- The analogue of the cosine formula:

    $$\sin a \cos B = \cos b \sin c - \sin b \cos c \cos A$$
- The Four Parts Formula:

    $$\cos a \cos C = \sin a \cot b - \sin C \cot B$$

When the sides are small, the spherical triangle can be approximated by a plane triangle. In this case, the formulas for spherical trigonometry reduce to the familiar formulas of plane trigonometry.

The spherical excess of a spherical triangle is defined as

$$E = A + B + C - \pi$$

The area of the spherical triangle is then given by

$$\text{Area} = E \cdot R^2$$

where $R$ is the radius of the sphere. The radius is often taken to be unity, in which case the area is simply the spherical excess.

## Geometry of the Earth

The shape of the Earth is termed as a geoid, and is roughly an oblate spheroid, meaning it is slightly flattened at the poles and bulging at the equator. The radius of the Earth varies depending on where it is measured, with the equatorial radius being about 6,378 km and the polar radius being about 6,357 km. For most astronomical calculations, however, the Earth is treated as a perfect sphere with a mean radius of approximately 6,371 km.

A point on the surface of the Earth can be specified by its latitude and longitude. Latitude is the angle between the equatorial plane and a line drawn from the centre of the Earth to the point, while longitude is the angle between the prime meridian (defined as the great circle passing through the north and south poles, and the Royal Observatory in Greenwich, England) and a great circle passing through the point and the poles.

Due to non-spherical shape of the Earth, there are multiple definitions of latitude, as follows:

- Geodetic Latitude: The angle between the equatorial plane and the normal to the surface of the ellipsoid at the point.
- Geocentric Latitude: The angle between the equatorial plane and a line drawn from the centre of the Earth to the point.
- Astronomical Latitude: The angle between the equatorial plane and the vertical direction at the point, as determined by a plumb line.

Usually, unless explicitly stated, the term latitude refers to geodetic latitude. The difference between geodetic and geocentric latitude is small, but can be significant for precise measurements.

Latitude is measured in degrees, with the equator at $0^\circ$, the north pole at $90^\circ$ north, and the south pole at $90^\circ$ south. Sometimes the directions are dropped, and negative values are used to indicate southern latitudes , i.e., $-90^\circ$ latitude is the south pole.

Longitude is also measured in degrees, with the prime meridian at $0^\circ$, and increasing westwards up to $360^\circ$. They are usually expressed in the range $0^\circ$ to $180^\circ$ E and $0^\circ$ to $180^\circ$ W, or alternatively as negative values for eastern longitudes, i.e., $-180^\circ$ longitude is the same as $180^\circ$ W.

The co-latitude is defined as the complement of the latitude, i.e.,

$$\text{co-latitude} = 90^\circ - \text{latitude}$$

The flattening, or ellipticity, of the Earth is defined as

$$f = \frac{a - b}{a}$$

where $a$ is the equatorial radius and $b$ is the polar radius. The flattening of the Earth is approximately $1/298.257$.

The geodetic latitude $\phi$ is related to the geocentric latitude $\theta$ by the formula

$$\tan \phi = (1 - f)^2 \tan \theta$$

Two locations having the same latitude are said to be on the same parallel of latitude, while two locations having the same longitude are said to be on the same meridian. The distance between two points on the same parallel of latitude is called departure, and is given by

$$d = R \Delta \lambda \, \cos \phi$$

where $R$ is the radius of the Earth, $\phi$ is the latitude, and $\Delta \lambda$ is the difference in longitude between the two points. Note that the departure is not the shortest distance between the two points, as it is measured along the parallel of latitude, which is a small circle.

{{< svg "pos/departure.svg" "Departure between two points" "Distance along the small circle parallel to the Equator is the departure between AB, distance along the great circle is the shortest distance between AB" >}}

The distance between two points on the same meridian is given by

$$d = R \Delta \phi$$

where $\Delta \phi$ is the difference in latitude between the two points.

A nautical mile is the great circle distance subtending an angle of one minute of arc at the centre of the Earth.

{{< svg "pos/latlon.svg" "Latitude and Longitude" "Latitude of A is the angle AA', whereas the longitude difference between AB is the angle APB" >}}

## The Celestial Sphere

The celestial sphere is an imaginary sphere of infinite radius, concentric with the Earth, on which all celestial objects appear to be projected. The Earth is at the centre of this sphere, and the celestial objects are at the surface of the sphere. This is a useful tool as it allows us to represent the positions of celestial objects on a two-dimensional surface, without considering its distance from the observer.

The celestial spheres and all the objects (stars, galaxies, etc.) on it appear to rotate westwards overhead, around the Earth once nearly every 24 hours. This apparent motion is due to the rotation of the Earth on its axis. However, it makes no difference to the observer whether the celestial sphere is rotating around the Earth or the Earth is rotating on its axis. The point about which the celestial sphere appears to rotate is called the celestial pole. This is the projection of Earth's axis of rotation onto the celestial sphere. The two celestial poles are the north celestial pole (NCP) and the south celestial pole (SCP).

The north celestial pole is easily recognizable in the sky as it is very close to the bright star Polaris, also known as the North Star. The south celestial pole is located in the southern hemisphere and does not have a bright star associated with it, however one can approximately locate it by finding $\sigma$ Octantis, a faint star in the constellation Octans.

The celestial equator is the projection of the Earth's equator onto the celestial sphere. It divides the celestial sphere into the northern and southern celestial hemispheres, and is perpendicular to the line connecting the north and south celestial poles.

The Sun, when projected onto the celestial sphere, appears to move along a great circle in the course of a year. This great circle is called the ecliptic. The ecliptic is tilted at an angle of approximately $23.5^\circ$ to the celestial equator, which is due to the tilt of the Earth's axis of rotation relative to its orbit around the Sun. Sun's motion along the ecliptic is slow, much slower than the rotation of the celestial sphere, and thus can approximately be considered as a fixed point on the celestial sphere for short periods of time.

The poles of the ecliptic are the two points on the celestial sphere which are at $90^\circ$ from the ecliptic. The north ecliptic pole is located in the constellation Draco, while the south ecliptic pole is located in the constellation Dorado.

For an observer, the point on the celestial sphere directly overhead is called the zenith, while the point directly below is called the nadir. The line connecting the zenith and nadir is called the zenith-nadir line. The horizon is the great circle on the celestial sphere that is perpendicular to the zenith-nadir line. The points where the celestial equator intersects the horizon are called the east and west points.

The meridian of an observer is the great circle on the celestial sphere that passes through the zenith, nadir, and the north and south celestial poles. The points where the celestial equator intersects the meridian are called the north and south points.

{{< svg "pos/celsph.svg" "Celestial Sphere" "Celestial Sphere" >}}

In the above diagram, the north celestial pole is denoted by $P$, and the south celestial pole by $Q$. The north and south ecliptic poles are denoted by $K$ and $K'$, respectively. The zenith is denoted by $Z$, the nadir by $Z'$. The cardinal points are the east point $E$, and the west point $W$, the north point $N$ and the south point $S$.

The horizon is the great circle defined by the cardinal points $NWSEN$. The celestial equator is the other great circle passing through the east and west points. The meridian is the great circle passing through the zenith, nadir, north celestial pole and south celestial pole, defined by $ZPNZ'QSZ$ (This has not been labelled in the figure to avoid cluttering). The ecliptic is the great circle perpendicular to the north and south ecliptic poles, containing the Sun. Additionally, the great circle $ZEZ'W$ is called the prime vertical.
