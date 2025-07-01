---
title: Perturbation in Astronomical Observations
weight: 4
---

When observing celestial objects, several factors can affect the observed position of the object. These factors include atmospheric refraction, observer's altitude, aberration of light, parallax, precession, nutation, and proper motion of the star.

## Refraction

Since light is refracted by the Earth's atmosphere, the observed altitude of a celestial object is slightly higher than its true altitude. This effect is called atmospheric refraction. The amount of refraction depends on the altitude of the object and the atmospheric conditions, such as temperature and pressure.

The atmosphere can be modelled as a stack of parallel layers, each having refractive index $n_i$. Let the true zenith angle of the object be $z$ and apparent zenith angle be $\zeta$. Using snell's law, we get that

$$\sin z = n_{k} \sin z_{k} = n_{k-1} \sin z_{k-1} = \ldots = n_{1} \sin z_{1} = n_0 \sin \zeta$$

Define the refraction angle as $R = z - \zeta$. It is usally small, so

$$n_0 \sin \zeta = \sin (R + \zeta) \approx R \cos \zeta + \sin \zeta$$
$$\implies R = (n_0 - 1) \tan \zeta$$

At STP conditions, $n_0 - 1 \approx 60.3''$ and is called the constant of refraction.

This is a good approximation for $z < 45^\circ$, and fairly accurate for $z < 70^\circ$. For zenith angle close to $90^\circ$, the refraction angle is around $35'$ and is called horizontal refraction. It lengthens the time of sunrise and sunset, and causes the Sun to appear above the horizon even when it is below it.

## Correction for observer's altitude

If the observer is at some altitude $h$ above the sea level, the observer's horizon will no longer be a straight line. The observer will be able to see more than half of the sky at any given time, due to the curvature of the Earth.

## Aberration

Since the speed of light is finite, the position of a celestial object as observed from the Earth is slightly different from its true position, shifted in the direction of the motion of Earth, due to the motion of the Earth in its orbit around the Sun. This effect is called aberration of light.

The angle of aberration is given by

$$\alpha = \frac{v}{c} \sin \theta \equiv \kappa \sin \theta$$

where $v$ is the velocity of the Earth in its orbit, $c$ is the speed of light, and $\theta$ is the angle between the direction of motion of the Earth and the direction of the celestial object. Here $\kappa \approx 20.496''$ is the constant of aberration for Earth.

The rotation of Earth too produces a small effect, but it is negligible compared to the effect of the Earth's orbit. The total aberration is the vector sum of the aberration due to the Earth's motion in its orbit and the aberration due to the Earth's rotation. The aberration due to Earth's rotation, called diurnal aberration, is given by

$$\alpha_d = \kappa_d \cos \phi$$

where $\phi$ is the observer's latitude, and $\kappa_d \approx 0.32''$ is the constant of diurnal aberration.

## Parallax

The difference in observed positions of celestial objects when seen from different locations is called parallax. It is the apparent shift of the object against the background of more distant objects, due to the change in the observer's position. The shift in the direction of a star due to annual motion of the Earth around the Sun is called annual parallax, while the shift in the direction of a star due to the observer's position on the Earth is called diurnal parallax.

During the course of a year, a star will appear to describe a circle if it is at the ecliptic pole, a line segment if it is in the ecliptic plane, and an ellipse otherwise, called as the parallactic ellipse. The semi-major axis of the ellipse is the annual parallax.

For an object with annual parallax $\pi$, its distance $d$ is given by

$$d = \frac{1 \mathrm{AU}}{\pi}$$

where $1 \mathrm{AU}$ is the distance from the Earth to the Sun. If $\pi$ is expressed in arcseconds, then

$$d = \frac{1}{\pi}$$

gives the distance $d$ in units of parsecs. More precisely, one parsec is defined as the distance at which an object has an annual parallax of one arcsecond.

## Precession

The non-spherical geometry of Earth leads to the sun and moon pulling on the Earth's equatorial bulge, which results in a torque. Since the Earth is rotating, the torque cannot change the inclination of the equator with respect to the ecliptic, but it can change the direction of the axis of rotation. This results in a slow rotation of the Earth's axis, called precession. The rotation axis of Earth thus describes a cone about the ecliptic pole of a radius of $23.5^\circ$, with a period of about 26,000 years.

The precession of the axis of rotation is called precession of the equinoxes, as it causes the equinoxes to shift slowly along the ecliptic. The precession of the equinoxes is about $50.2''$ per year, i.e. the equinoxes move backwards (clockwise) along the ecliptic at a rate of $50.2''$ each year.

Presently, the star closest to the north celestial pole is Polaris, but due to precession, the north celestial pole will move away from Polaris and towards the star Vega, which will be closest to the north celestial pole in about 12,000 years. Similarly, the south celestial pole will move towards the star Achernar in about 12,000 years. Thuban was the closest star to the north celestial pole about 4,000 years ago.

The tropical year - the time interval between successive passages of sun through the vernal equinox - is shorter than the sidereal year - the time interval between successive passages of sun through the same point in the ecliptic. The difference of about 20 minutes is due to precession of the equinoxes.

## Nutation

Moon's orbital plane is tilted with respect to the eliptic, resulting in precession of its orbital plane with a period of about 18.6 years. This causes the ecliptic to oscillate slightly, resulting in a small oscillation of the celestial poles and equinoxes, called nutation.

The nutation is superimposed on the precession of the equinoxes, and has a maximum amplitude of about $9.2''$, i.e. nutation leads to change in ecliptic obliquity of Earth with a period of about 18.6 years, with a maximum amplitude of about $9.2''$.

## Proper Motion

Stars are not fixed in the sky, but move slowly relative to the Sun and the Earth. The motion of a star relative to the Sun is called proper motion. It is usually expressed in terms of the projected angular velocity, i.e. the change in position of the star on the celestial sphere per year, in units of arcseconds per year. This only gives the tangential component of the motion, as it does not take into account the radial component of the motion, i.e. the change in distance of the star from the Sun. The radial component of motion, called the radial velocity can be measured using the Doppler effect, and is usually expressed in km/s.

If $\mu_\alpha$ is the rate of change of the RA of a star, and $\mu_\delta$ is the rate of change of the declination, then the proper motion is given by

$$\mu = \sqrt{\mu_\alpha^2 \cos^2 \delta + \mu_\delta^2}$$

If the star is at a distance $r$ from the observer, then the tangential velocity $v_t$ of the star is given by

$$v_t = \mu r$$

If $\mu$ is measured in arcseconds per year, and $r$ in parsecs, then the tangential velocity $v_t$ is given in km/s by

$$v_t \approx 4.74 \mu r$$

The star with the greatest proper motion is Barnard's star, which has a proper motion of about $10.3''$ per year, and a tangential velocity of about $90$ km/s.

If the radial component of a star's velocity is $v_r$, its net velocity $v$ is given by

$$v = \sqrt{v_t^2 + v_r^2}$$
