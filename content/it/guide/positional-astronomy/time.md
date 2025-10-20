---
title: Time
weight: 3
---

## Sidereal Time

Local sidereal time (LST) is defined as the hour angle of the vernal equinox ♈︎.

$$\tag{1.3.1} \text{LST} = \text{HA}_\gamma$$

How does one find the local sidereal time in practice? Let's say an object with right ascension $\text{RA}_X$ is observed to have an hour angle $\text{HA}_X$. Since the hour angle is the angle between the observer's meridian and the hour circle passing through the object, and the right ascension is the angle between the vernal equinox ♈︎ and the hour circle passing through the object, it follows that the angle between the observer's meridian and ♈︎ is simply the sum of these two angles. Thus, we find that the local sidereal time is simply the sum of the hour angle and right ascension of the object.

$$\tag{1.3.2} \boxed{\text{LST} = \text{HA}_\gamma = \text{HA}_X + \text{RA}_X}$$

The time between transits of a celestial object over the Greenwich meridian and the local observer's meridian defines the longitude of the observer. The hour angle of an object $X$ as seen from the Greenwich meridian is termed the Greenwich hour angle of the object (GHA). Similarly, the Greenwich sidereal time (GST) is defined as the hour angle of the vernal equinox ♈︎ as seen from the Greenwich meridian. For an observer at longitude $\lambda$ (taken positive westwards),

$$\tag{1.3.3} \text{GST} = \text{LST} + \lambda$$
$$\tag{1.3.4} \boxed{\text{GHA}_X = \text{HA}_X + \lambda}$$

A sidereal day is the time interval between successive transits of the vernal equinox ♈︎ over the observer's meridian. The sidereal day is about 4 minutes shorter than the mean solar day, lasting about $23^h \, 56^m \, 4.1^s$ in mean solar time (equivalent to $24^h$ in sidereal time). It starts when ♈︎ transits across the observer's meridian and lasts until ♈︎ transits the meridian again.

## Mean and True Solar Time

One apparent solar day is the time between successive passages of the Sun across the observer's meridian. Apparent solar time is defined as the hour angle of the Sun.

For day-to-day timekeeping, we need a uniform duration for the day. The apparent solar day is not uniform and varies throughout the year. This is because of two reasons:

1. The Earth's axial tilt causes the Sun's path to vary in declination throughout the year.
2. The Earth's elliptical orbit means that the Sun's angular speed is not constant.

To overcome this, we define the mean Sun as a fictitious body, which moves along the celestial equator in the direction of increasing RA (eastwards) at a constant angular velocity equal to the mean angular velocity of the true Sun. The time between successive passages of the mean Sun over the observer's meridian is called the mean solar day.

{{< callout type="remark" >}}
To define the position of the mean Sun with respect to the Sun in more detail, we define another fictitious body, called the dynamical mean Sun. It starts off from the perigee with the Sun, moves along the ecliptic with angular velocity equal to the Sun's mean angular velocity, and returns to the perigee at the same time as the Sun. When the dynamical mean Sun reaches the vernal equinox ♈︎, the mean Sun starts off along the celestial equator, returning to ♈︎ at the same time as the dynamical mean Sun.
{{< /callout >}}

The mean solar time (MST) is defined as the hour angle of the mean Sun.

The equation of time is defined as the difference between the apparent solar time and the mean solar time, or the difference between the time of passage of the Sun and the mean Sun over the observer's meridian.

$$\tag{1.3.5} \boxed{\mathcal{E} = \text{HA}_\odot - \text{HA}_{MS}} $$

When the hour angle of the mean Sun is zero, it is said to be mean noon. When the hour angle of the true Sun is zero, it is said to be solar noon. The time difference between the two is equal to the equation of time.

From equation (1.3.2), we have

$$\text{LST} = \text{HA}_\odot + \text{RA}_\odot = \text{HA}_{MS} + \text{RA}_{MS}$$

Hence, the equation of time can also be expressed as $\mathcal{E} = \text{RA}_{MS} - \text{RA}_\odot$.

We define Greenwich Mean Time (GMT) or Universal Time (UT) as

$$\tag{1.3.6} \boxed{\text{GMT} = \text{GHA}_{MS} + 12^h = \text{GHA}_\odot - \mathcal{E} + 12^h}$$

Thus, the GMT at solar noon at Greenwich is

$$\text{GMT}_{\odot , G} = 12^h - \mathcal{E}$$

{{< callout type="remark" >}}
Readings in sidereal time and mean solar time can be interconverted by scaling with appropriate factors:

$$\text{ST} \cdot 365.2422 = \text{MST} \cdot 366.2422$$

This shows that one sidereal day is approximately $23^h 56^m 4.1^s$ in mean solar time. The reason for this is that the Earth has to rotate a little more than one full rotation for the Sun to return to the same position in the sky, due to the Earth's motion in its orbit around the Sun.

{{< callout type="image" >}}
{{< png "pos/sidereal.png" "Sidereal Time" "The difference in sidereal time and solar time arises due to the Earth's rotation and its orbit around the Sun." >}}
{{< /callout >}}

{{< /callout >}}

## Civil Time

Earth has been divided into 24 standard time zones. Within each zone, the same civil mean time, called Zone Time (ZT), is followed. Each zone is around $15^\circ$ ($1^h$) wide, although the actual boundaries are irregular, following political boundaries.

The Greenwich Zone (Zone 0) lies between the longitudes $0^h 30^m$ E and $0^h 30^m$ W. Zone +1 lies between $0^h 30^m$ E and $1^h 30^m$ E, Zone -1 lies between $0^h 30^m$ W and $1^h 30^m$ W, and so on. The time followed in each zone is the mean solar time at the central meridian of the zone. Zones +12 and -12 lie between $11^h 30^m$ W to $12^h$ W and $11^h 30^m$ E to $12^h$ E respectively, both keeping the time of the $12^h$ meridian. The meridian separating them is the International Date Line (IDL). Crossing it from east to west omits one day, and crossing from west to east adds one day.

The Greenwich date is defined as GMT plus the date at Greenwich. The Greenwich Mean Time is related to the zone time at an observer's meridian by

$$\tag{1.3.7} GMT = ZT + \lambda$$

where $\lambda$ is the longitude of the central meridian of the zone (positive westwards), and $ZT$ is the zone time at the observer's meridian.

## Years

A year is a period of time based on the motion of the Earth around the Sun. There are several types of years:

- **Tropical year**: The time it takes for the Earth to complete one orbit around the Sun, or for the ecliptic longitude of the Sun to increase by 360$^\circ$, defined to be exactly 365.24219 days. This is the basis for the Gregorian calendar, which is the calendar followed by most of the world today.
- **Sidereal year**: The time it takes for the Earth to complete one orbit around the Sun with respect to the stars, about 365.2566 days. This is slightly longer than the tropical year due to the precession of the equinoxes.
- **Anomalistic year**: The time it takes for the Earth to return to the same point in its elliptical orbit, about 365.2596 days. This is the time between successive perihelion passages.
- **Draconic year**: The time it takes for the Earth to return to the same node of its orbit (the point where the orbit crosses the ecliptic), about 346.6201 days. This is the time between successive passages of the Sun through the same node of the Moon's orbit.
- **Lunar year**: A year based on the cycles of the Moon, consisting of 12 synodic months, which is about 354.37 days. This is shorter than the tropical year, leading to the need for intercalation in lunar calendars to keep them aligned with the seasons.

In the Gregorian calendar, a normal year consists of 365 days. However, every fourth year is a leap year, having 366 days. Furthermore, every year divisible by 100 and not by 400 is not a leap year. Thus, the year 2000 was a leap year, but 1900 was not.

Julian dates are used by astronomers to give each day a running number. A Julian century is 36,525 days long. The starting date was chosen as January 1, 4713 BC in the Julian calendar, which is equivalent to November 24, 4714 BC in the proleptic Gregorian calendar.
