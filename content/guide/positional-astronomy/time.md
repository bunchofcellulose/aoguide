---
title: Time
weight: 3
---

## Sidereal Time

The local sidereal time is defined as the hour angle of vernal equinox ♈︎.

$$\boxed{\text{LST} = \text{HA}_\gamma}$$

If the hour angle and right ascension of some object $X$ are known, the local sidereal time can be calculated as

$$\text{LST} = \text{HA}_X + \text{RA}_X$$

where $\text{HA}_X$ is the hour angle of object $X$ and $\text{RA}_X$ is the right ascension of object $X$.

The position of the vernal equinox ♈︎ changes over time due to precession and nutation. The equinoxes move backwards with time, the steady mean backward motion termed general precession. If nutation variations are ignored, the position of ♈︎ at any time defined the mean sidereal time (MST). If nutational variations are included, the position of ♈︎ at any time defines the apparent sidereal time (AST). The equation of equinoxes is defined as

$$ \mathcal{E}_\gamma = \text{AST} - \text{MST} $$

It fluctuates around $-1^s$.

The time between transits of a celestial object over the Greenwich meridian and the local observer's meridian defines the longitude of the observer. The hour angle of an object as seen from the Greenwich meridian is the Greenwich hour angle (GHA). Similary, the Greenwich sidereal time (GST) is defined as the hour angle of the vernal equinox ♈︎ as seen from the Greenwich meridian. For an observer at longitude $\lambda$ (taken positive westwards),

$$\text{GST} = \text{LST} + \lambda$$
$$\boxed{\text{GHA}_X = \text{HA}_X + \lambda}$$

The sidereal day stars when ♈︎ transits across the observer's meridian and lasts 24 sidereal hours, until ♈︎ transists the meridian again.

## Mean and True Solar Time

One apparent solar day is the time between successive passages of the sun across observer's meridian. Its length varies through the year due to Earth's axial tilt and elliptical orbit.

To overcome this, we define the mean sun as a fictitious body, which moves along the celestial equator in the direction of increasing RA at a constant angular velocity equal to the mean angular velocity of the real sun. The time between successive passages of the mean sun over the observer's meridian is called mean solar day.

A fictitious body called the dynamical mean sun starts off from the perigee with the sun, moves along the ecliptic with angular velocity equal to the sun's mean angular velocity and returns to the perigee at the same time as the sun. When the dynamical mean sun reaches the vernal equinox ♈︎, the mean sun starts off along the celestial equator, returning to ♈︎ at the same time as the dynamical mean sun.

The equation of time is defined as the difference between the apparent solar time and the mean solar time, or the difference between the time of passage of the sun and the mean sun over the observer's meridian.

$$ \mathcal{E} = \text{HA}_\odot - \text{HA}_{MS} $$

When hour angle of mean sun is zero, it is said to be mean noon. When the hour angle of the true sun is zero, it is said to be solar noon. The time difference between the two is called the equation of time.

$$\text{LST} = \text{HA}_\odot + \text{RA}_\odot = \text{HA}_{MS} + \text{RA}_{MS}$$

Hence the equation of time can also be expressed as $\mathcal{E} = \text{RA}_{MS} - \text{RA}_\odot$.

We define Greenwich mean time (GMT) or universal time (UT) as

$$\boxed{\text{GMT} = \text{GHA}_{MS} + 12^h = \text{GHA}_\odot - \mathcal{E} + 12^h}$$

Thus the GMT at solar noon at Greenwich is

$$\text{GMT}_{\odot , G} = 12^h - \mathcal{E}$$

Readings in sidereal time and mean solar time can be interconverted by scaling with appropriate factors:

$$\text{LST} = \text{MST} \cdot \frac{366.2422}{365.2422}$$

Thus one sidereal day is approximately $23^h 56^m 4.1^s$ in mean solar time.

## Civil Time

Earth has been divided into standard time zones. Within each zone the same civil mean time called Zone Time (ZT) is used. Each zone is around $15^\circ$ ($1^h$) wide.

Greenwich Zone (Zone 0) lies between the longitudes $0^h 30^m$ E and $0^h 30^m$ W. Zone +1 lies between $0^h 30^m$ E and $1^h 30^m$ E, Zone -1 lies between $0^h 30^m$ W and $1^h 30^m$ W, and so on. The time followed in each zone is the mean solar time at the central meridian of the zone. Zone +12 and -12 lie between $11^h 30^m$ W to $12^h$ W and $11^h 30^m$ E to $12^h$ E respectively, both keeping a time of the $12^h$ meridian. The meridian separating them is the International Date Line (IDL). Crossing it from east to west omits one day, and crossing from west to east adds one day. The Greenwich date is defined as GMT plus the date at Greenwich.

$$GMT = ZT + \lambda$$

where $\lambda$ is the longitude of the central meridian of the zone, and $ZT$ is the zone time at observer's meridian.

The civil year is based on the tropical year, the time interval between successive passages of the sun through the vernal equinox ♈︎, and equal to 365.2422 mean solar days.

A normal year consists of 365 days, and every fourth year is a leap year, having 366 days. Every century except those divisible by 400 is not a leap year. Thus the year 2000 was a leap year, but 1900 was not. This is the Gregorian calendar, which is the most widely used civil calendar today.

Julian dates are used by astronomers to give each day a running number. A Julian century is 36,525 days long. The starting date was chosen as January 1, 4713 BC in the Julian calendar, which is equivalent to November 24, 4714 BC in the proleptic Gregorian calendar.
