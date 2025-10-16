---
title: The Sphere
weight: 1
prev: /guide/positional-astronomy/
---

## Geometry of the Sphere

The geometry of the sphere consists of great circles, small circles, and arcs of these figures. For convenience, the radius of the sphere is chosen to be unity. Thus, distances along great circles are often measured as angles the arcs subtend at the center.

A great circle is defined as the intersection of the sphere with a plane containing the center of the sphere. Thus, any circle on the sphere whose center coincides with the center of the sphere is a great circle. Since the center is equidistant from all points on the sphere, the figure of intersection must be a circle by definition. If the plane does not pass through the center, the intersection is a small circle. The great circles are the largest circles on the sphere and divide it into two equal hemispheres. The small circles are smaller than the great circles and do not divide the sphere into equal parts.

The two points equidistant at $90^\circ$ from a great circle are called the poles of the great circle.

{{< svg "pos/gc.svg" "Poles of a Great Circle" "Poles of a Great Circle" >}}

### Spherical Triangles

When three great circles intersect one another, a closed figure is formed by three arcs of the great circles, called a spherical triangle. All spherical triangles possess the following properties:

- The sum of the lengths of any two sides is greater than the third side
- The sum of the three angles is greater than $180^\circ$ but less than $540^\circ$
- Each spherical angle (internal angle of the spherical triangle) is less than $180^\circ$

The sides of a spherical triangle are expressed in angular measure.

{{< svg "pos/sphtri.svg" "Spherical Triangle" "Spherical Triangle ABC formed by the intersections of great circles" >}}

Let the sides of the triangle be denoted by $a$, $b$, and $c$ and the angles by $A$, $B$, and $C$. The sides are the arcs of the great circles, while the angles are the angles between the planes of the great circles. For example, angle $A$ is the angle $\angle BAC$ and side $a$ is the arc $BC$.

It is often useful to remember the following identities:

$$\tag{1.1.1} 1 ^c \approx 206265 '' \approx 57.3^\circ$$
$$\tag{1.1.2} 1^\circ = 60' = 3600'' $$

where $1 ^c$ is one radian of arc, $''$ is seconds of arc, $'$ is minutes of arc, and $^\circ$ is degrees of arc.

The shortest distance between two points on the surface of a sphere is along a great circle. This distance is called the arc of the great circle and is measured in angular units. The angle subtended at the center of the sphere by the arc is called the central angle.

### Spherical Trigonometry

Often we are interested in finding the sides or angles of spherical triangles. We use spherical trigonometry to find these. The most commonly used identities are the following:

- The Law of Cosines:
  
    $$\tag{1.1.3} \boxed{\cos a = \cos b \cos c + \sin b \sin c \cos A}$$
- The Law of Sines:

    $$\tag{1.1.4} \boxed{\frac{\sin a}{\sin A} = \frac{\sin b}{\sin B} = \frac{\sin c}{\sin C}}$$
- The analogue of the cosine formula:

    $$\tag{1.1.5} \boxed{\sin a \cos B = \cos b \sin c - \sin b \cos c \cos A}$$
- The Four Parts Formula:

    $$\tag{1.1.6} \boxed{\cos a \cos C = \sin a \cot b - \sin C \cot B}$$

When the sides are small, the spherical triangle can be approximated by a plane triangle. In this case, the formulas for spherical trigonometry reduce to the familiar formulas of plane trigonometry.

#### Polar Triangles

The polar triangle associated with a spherical triangle $ABC$ is defined as follows. Consider the great circle that contains the side $BC$. This great circle is defined by the intersection of a diametral plane with the surface. Draw the normal to that plane at the center: it intersects the surface at two points, and the point that is on the same side of the plane as $A$ is (conventionally) termed the pole of $A$ and is denoted by $A'$. The points $B'$ and $C'$ are defined similarly. The polar triangle of a polar triangle is the original triangle.

{{< svg "pos/polartri.svg" "Polar Triangle A'B'C' of the triangle ABC" "Polar triangle A'B'C' of the spherical triangle ABC" >}}

The angles and sides of the polar triangle are given by
$$
\tag{1.1.7}
\begin{align*}
    &A' = \pi - a, \qquad &B' = \pi - b, \qquad &C' = \pi - c \\
    &a' = \pi - A, \qquad &b' = \pi - B, \qquad &c' = \pi - C
\end{align*}
$$

These can be proven easily. Suppose $A'B'$ intersect great circle $BC$ at a point $D$, and $A'C'$ intersect great circle BC at point a $E$. We get

$$A' + a = DE + BC = DC + BE = \pi / 2 + \pi / 2 = \pi$$

So, $A' = \pi - a$. The other relations can be proved similarly. Note:

1. $A' = DE$ because $A'$ is the pole of great circle $DE$
2. $DC = \pi /2$ because $C$ is the pole of great circle $A'D$ (polar triangle of a polar triangle is the original triangle.)
3. $BE = \pi / 2$ because $B$ is the pole of great circle $A'E$ (polar triangle of a polar triangle is the original triangle.)

Therefore, if any identity is proved for the triangle $ABC$, then we can immediately derive a second identity by applying the first identity to the polar triangle by making the above substitutions. Similarly, the identities for a quadrantal triangle (one where a side is $90^\circ$) can be derived from those for a right-angled triangle (one where an angle is $90^\circ$). Thus, we get two additional identities:

- The Law of Cosines for angles:
  
    $$\tag{1.1.8} \cos A = - \cos B \cos C + \sin B \sin C \cos a$$
- The analogue of the cosine formula for angles:

    $$\tag{1.1.9} \sin A \cos b = \cos B \sin C + \sin B \cos C \cos a$$

#### Spherical Excess

The spherical excess of a spherical triangle is defined as

$$\tag{1.1.10} E = A + B + C - \pi$$

Using the spherical excess, we can find the area of the spherical triangle:

$$\tag{1.1.11} \text{Area} = E \cdot R^2$$

where $R$ is the radius of the sphere. The radius is often taken to be unity, in which case the area is simply the spherical excess. Recalling the definition of a solid angle, we conclude that the spherical excess is also the solid angle subtended by the spherical triangle at the center of the sphere. An important result is the spherical excess of a right-angled spherical triangle, which is given by

$$\tag{1.1.12} \tan \frac{1}{2} E = \tan \frac{a}{2} \tan \frac{b}{2}$$

## Geometry of the Earth

The shape of the Earth is termed a geoid and is roughly an oblate spheroid, meaning it is slightly flattened at the poles and bulging at the equator. The radius of the Earth varies depending on where it is measured, with the equatorial radius being about 6,378 km and the polar radius being about 6,357 km. For most of our calculations, however, the Earth can be treated as a perfect sphere with a mean radius of approximately 6,371 km.

A point on the surface of the Earth can be uniquely specified by its latitude and longitude. Latitude is the angle between the equatorial plane and a line drawn from the center of the Earth to the point, while longitude is the angle between the prime meridian (defined as the great circle passing through the north and south poles, and the Royal Observatory in Greenwich, England) and a great circle passing through the point and the poles. To indicate the height or depth above or below the mean sea level, a third coordinate—the altitude—must be introduced.

Latitude is measured in degrees, with the equator at $0^\circ$, the north pole at $90^\circ$ north, and the south pole at $90^\circ$ south. Sometimes the directions are dropped, and negative values are used to indicate southern latitudes, i.e., $-90^\circ$ latitude is the south pole.

Longitude is also measured in degrees, with the prime meridian at $0^\circ$, and increasing westwards up to $360^\circ$. They are usually expressed in the range $0^\circ$ to $180^\circ$ E and $0^\circ$ to $180^\circ$ W, or alternatively as negative values for eastern longitudes, i.e., $-90^\circ$ or $270^\circ$ longitude is the same as $90^\circ$ E.

{{< svg "pos/latlon.svg" "Latitude and Longitude" "Latitude of A is the angle AA', whereas the longitude difference between A and B is the angle APB or A'B'" >}}

The co-latitude is defined as the complement of the latitude, i.e.,

$$\text{co-latitude} = 90^\circ - \text{latitude}$$

{{< callout type="remark" >}}
Due to the non-spherical shape of the Earth, there are multiple definitions of latitude, as follows:

- Geodetic Latitude: The angle between the equatorial plane and the normal to the surface of the ellipsoid at the point.
- Geocentric Latitude: The angle between the equatorial plane and a line drawn from the center of the Earth to the point.
- Astronomical Latitude: The angle between the equatorial plane and the vertical direction at the point, as determined by a plumb line.

Usually, unless explicitly stated, the term latitude refers to geodetic latitude. The difference between geodetic and geocentric latitude is small, but can be significant for precise measurements. The astronomical latitude depends on the local gravitational field as well as the speed of rotation of the Earth at that point.

The flattening, or ellipticity, of the Earth is defined as

$$\tag{1.1.13} f = \frac{a - b}{a}$$

where $a$ is the equatorial radius and $b$ is the polar radius. The flattening of the Earth is approximately $1/298.257$.

The geodetic latitude $\phi$ and the geocentric latitude $\theta$ are related to each other by the ellipticity $f$ as follows:

$$\tag{1.1.14} \tan \phi = (1 - f)^2 \, \tan \theta$$
{{< /callout >}}

Two locations having the same latitude are said to be on the same parallel of latitude, while two locations having the same longitude are said to be on the same meridian. The distance between two points on the same parallel of latitude is called their departure, given by

$$p = R \Delta \lambda \, \cos \phi$$

where $R$ is the radius of the Earth, $\phi$ is the latitude, and $\Delta \lambda$ is the difference in longitude between the two points. Note that the departure is not the shortest distance between the two points, as it is measured along the parallel of latitude, which is a small circle.

{{< svg "pos/departure.svg" "Departure between two points" "Distance along the small circle parallel to the equator is the departure between AB, distance along the great circle is the shortest distance between AB" >}}

The distance between two points on the same meridian is given by

$$p = R \Delta \phi$$

where $\Delta \phi$ is the difference in latitude between the two points.

A nautical mile is the great circle distance subtending an angle of one minute of arc at the center of the Earth. A knot is a speed of one nautical mile per hour.

The bearing angle is defined as the angle between the north direction and the direction from one point to another, measured clockwise from north. If the bearing angle is measured from the south direction, it is called the back bearing angle.

## The Celestial Sphere

The celestial sphere is an imaginary sphere of infinite radius, concentric with the Earth, on which all celestial objects appear to be projected. The Earth is at the center and the celestial objects are at the surface of the sphere. This is a useful tool as it allows us to represent the positions of celestial objects on a two-dimensional surface, without considering their distances from the observer.

For an observer, the point on the celestial sphere directly overhead is called the zenith, while the point directly below is called the nadir. The line connecting the zenith and nadir is called the zenith-nadir line. The horizon is the great circle on the celestial sphere that is perpendicular to the zenith-nadir line. This is the boundary where the sky appears to meet the Earth, and it defines the limits of the observer's view of the celestial sphere. The points where the celestial equator intersects the horizon are defined as the east and west cardinal points.

The celestial meridian or local meridian of an observer is a great circle on the celestial sphere that passes through the zenith, nadir, and the north and south celestial poles. The points where the celestial equator intersects the meridian are defined as the north and south cardinal points. The prime vertical is defined as the great circle passing through the zenith, nadir, and the east and west cardinal points.

The celestial sphere and all the objects on it (stars, galaxies, etc.) appear to rotate westwards around the Earth once nearly every 24 hours. This apparent motion is due to the rotation of the Earth on its axis. However, to the observer it makes no difference whether it is the Earth that is rotating on its axis, or if the celestial sphere is rotating around the Earth. The point about which the celestial sphere appears to rotate is called the celestial pole. This is the projection of Earth's axis of rotation onto the celestial sphere. The two celestial poles are the north celestial pole (NCP) and the south celestial pole (SCP).

The north celestial pole is the point about which the sky seems to rotate clockwise. It is easily recognizable in the sky as it is very close to the bright star Polaris, which because of this is also known as the north star or pole star. The south celestial pole is located in the southern hemisphere opposite to the north celestial pole. It does not have a bright star associated with it; however, one can approximately locate it by finding $\sigma$ Octantis (IAU name Polaris Australis), a faint star in the constellation Octans.

The celestial equator is the projection of the Earth's equator onto the celestial sphere. It divides the celestial sphere into the northern and southern hemispheres. The poles of the celestial equator are the north and south celestial poles.

The Sun, when projected onto the celestial sphere, appears to move along a great circle in the course of a year. This great circle on which the Sun moves is called the ecliptic. The ecliptic is tilted at an angle of approximately $23.5^\circ$ to the celestial equator, which is due to the tilt of the Earth's axis of rotation relative to its orbit around the Sun. The Sun's motion along the ecliptic is slow, much slower than the rotation of the celestial sphere, and thus the Sun can approximately be considered as a fixed point on the celestial sphere for short periods of time.

The poles of the ecliptic are the two points on the celestial sphere which are at $90^\circ$ from the ecliptic. The north ecliptic pole is located in the constellation Draco, while the south ecliptic pole is located in the constellation Dorado.

{{< svg "pos/celsph.svg" "Celestial Sphere" "Celestial Sphere" >}}

In the above diagram, the north celestial pole is denoted by $P$, and the south celestial pole by $Q$. The north and south ecliptic poles are denoted by $K$ and $K'$, respectively. The zenith is denoted by $Z$, the nadir by $Z'$. The cardinal points are the east point $E$, and the west point $W$, the north point $N$ and the south point $S$.

The horizon is the great circle defined by the cardinal points $NWSEN$. The celestial equator is the other great circle passing through the east and west points. The meridian is the great circle passing through the zenith, nadir, north celestial pole, and south celestial pole, defined by $ZPNZ'QSZ$ (This has not been labelled in the figure to avoid cluttering). The ecliptic is the great circle perpendicular to the north and south ecliptic poles, containing the Sun. Additionally, the great circle $ZEZ'W$ is called the prime vertical.

## Problems

{{< tabs >}}
    {{< tab name="P1" >}}

    Solve completely for the spherical triangle $ABC$, given <br>
    $$
    \begin{align*}
    &i)\,   &A = 60.0^\circ,\quad &B = 70.0^\circ,\, &c = 80.0^\circ \\
    &ii)\,  &a = 50.0^\circ,\quad &b = 60.0^\circ,\, &c = 70.0^\circ \\
    &iii)\, &a = 40.0^\circ,\quad &b = 50.0^\circ,\, &C = 60.0^\circ \\
    &iv)\,  &A = 120.0^\circ,\quad &B = 45.0^\circ,\, &C = 60.0^\circ \\
    &v)\,   &A = 110.0^\circ,\quad &B = 60.0^\circ,\, &a = 60.0^\circ \\
    &vi)\,  &a = 60.0^\circ,\quad &b = 70.0^\circ,\, &A = 50.0^\circ \\
    \end{align*}
    $$

    {{< /tab >}}

    {{< tab name="Solution" >}}
    
    The solutions are as follows:
    $$
    \begin{align*}
    &i)\,   &a = 58.6^\circ,\quad &b = 66.3^\circ,\, &C = 91.7^\circ \\
    &ii)\,  &A = 54.6^\circ,\quad &B = 67.1^\circ,\, &C = 88.2^\circ \\
    &iii)\, &A = 55.7^\circ,\quad &B = 79.8^\circ,\, &c = 42.4^\circ \\
    &iv)\,  &a = 103.8^\circ,\quad &b = 52.4^\circ,\, &c = 76.2^\circ \\
    &v)\,   &b = 52.9^\circ,\quad &c = 16.5^\circ,\, &C = 18.0^\circ \\
    &vi)\,  &B = 56.2^\circ,\quad &c=104.4^\circ,\, &C = 121.0^\circ \\
    \end{align*}
    $$

    {{< /tab >}}
{{< /tabs >}}

{{< tabs >}}
    {{< tab name="P2" >}}

    Find the distance along the great circle between two points on the Earth, having coordinates $(\phi_1, \lambda_1)$ and $(\phi_2, \lambda_2)$.

    {{< /tab >}}

    {{< tab name="Solution" >}}

    Joining the two points to the north pole, we get a spherical triangle with two sides equal to $90^\circ - \phi_1$ and $90^\circ - \phi_2$, and the included angle equal to $\Delta \lambda = |\lambda_2 - \lambda_1|$. Using the law of cosines, the great circle distance $D = d\, R$ is given by

    $$\cos d = \cos(90^\circ - \phi_1) \cos(90^\circ - \phi_2) + \sin(90^\circ - \phi_1) \sin(90^\circ - \phi_2) \cos \Delta \lambda$$
    $$\implies \cos d = \sin \phi_1 \sin \phi_2 + \cos \phi_1 \cos \phi_2 \cos \Delta \lambda$$
    $$\tag{1.1.15} \therefore \boxed{D = R \cos^{-1} \left[ \sin \phi_1 \sin \phi_2 + \cos \phi_1 \cos \phi_2 \cos \Delta \lambda \right]}$$

    where $R$ is the radius of the Earth. This is a very important result and is often used.

    {{< /tab >}}
{{< /tabs >}}

{{< tabs >}}
    {{< tab name="P3" >}}

    Find the difference between the departure and the great circle distance between two points on the Earth, having the same latitude $\phi$ and longitude difference $\Delta \lambda$. Find the result in the limit of small $\Delta \lambda$.

    {{< /tab >}}

    {{< tab name="Solution" >}}
    
    As shown in the previous problem, the great circle distance $D = d\,R$ is given by

    $$\cos d = \sin \phi_1 \sin \phi_2 + \cos \phi_1 \cos \phi_2 \cos \Delta \lambda$$

    Since $\phi_1 = \phi_2 = \phi$, we get

    $$\cos d = \sin^2 \phi + \cos^2 \phi \cos \Delta \lambda$$
    $$\implies \cos d = 1 - \cos^2 \phi (1 - \cos \Delta \lambda)$$

    Using the Taylor series expansion for cosine, we get

    $$\cos d = 1 - \cos^2 \phi \left( 1 - \left[ 1 - \frac{(\Delta \lambda)^2}{2} + \frac{(\Delta \lambda)^4}{24} - \ldots \right] \right)$$
    $$\implies \cos d = 1 - \frac{\cos^2 \phi}{2} (\Delta \lambda)^2 + \frac{\cos^2 \phi}{24} (\Delta \lambda)^4 - \ldots$$

    Using the Taylor series expansion for arccosine, we get
    $$d = \cos \phi \Delta \lambda - \frac{1}{24} \cos \phi \sin^2 \phi (\Delta \lambda)^3 + \ldots$$

    Thus, the difference between the departure and the great circle distance is

    $$\boxed{p - D = \frac{R}{24} \cos \phi \sin^2 \phi (\Delta \lambda)^3 + \ldots}$$

    The difference in the two paths is only about 5 km for $\Delta \lambda < 20^\circ$!

    {{< /tab >}}
{{< /tabs >}}

{{< tabs >}}
    {{< tab name="P4" >}}

    A ship is travelling at 20 knots from Vizhinjam International Seaport ($8^\circ 22'$ N, $76^\circ 57'$ E) to Port of Colombo ($6^\circ 57'$ N, $79^\circ 51'$ E). Find the time taken to reach Colombo, assuming the ship travels along the great circle. Also, find the bearing angle at the start of the journey.

    {{< /tab >}}

    {{< tab name="Solution" >}}

    The distance between the two ports along a great circle is given by

    $$\cos d = \sin \phi_1 \sin \phi_2 + \cos \phi_1 \cos \phi_2 \cos \Delta \lambda$$

    From this, we get $d = 3^\circ 12' = 192'$. Thus, the distance is 192 nautical miles. At a speed of 20 knots, the time taken to reach Colombo is

    $$\boxed{t = \frac{192}{20}\,\mathrm{hours} = 9^h 36^m}$$

    The bearing angle $B$ at the start of the journey can be found using the sine rule:

    $$ \frac{\sin \Delta \lambda}{\sin d} = \frac{\sin B}{\sin (90^\circ - \phi_2)}$$

    Thus, we get $\boxed{B = 115^\circ 53'}$

    {{< /tab >}}
{{< /tabs >}}
