---
title: Sun, Moon and Planets
weight: 5
---

## The Sun

As seen from Earth, the Sun appears to go around the Earth in a period of one year, following a path called the ecliptic. The ecliptic is the plane of the Earth's orbit around the Sun, and it is tilted with respect to the celestial equator by about $23.5^\circ$. The Sun's apparent motion along the ecliptic is not uniform, as it moves faster when it is closer to the Earth (at perihelion) and slower when it is farther away (at aphelion).

### Sunrise and Sunset

We are often asked to find the time and duration of sunrise and sunset for a given location and date. The time of sunrise is the moment when the upper limb of the Sun appears above the horizon, while the time of sunset is the moment when the upper limb of the Sun disappears below the horizon. The duration of sunrise or sunset is the time interval between the top and bottom limbs of the Sun crossing the horizon.

Suppose an object $X$ has the equatorial coordinates $(\alpha, \delta)$ and the observer's latitude is $\phi$. The hour angle $h$ of the object at the time of rising or setting (see P2 chapter 1.2) is given by

$$\tag{1.5.1} \boxed{\cos h = -\tan \phi \tan \delta}$$

This gives two solutions for the hour angle $h$ in the interval $[-12^h, 12^h]$. The solution lying in the interval $[-12^h, 0]$ corresponds to the time of rising, while the solution lying in the interval $[0, 12^h]$ corresponds to the time of setting.

The azimuth $A$ of the object at the time of rising or setting (see P3 chapter 1.2) is given by

$$\tag{1.5.2} \cos A = \sin \delta \sec \phi$$

where the solution for azimuth lying in the range $[0, 180^\circ]$ corresponds to the time of rising, while the solution lying in the range $[180^\circ, 360^\circ]$ corresponds to the time of setting.

This simple treatment, however, does not give accurate results for the Sun, due to the effects of atmospheric refraction and the finite size of the solar disk. The Sun is not a point source, and its upper limb appears above the horizon when it is still below the horizon due to atmospheric refraction. The time of sunrise and sunset can be calculated more accurately by taking these effects into account.

{{< callout type="remark" >}}
Even after sunset, some sunlight is received by the observer by scattering off the atmosphere. This phenomenon is called twilight. There are three types of twilight: civil, nautical, and astronomical.

- Civil twilight: The time when the Sun is between $0^\circ$ and $6^\circ$ below the horizon. During this time, there is enough light for most outdoor activities without additional lighting.
- Nautical twilight: The time when the Sun is between $6^\circ$ and $12^\circ$ below the horizon. During this time, the horizon is still visible at sea, allowing sailors to take navigational measurements.
- Astronomical twilight: The time when the Sun is between $12^\circ$ and $18^\circ$ below the horizon. During this time, the sky is dark enough for astronomical observations, as the Sun's light does not interfere with the visibility of stars and other celestial objects.
{{< /callout >}}

### Tilted Plane of the Ecliptic

Due to the axial tilt of the Earth, the Sun's declination $\delta$ varies throughout the year. The Sun reaches its maximum declination of $23.5^\circ$ at the summer solstice (around June 21) and its minimum declination of $-23.5^\circ$ at the winter solstice (around December 21). The equinoxes occur when the Sun's declination is $0^\circ$, around March 21 (vernal equinox) and September 23 (autumnal equinox).

The amount of heat received from the Sun and the daily average temperature of a place is largely independent of the distance from the Sun, but proportional to the inclination of the Sun's rays hitting the surface of the Earth. The more direct the rays, the more energy is received per unit area. This is why the equator is hotter than the poles, as the Sun's rays are more direct at the equator.

$$E \propto \cos (\phi - \delta)$$

where $E$ is the amount of energy received per unit area, $\phi$ is the observer's latitude, and $\delta$ is the Sun's declination.

This is also what causes seasons, as the tilt of the Earth's axis causes different parts of the Earth to receive varying amounts of sunlight throughout the year, as discussed next.

If the observer's latitude is numerically less than $23.5^\circ$, there will be two occasions each year when the Sun is directly overhead the observer ($\phi = \delta$). If the observer's latitude is numerically greater than $23.5^\circ$, the Sun will never be directly overhead the observer. If the observer's latitude is numerically equal to $23.5^\circ$, the Sun will be directly overhead at the Tropic of Cancer (north) and the Tropic of Capricorn (south) only once a year, at the summer and winter solstices respectively.

If the latitude of the observer is numerically greater than $66.5^\circ$, the Sun will remain below the horizon for at least one full day (24 hours) during some part of the year and above the horizon for at least one full day during some other part of the year. The phenomenon when the Sun doesn't set even at midnight is known as the midnight sun, and when it does not rise is called the polar night. The small circle at latitude $66.5^\circ$ is called the Arctic Circle in the northern hemisphere and the Antarctic Circle in the southern hemisphere.

At the poles, the Sun remains above the horizon for six months during summer and below the horizon for six months during winter.

### Seasons

We experience seasons on Earth due to the axial tilt of the Earth and its orbit around the Sun. The tilt causes different parts of the Earth to receive varying amounts of sunlight throughout the year, leading to changes in temperature and daylight hours. The hemisphere tilted towards the Sun experiences summer, while the hemisphere tilted away from the Sun experiences winter.

When the Sun moves from the vernal equinox to the summer solstice, the northern hemisphere experiences the spring season, with increasing daylight and warmer temperatures. The southern hemisphere experiences autumn during this time, with decreasing daylight and cooler temperatures.

From the summer solstice to the autumnal equinox, the northern hemisphere experiences summer, with the longest days and highest temperatures. The southern hemisphere experiences winter during this time, with the shortest days and lowest temperatures. The length of daylight is longest at the summer solstice and shortest at the winter solstice.

From the autumnal equinox to the winter solstice, the northern hemisphere experiences autumn, with decreasing daylight and cooler temperatures. Finally, from the winter solstice to the vernal equinox, the northern hemisphere experiences winter, with the shortest days and lowest temperatures. The southern hemisphere experiences the seasons in reverse order, with summer occurring when the northern hemisphere is experiencing winter, and vice versa.

The length of a season can be defined as the time interval between two successive solstices or equinoxes. This can be calculated by finding the time taken for the Sun to move between these points in its orbit around the Earth. It is usually around three months, but can vary slightly due to the elliptical shape of the Earth's orbit.

The Sun is near the vernal equinox around March 21, at the summer solstice around June 21, at the autumnal equinox around September 21, and at the winter solstice around December 21. However, the exact dates can vary slightly each year due to the elliptical shape of the Earth's orbit and the leap year system.

## Geocentric Path of the Planets

All planets, like Earth, orbit the Sun in elliptical orbits. To describe the position of a planet with respect to the Earth and the Sun, we often make use of two angles—the elongation $\eta$ and the phase angle $\phi$ of the planet.

The planets can be classified as either interior or exterior planets based on their position relative to Earth's orbit. An exterior planet is one that orbits the Sun outside of Earth's orbit, while an interior planet is one that orbits the Sun inside of Earth's orbit.

### Elongation

A planet is said to be in conjunction with the Sun when it is collinear with the Earth and the Sun and is on the same side as the Sun when viewed from Earth.

It is said to be in opposition when it is on the opposite side of the Sun. When a planet is in opposition, it is at its closest point to Earth and appears fully illuminated.

Only an exterior planet can be in opposition to the Sun, while an interior planet can only be in conjunction with the Sun.

For interior planets, there are two types of configurations: inferior conjunction and superior conjunction. In inferior conjunction, the planet is between the Earth and the Sun, while in superior conjunction, the planet is on the opposite side of the Sun from Earth.

The elongation $\eta$ of a planet is defined as the angular distance between it and the Sun as seen from Earth. An elongation of $0^\circ$ corresponds to conjunction and $180^\circ$ corresponds to opposition.

{{< callout type="remark" >}}
For inferior planets (Mercury and Venus), the maximum elongation is the greatest angular separation they can achieve from the Sun as seen from Earth. For Mercury, it is about $28^\circ$, while for Venus it is about $47^\circ$. These planets can never achieve an elongation greater than this, and thus are only seen just before sunrise or just after sunset. Exterior planets can have any elongation from $0^\circ$ to $180^\circ$.
{{< /callout >}}

### Phase Angle and Phase

The phase angle $\phi$ of a planet is the angle subtended by the Sun and the Earth as seen from the planet. It helps in quantifying how much of the planet's illuminated side is visible from Earth.

Interior planets can have any phase angle from $0^\circ$ (new) to $180^\circ$ (full), while exterior planets can have phase angles from $0^\circ$ to some maximum value less than $90^\circ$, which it attains at quadrature.

Quadrature is the configuration when an exterior planet is at a right angle to the line connecting the Earth and the Sun. The planet can either be in eastern quadrature (east of the Sun) or western quadrature (west of the Sun).

The phase $q$ of a planet is defined as the fraction of the planet's illuminated side that is visible from Earth. It can be calculated using the formula:

$$\tag{1.5.3} q = \frac{1 + \cos(\phi)}{2}$$

where $\phi$ is the phase angle. The phase can vary from 0 (new—the planet appears completely dark) to 1 (full—the planet appears fully illuminated) for interior planets, and from some minimum value greater than 0.5 to 1 for exterior planets. Thus, exterior planets are always seen in gibbous or full phase.

For interior planets, a phase of 0 corresponds to inferior conjunction, a phase of 0.5 corresponds to greatest elongation, and a phase of 1 corresponds to superior conjunction.

{{< callout type="image" >}}
{{< svg "pos/planetconfig.svg" "Planetary Configurations" "Planetary Configurations (Source: Wikipedia)" >}}
{{< /callout >}}

### Retrograde Motion

Retrograde motion is the apparent backward motion of a planet as observed from Earth. This occurs when the Earth overtakes a planet in its orbit, causing the planet to appear to move in the opposite direction against the background stars.

The period of retrograde motion varies for each planet and can last for a few weeks to months. The retrograde motion of a planet can be predicted based on its orbital period and the relative positions of the Earth and the planet.

Retrograde motion for exterior planets occurs when the planet is near the opposition point in its orbit, with the opposition occurring in the middle of the retrograde loop. The points when the apparent motion of the planet changes from direct to retrograde and vice versa are called stationary points.

{{< callout type="image" >}}
{{< gif "pos/retrograde.gif" "Retrograde Motion of Planets" "The retrograde motion of planets occurs when Earth overtakes them in their orbits. (Source: Wikipedia)" >}}
{{< /callout >}}

### Synodic Period

The synodic period of a planet is the time interval between its two successive conjunctions or oppositions. It is different from the sidereal period, which is the time it takes for a planet to complete one orbit around the Sun with respect to the stars.

Let the sidereal period of the planet be $T_p$ and the sidereal period of the Earth be $T_e$. If the planet orbits the Sun in the same direction as the Earth (anticlockwise), its synodic period $T_s$ is given by

$$\tag{1.5.4} \boxed{\frac{1}{T_s} = \left\lvert \frac{1}{T_p} - \frac{1}{T_e} \right\rvert}$$

If the planet orbits the Sun in the opposite direction to that of Earth (clockwise), its synodic period is

$$\tag{1.5.5} \frac{1}{T_s} = \frac{1}{T_p} + \frac{1}{T_e}$$

The mean solar day is just the synodic period of Earth's rotation and its revolution around the Sun.

## Moon

The Moon is Earth's only natural satellite. It orbits the Earth in an elliptical orbit, with a semi-major axis of about 384,400 km, an eccentricity of 0.055, and an orbital tilt of about 5.1$^\circ$ with respect to the ecliptic plane. The angular diameter of the Moon as seen from Earth varies from about 29.4' to 33.5', with an average of about 31'.

The rotation period of the Moon is equal to its sidereal period, about 27.3 days. Due to this, the same side of the Moon always faces the Earth, a phenomenon known as synchronous rotation or tidal locking. The far side of the Moon is never visible from Earth.

The lunar nodes are the points where the Moon's orbit intersects the ecliptic plane. These nodes precess with a period of about 18.6 years, due to the gravitational influence of the Sun and the Earth. This is also the reason for the nutation of Earth's axis.

### Phases of the Moon

The Moon goes through a cycle of phases as it orbits the Earth. The phases are determined by the relative positions of the Sun, Earth, and Moon. The main phases of the Moon are:

- **New Moon**: The Moon is between the Earth and the Sun, and its illuminated side is facing away from the Earth. Thus, it is not visible from Earth, having a phase of 0.
- **Waxing Crescent**: A small sliver of the Moon's illuminated side is visible on the west side of the Moon. It increases in visibility until it reaches the First Quarter phase. It has a phase between 0 and 0.5. The most notable feature visible is Mare Crisium.
- **First Quarter**: The whole of the west half of the Moon appears illuminated. It has a phase of 0.5. A few of the features visible now are Mare Imbrium, Mare Serenitatis, and Mare Tranquillitatis.
- **Waxing Gibbous**: More than half of the Moon's illuminated side is visible, increasing until it reaches the Full Moon phase.
- **Full Moon**: The entire illuminated side of the Moon is visible, with the Earth between the Sun and the Moon. It has a phase of 1.0.
- **Waning Gibbous**: More than half of the Moon's illuminated side is visible; however, it is decreasing to the Third Quarter phase. The western part of the Moon is dark now, with Mare Crisium no longer visible.
- **Third Quarter**: The whole of the east half of the Moon is illuminated. It has a phase of 0.5. The most prominent features visible now are the Copernicus crater and the Aristarchus crater.
- **Waning Crescent**: A small sliver of the Moon's illuminated side is again visible, this time on the east side, decreasing until it reaches the New Moon phase again.

{{< callout type="image" >}}
{{< png "pos/moonphases.png" "Phases of the Moon" "The different phases of the Moon as it orbits the Earth." >}}
{{< /callout >}}

From new moon to new moon, the Moon takes about 29.5 days, which is known as a synodic month. The synodic month is longer than the sidereal month (27.3 days) due to the Earth's motion around the Sun.

A Metonic cycle is a period of 19 years after which the phases of the Moon repeat on the same days of the year. This is because 19 years are almost equal to 235 lunar months, which is why the lunar calendar is often based on a Metonic cycle.

### Libration

Even though the Moon is tidally locked, we can see a bit more than half of its surface from Earth due to a phenomenon called libration. Libration allows us to see about 59% of the Moon's surface over time. It occurs due to the tilt of the Moon's orbit, the tilt of the Moon's axis, and the elliptical shape of its orbit.

**Libration in longitude**: This is caused by the elliptical shape of the Moon's orbit. As the Moon moves closer to and farther from the Earth, its angular speed changes, causing it to appear to wobble slightly in longitude. The rotation seems to lag or lead its orbital position. The amplitude of this libration is about 7.8 degrees.

**Libration in latitude**: This is caused by the tilt of the Moon's axis—the tilt between its rotation axis and orbital axis. As the Moon orbits the Earth, we can see slightly more of its northern or southern hemisphere at different times. The amplitude of this libration is about 6.5 degrees.

**Diurnal libration**: This is caused by the observer's position on the Earth's surface. As the Earth rotates, the observer's position changes, allowing them to see slightly more of the Moon's surface at different times of the day. The amplitude of this libration is about 1 degree.

{{< callout type="image" >}}
{{< gif "pos/libration.gif" "Libration of the Moon" "The libration of the Moon allows us to see slightly more than half of its surface. (Source: Wikipedia)" >}}
{{< /callout >}}

### Eclipses

#### Lunar Eclipse

A lunar eclipse occurs when the Earth passes between the Sun and the Moon, causing the Earth's shadow to fall on the Moon. The shadow of the Earth has three parts: the umbra (the darkest part), the penumbra (the lighter part), and the antumbra (the region where the shadow is not completely dark).

{{< callout type="image" >}}
{{< svg "pos/lunareclipse.svg" "Lunar Eclipse" "Geometry of a Lunar Eclipse (source: Wikipedia)" >}}
{{< /callout >}}

Lunar eclipses can be classified into several types:

- A total lunar eclipse occurs when the Moon passes through the Earth's umbra, while a partial lunar eclipse occurs when only part of the Moon passes through the umbra. When the Moon is inside the umbral region, it appears blood red, due to the scattering of sunlight through the Earth's atmosphere. This is often referred to as a "blood moon." If you were lucky enough, you might have seen the blood moon during the total lunar eclipse of September 7, 2025.

{{< callout type="image" >}}
{{< png "pos/792025.png" "7 September 2025 Lunar Eclipse" "Total Lunar Eclipse of 7 September 2025. Photo captured by the Sri Lankan team of IOAA 2025" >}}
{{< /callout >}}

- A penumbral lunar eclipse occurs when the Moon passes through the Earth's penumbra, causing a subtle shading on the Moon's surface.
- A partial lunar eclipse occurs when only a portion of the Moon passes through the Earth's umbra.
- A central lunar eclipse is a type of total lunar eclipse where the Moon is in the center of the Earth's shadow.
- A Selenelion (also called horizontal eclipse) occurs when both the Sun and the eclipsed Moon can be seen at the same time, usually during sunrise or sunset. A selenelion occurs during every total lunar eclipse—it is an experience of the observer, not a planetary event separate from the lunar eclipse itself. Although during selenelion the Moon is completely within the Earth's umbra, both it and the Sun can be observed in the sky because atmospheric refraction causes each body to appear higher (i.e., more central) in the sky than its true geometric planetary position.

#### Solar Eclipse

A solar eclipse occurs when the Moon passes between the Sun and the Earth, causing the Moon's shadow to fall on the Earth.

{{< callout type="remark" >}}
Eclipse, occultation, and transit—all these terms represent one object covering or passing in front of another object, but there is a slight difference between them.

An eclipse is an event in which a body passes through the shadow of another body. An occultation takes place when an occulting body passes in front of another body, blocking its light. A transit is an event when an inferior planet moves across the solar disk, appearing as a small dot moving across the Sun's face.

Thus, a lunar eclipse is an eclipse (since the Moon passes through Earth's shadow). However, a solar eclipse is an occultation (since here, the Moon occults the Sun).
{{< /callout >}}

{{< callout type="image" >}}
{{< svg "pos/solareclipse.svg" "Solar Eclipse" "Geometry of a Solar Eclipse (source: Wikipedia)" >}}
{{< /callout >}}

Just like lunar eclipses, solar eclipses too can be classified into several types:

- A total solar eclipse occurs when the Moon completely covers the Sun.
- A partial solar eclipse occurs when only part of the Sun is covered by the Moon.
- An annular solar eclipse occurs when the Moon is too far from the Earth to completely cover the Sun, leaving a ring of sunlight visible around the edges of the Moon.
- A hybrid eclipse is a rare type of solar eclipse that shifts between a total and an annular eclipse along different sections of its path.
- A central eclipse is an eclipse during which the central line of the umbra touches Earth's surface.

A solar eclipse can only occur during a new moon, while a lunar eclipse can only occur during a full moon. However, not every new moon results in a solar eclipse, and not every full moon results in a lunar eclipse. This is because the Moon's orbit is tilted with respect to the Earth's orbit around the Sun, so the three bodies do not always align perfectly. Thus, for an eclipse to occur, the Moon must be near one of its nodes (the points where its orbit intersects the ecliptic plane) during a new or full moon.

The longest possible duration of a total solar eclipse is about $7^m 30^s$, while the longest possible duration of a total lunar eclipse is about $1^h 40^m$. The frequency of eclipses varies, with at least two solar and two lunar eclipses occurring each year. The reason for the occurrence of lunar eclipses being much more frequent than that of solar eclipses is because the Earth's shadow is much larger than the Moon's shadow, giving the Moon more chances to pass through it.

A Saros cycle is a period of about 18 years, 11 days, and 8 hours after which the geometry of the Sun, Earth, and Moon repeats, leading to similar eclipses. This cycle is used to predict future eclipses.

### Months

A month is a period of time based on the motion of the Moon around the Earth. There are several types of months:

- **Sidereal month**: The time it takes for the Moon to complete one orbit around the Earth with respect to the stars, about 27.3217 days.
- **Synodic month**: The time it takes for the Moon to complete one cycle of phases, from new moon to new moon, about 29.5306 days.
- **Tropical month**: The time it takes for the Moon to return to the same position relative to the Sun, about 27.3216 days.
- **Anomalistic month**: The time it takes for the Moon to return to the same point in its elliptical orbit, about 27.5545 days.
- **Draconic month**: The time it takes for the Moon to return to the same node of its orbit, about 27.2122 days.
