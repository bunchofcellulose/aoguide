---
title: Sun, Moon and Planets
weight: 5
---

## Geocentric Path of the Sun

The sun appears to go around the Earth in a period of one year, following a path called the ecliptic. The ecliptic is the plane of the Earth's orbit around the Sun, and it is tilted with respect to the celestial equator by about $23.5^\circ$. The sun's apparent motion along the ecliptic is not uniform, as it moves faster when it is closer to the Earth (at perihelion) and slower when it is farther away (at aphelion).

### Sunrise and Sunset

We are often asked to find the time of sunrise and sunset for a given location and date. The time of sunrise is the moment when the upper limb of the Sun appears above the horizon, while the time of sunset is the moment when the upper limb of the Sun disappears below the horizon.

Say an object $X$ has the equatorial coordinates $(\alpha, \delta)$ and the observer's latitude is $\phi$. The hour angle $h$ of the object at the time of rising or setting (see P2 chapter 1.2) is given by

$$\tag{1.5.1} \boxed{\cos h = -\tan \phi \tan \delta}$$

This gives two solutions for the hour angle $h$ in the interval $[-12^h, 12^h]$. The solution lying in the interval $[-12^h, 0]$ corresponds to the time of rising, while the solution lying in the interval $[0, 12^h]$ corresponds to the time of setting.

The azimuth $A$ of the object at the time of rising or setting (see P3 chapter 1.2) is given by

$$\tag{1.5.2} \cos A = \sin \delta \sec \phi$$

where the solution of azimuth lying in the range $[0, 180^\circ]$ corresponds to the time of rising, while the solution lying in the range $[180^\circ, 360^\circ]$ corresponds to the time of setting.

This simple treatment however, does not give accurate results for the Sun, due to the effects of atmospheric refraction and the finite size of the solar disk. The Sun is not a point source, and its upper limb appears above the horizon when it is still below the horizon due to atmospheric refraction. The time of sunrise and sunset can be calculated more accurately by taking into account these effects.

Even after sunset, some sunlight is recieved by the observer by scattering off of the atmoshpere. This phenomena is called twilight. Civil twilight is defined as the time when the Sun is between $6^\circ$ below the horizon and the horizon, nautical twilight is defined as the time when the Sun is between $12^\circ$ below the horizon and $6^\circ$ below the horizon, and astronomical twilight is defined as the time when the Sun is between $18^\circ$ below the horizon and $12^\circ$ below the horizon. The times of these twilights can be calculated using similar formulas as above, with appropriate values for $\delta$.

### Tilted plane of the ecliptic

Due to the axial tilt of the Earth, the Sun's decliniation $\delta$ varies throughout the year, causing the seasons. The Sun reaches its maximum declination of $23.5^\circ$ at the summer solstice (around June 21) and its minimum declination of $-23.5^\circ$ at the winter solstice (around December 21). The equinoxes occur when the Sun's declination is $0^\circ$, around March 21 (vernal equinox) and September 23 (autumnal equinox).

If the observer's latitude is numerically less than $23.5^\circ$, there will be two occasions each year when the Sun is directly overhead the observer ($\phi = \delta$). If the observer's latitude is numerically greater than $23.5^\circ$, there will be no occasions when the Sun is directly overhead the observer. If the observer's latitude is numerically equal to $23.5^\circ$, the Sun will be directly overhead at the tropic of Cancer (north) and the tropic of Capricorn (south) only once, at the summer and winter solstices respectively.

If the latitude of the observer is numerically greater than $66.5^\circ$, the Sun will remain below the horizon for at least one full day during some part of the year and above horizon for at least one full day during some other part of the year. The phenomena when the Sun doesn't set even at midnight is known as the midnight sun, and when it does not rise is called the polar night. The small circle at latitude $66.5^\circ$ is called the Arctic Circle in the northern hemisphere and the Antarctic Circle in the southern hemisphere.

At the poles, the Sun remains above the horizon for six months during summer and below the horizon for six months during winter.

The amount of hear recieved from the sun and the daily average temperature of a place is highly independent of the distance from the Sun. Amounth of energy arriving per unit area is propotional to the inclinaition of the Sun's rays hitting the surface of the Earth. The more direct the rays, the more energy is received per unit area. This is why the equator is hotter than the poles, as the Sun's rays are more direct at the equator.

$$E \propto \cos (\phi - \delta)$$

where $E$ is the amount of energy received per unit area, $\phi$ is the observer's latitude, and $\delta$ is the Sun's declination.

### Seasons

We experience seasons on Earth due to the axial tilt of the Earth and its orbit around the Sun. The tilt causes different parts of the Earth to receive varying amounts of sunlight throughout the year, leading to changes in temperature and daylight hours.

When the sun moves from the vernal equinox to the summer solstice, the northern hemisphere experiences the spring season, with increasing daylight and warmer temperatures. From the summer solstice to the autumnal equinox, the northern hemisphere experiences summer, with the longest days and highest temperatures. From the autumnal equinox to the winter solstice, the northern hemisphere experiences autumn, with decreasing daylight and cooler temperatures. Finally, from the winter solstice to the vernal equinox, the northern hemisphere experiences winter, with the shortest days and lowest temperatures.

The southern hemisphere experiences the seasons in reverse order, with summer occurring when the northern hemisphere is experiencing winter, and vice versa.

The length of the season is the time it takes for the Sun to move from one solstice or equinox to the next. The length of each season is approximately three months, but it can vary slightly due to the elliptical shape of the Earth's orbit.

The sun is near the vernal equinox around March 21, at the summer solstice around June 21, at the autumnal equinox around September 21, and at the winter solstice around December 21. The exact times can vary slightly each year due to leap years and other factors.

## Geocentric Path of the Planets

All planets, like Earth, orbit the Sun in elliptical orbits. The positions of the planets relative to the Sun and Earth can be described using various angles and configurations.

An exterior planet is one that orbits the Sun outside of Earth's orbit, while an interior planet is one that orbits the Sun inside of Earth's orbit. The planets in our solar system can be classified as either interior or exterior planets based on their position relative to Earth's orbit.

### Phase and Elongation

The elongation $\eta$ of a planet is the angular distance between the Sun and the planet as seen from Earth. It is measured in degrees, with $0^\circ$ being conjunction (when the planet is closest to the Sun) and $180^\circ$ being opposition (when the planet is on the opposite side of the Sun from Earth).

For inferior planets (Mercury and Venus), the maximum elongation is the greatest angular distance they can achieve from the Sun as seen from Earth. The maximum elongation occurs when the planet is at a right angle to the line connecting the Earth and the Sun. The maximum elongation for Mercury is about $28^\circ$, while for Venus it is about $47^\circ$. These planets can never achieve an elongation greater than this, and thus are only seen just before sunrise or just after sunset. Exterior planets can achieve any value of elongation from $0^\circ$ to $180^\circ$.

The phase angle $\phi$ of a planet is the angle subtended by the Sun and the Earth as seen from the planet. It helps in quantifying how much of the planet's illuminated side is visible from Earth.

Interior planets can have any phase angle from $0^\circ$ (new) to $180^\circ$ (full), while exterior planets can have phase angles from $0^\circ$ to some maximum value less than $90^\circ$, which it attains at quadrature (when the planet is at a right angle to the line connecting the Earth and the Sun).

The phase $q$ of a planet is defined as the fraction of the planet's illuminated side that is visible from Earth. It can be calculated using the formula:

$$q = \frac{1 + \cos(\phi)}{2}$$

where $\phi$ is the phase angle. The phase can vary from $0$ (new) to $1$ (full) for interior planets, and from minimum value greater than $0.5$ to $1$ for exterior planets. Thus exterior planets are always seen in gibbous or full phase.

For interior planets, a phase of $0$ corresponds to inferior conjunction (when the planet is between the Earth and the Sun), a phase of $0.5$ corresponds to greatest elongation (when the planet is at its farthest from the Sun as seen from Earth), and a phase of $1$ corresponds to superior conjunction (when the planet is on the opposite side of the Sun from the Earth).

### Planetary Configurations

A planet is said to be in conjunction with the Sun when it is on the same side of the Sun when viewed from Earth, and in opposition when it is on the opposite side of the Sun. When a planet is in opposition, it is at its closest point to Earth and appears fully illuminated.

Only an exterior planet can be in opposition to the Sun, while an interior planet can only be in conjunction with the Sun.

For interior planets, there are two types of configurations: inferior conjunction and superior conjunction. In inferior conjunction, the planet is between the Earth and the Sun, while in superior conjunction, the planet is on the opposite side of the Sun from the Earth.

Inferior planets can also be in greatest elongation, which is the point at which they are farthest from the Sun as seen from Earth. This occurs when the planet is at a right angle to the line connecting the Earth and the Sun.
The planet can either be in the greatest eastern elongation (east of the Sun) or the greatest western elongation (west of the Sun).

Exterior planets can be in quadrature, which is when the planet is at a right angle to the line connecting the Earth and the Sun. This occurs when the planet is 90 degrees away from the Sun as seen from Earth. The planet can either be in eastern quadrature (east of the Sun) or western quadrature (west of the Sun).

### Retrograde Motion

Retrograde motion is the apparent backward motion of a planet as observed from Earth. This occurs when the Earth overtakes an exterior planet in its orbit, causing the planet to appear to move in the opposite direction against the background stars. The period of retrograde motion varies for each planet and can last for several weeks to months.

Only exterior planets can exhibit retrograde motion, as interior planets always move in the same direction as the Earth. The retrograde motion of a planet can be predicted based on its orbital period and the relative positions of the Earth and the planet.

Retrograde motion occurs when the planet is near the opposition point in its orbit. The opposition occurs in the middle of the retrograde loop. The points when the apparent motion of the planet changes from direct to retrograde and vice versa are called stationary points.

### Synodic Period

The synodic period of a planet is the time interval between two successive conjunctions or oppositions of the planet with respect to the Sun as seen from Earth. It is different from the sidereal period, which is the time it takes for a planet to complete one orbit around the Sun with respect to the stars.

Let the sidereal period of the planet be $T_p$ and the sidereal period of the Earth be $T_e$.

For a planet orbiting the Sun in the same direction as Earth, the synodic period $T_s$ is given by:

$$\boxed{\frac{1}{T_s} = \left\lvert \frac{1}{T_p} - \frac{1}{T_e} \right\rvert}$$

If the planet is orbiting the Sun in the opposite direction to Earth, the synodic period $T_s$ is given by:

$$\frac{1}{T_s} = \frac{1}{T_p} + \frac{1}{T_e}$$

The mean solar day is thus just the synodic period of Earth's rotation and its revolution around the Sun.

## Moon

The Moon is Earth's only natural satellite. It orbits the Earth in an elliptical orbit, with a semi-major axis of about 384,400 km, an eccentricity of 0.055, and an orbital tilt of about 5$^\circ$ with respect to the ecliptic plane. The angular diameter of the Moon as seen from Earth varies from about 29.4' to 33.5', with an average of about 31'.

The rotation period of the Moon is equal to its sidereal period, which is about 27.3 days. This means that the same side of the Moon always faces the Earth, a phenomenon known as synchronous rotation or tidal locking. The far side of the Moon is never visible from Earth.

The lunar nodes are the points where the Moon's orbit intersects the ecliptic plane. These nodes precess—with a period of about 18.6 years—due to the gravitational influence of the Sun and the Earth. This is what leads to the nutation of Earth's axis.

### Phases of the Moon

The Moon goes through a cycle of phases as it orbits the Earth. The phases are determined by the relative positions of the Sun, Earth, and Moon. The main phases of the Moon are:

- **New Moon**: The Moon is between the Earth and the Sun, and its illuminated side is facing away from the Earth. Thus it is not visible from Earth, having a phase of 0.
- **Waxing Crescent**: A small sliver of the Moon's illuminated side is visible. It increases in visibility until it reaches the First Quarter phase.
- **First Quarter**: Half of the Moon's illuminated side is visible, with the right side illuminated in the northern hemisphere. It has a phase of 0.5.
- **Waxing Gibbous**: More than half of the Moon's illuminated side is visible, increasing until it reaches the Full Moon phase.
- **Full Moon**: The entire illuminated side of the Moon is visible, with the Earth between the Sun and the Moon. It has a phase of 1.0.
- **Waning Gibbous**: More than half of the Moon's illuminated side is visible, however it is decreasing to the Third Quarter phase.
- **Third Quarter**: Half of the Moon's illuminated side is visible, with the left side illuminated. It has a phase of 0.5.
- **Waning Crescent**: A small sliver of the Moon's illuminated side is again visible, decreasing until it reaches the New Moon phase again.

From new moon to new moon, the Moon takes about 29.5 days, which is known as a synodic month. The synodic month is longer than the sidereal month (27.3 days) due to the Earth's motion around the Sun.

A Metonic cycle is a period of 19 years after which the phases of the Moon repeat on the same days of the year. This is because 19 synodic months are almost equal to 235 lunar months, which is why the lunar calendar is often based on a Metonic cycle.

### Libration

Even though the Moon is tidally locked, we can see a bit more than half of its surface from Earth due to a phenomenon called libration. Libration allows us to see about 59\% of the Moon's surface over time. It occurs due to the tilt of the Moon's orbit, the tilt of the Moon's axis, and the elliptical shape of its orbit.

**Libration in longitude**: This is caused by the elliptical shape of the Moon's orbit. As the Moon moves closer to and farther from the Earth, its angular speed changes, causing it to appear to wobble slightly in longitude. The rotation seems to lag or lead its orbital position. The amplitude of this libration is about 7.8 degrees.

**Libration in latitude**: This is caused by the tilt of the Moon's axis—the tilt between its rotation axis and orbital axis. As the Moon orbits the Earth, we can see slightly more of its northern or southern hemisphere at different times. The amplitude of this libration is about 6.5 degrees.

**Diurnal libration**: This is caused by the observer's position on the Earth's surface. As the Earth rotates, the observer's position changes, allowing them to see slightly more of the Moon's surface at different times of the day. The amplitude of this libration is about 1 degree.

### Eclipses

An eclipse is an event in which a body passes through the shadow of another body. An occultation takes place when an occulting body passes in front of another body, blocking its light. A transit is an event when an inferior planet moves across the solar disk, appearing as a small dot moving across the Sun's face.

A lunar eclipse occurs when the Earth passes between the Sun and the Moon, causing the Earth's shadow to fall on the Moon. The shadow of the Earth has three parts: the umbra (the darkest part), the penumbra (the lighter part), and the antumbra (the region where the shadow is not completely dark).

A total lunar eclipse occurs when the Moon passes through the Earth's umbra, while a partial lunar eclipse occurs when only part of the Moon passes through the umbra. A penumbral lunar eclipse occurs when the Moon passes through the Earth's penumbra, causing a subtle shading on the Moon's surface.

A solar eclipse occurs when the Moon passes between the Sun and the Earth, causing the Moon's shadow to fall on the Earth. It is an occultation of the Sun by the Moon (so not an eclipse by strict definition).

A total solar eclipse occurs when the Moon completely covers the Sun, while a partial solar eclipse occurs when only part of the Sun is covered by the Moon. An annular solar eclipse occurs when the Moon is too far from the Earth to completely cover the Sun, leaving a ring of sunlight visible around the edges of the Moon.

A solar eclipse can only occur during a new moon, while a lunar eclipse can only occur during a full moon. However, not every new moon results in a solar eclipse, and not every full moon results in a lunar eclipse. This is because the Moon's orbit is tilted with respect to the Earth's orbit around the Sun, so the three bodies do not always align perfectly. Thus, for an eclipse to occur, the Moon must be near one of its nodes (the points where its orbit intersects the ecliptic plane) during a new or full moon.

The longest possible duration of a total solar eclipse is about $7^m 30^s$, while the longest possible duration of a total lunar eclipse is about $1^h 40^m$. The frequency of eclipses varies, with at least two solar and two lunar eclipses occurring each year.

A Saros cycle is a period of about 18 years, 11 days, and 8 hours after which the geometry of the Sun, Earth, and Moon repeats, leading to similar eclipses. This cycle is used to predict future eclipses.

## Months and Years

Different types of months and years can be defined based on the motion of the Moon and the Sun.

### Months

A month is a period of time based on the motion of the Moon around the Earth. There are several types of months:

- **Sidereal month**: The time it takes for the Moon to complete one orbit around the Earth with respect to the stars, about 27.3217 days.
- **Synodic month**: The time it takes for the Moon to complete one cycle of phases, from new moon to new moon, about 29.5306 days.
- **Tropical month**: The time it takes for the Moon to return to the same position relative to the Sun, about 27.3216 days.
- **Anomalistic month**: The time it takes for the Moon to return to the same point in its elliptical orbit, about 27.5545 days.
- **Draconic month**: The time it takes for the Moon to return to the same node of its orbit, about 27.2122 days.
