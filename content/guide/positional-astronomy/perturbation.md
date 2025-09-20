---
title: Perturbation in Astronomical Observations
weight: 4
---

When observing celestial objects, several factors can affect the observed position of the object. These factors are discussed below.

## Refraction

Earth's atmosphere is not homogeneous, and its density decreases with altitude. The refractive index of air is slightly greater than 1, and it decreases with altitude. As light enters the Earth's atmosphere from space, it bends towards the normal due to the increase in refractive index. This bending of light causes the apparent position of celestial objects to be different from their true position, and the observed altitude of an celestial object to be slightly higher than its true altitude. The amount of refraction depends on the altitude of the object and the atmospheric conditions, such as temperature and pressure. Altitude is always (except very close to zenith) increased by refraction.

For low zenith angles (high altitudes), the atmosphere can be modelled as a stack of parallel layers of air, each having refractive index $n_i$. Let the true zenith angle of the object be $z$ and apparent zenith angle be $\zeta$. Using snell's law, we get that

$$\sin z = n_{k} \sin z_{k} = n_{k-1} \sin z_{k-1} = \ldots = n_{1} \sin z_{1} = n_0 \sin \zeta$$

We define $R = z - \zeta$ as the refraction angle. It is usually small, so

$$n_0 \sin \zeta = \sin (R + \zeta) \approx R \cos \zeta + \sin \zeta$$
$$\tag{1.4.1} \implies R = k \tan \zeta$$

where $k = n_0 - 1$ is called the constant of refraction. It depends on the atmospheric conditions. At STP conditions, $k \approx 60.3''$.

{{< callout type="image" >}}
{{< svg "pos/refraction.svg" "Refraction" "The bending of light as it passes through the Earth's atmosphere, causing the apparent position of celestial objects to differ from their true position." >}}
{{< /callout >}}

This is a good approximation for $z < 45^\circ$, and fairly accurate for $z < 70^\circ$. For zenith angle close to $90^\circ$, the refraction angle is around $35'$, and is called horizontal refraction. It lengthens the time of sunrise and sunset, and causes the Sun to appear above the horizon even when it has already set.

## Aberration

Since the speed of light is finite, the position of a celestial object as observed from the Earth is slightly different from its true position, shifted in the direction of the motion of Earth, due to the motion of Earth in its orbit around the Sun. This effect is called aberration of light.

The angle of aberration is given by

$$\tag{1.4.2} \alpha = \frac{v}{c} \sin \theta \equiv \kappa \sin \theta$$

where $v$ is the speed of Earth in its orbit, $c$ is the speed of light, and $\theta$ is the angle between the direction of motion of Earth and the direction of the celestial object. Here $\kappa \approx 20.496''$ is called the constant of aberration for Earth.

{{< callout type="image" >}}
{{< svg "pos/aberration.svg" "Aberration" "Here ϕ is the angle θ - α, where α = (v/c) sin θ is the angle of aberration. θ is the angle between the direction of motion of Earth and the direction of the celestial object." >}}
{{< /callout >}}

The rotation of Earth too produces a small effect, but it is negligible compared to the effect of Earth's orbital motion. The total aberration is the vector sum of the aberration due to the Earth's motion in its orbit and the aberration due to the Earth's rotation. The aberration due to Earth's rotation, called diurnal aberration, is given by

$$\tag{1.4.3} \alpha_d = \kappa_d \cos \theta$$

where $\kappa_d \approx 0.32'' \cos \phi$ is the constant of diurnal aberration, and $\phi$ is the observer's latitude.

## Light time correction

Light from a celestial object takes some time to reach the Earth. For example, light from the Sun takes about 499s to reach the Earth. During this time, the Sun moves a bit (as seen from Earth), and so the position of the Sun when the light was emitted is slightly different from its position when the light is observed on Earth. This displacement in the apparent position of a celestial object from its true position is called light time correction (LTC for short).

The reason for this phenomenon is that the speed of light is finite. The magnitude and direction of the displacement in position depends upon the distance of the object from the observer and the motion of the object, and is measured at the instant at which the object's light reaches the observer. It is independent of the motion of the observer. This is in contrast to aberration of light, which depends upon the instantaneous velocity of the observer at the time of observation, and is independent of the motion or distance of the object.

Light time correction is the most pronounced for objects in the solar system, such as planets and asteroids. For example, light from Jupiter takes about 35 minutes to reach the Earth, and during this time, Jupiter moves about 9'' (as seen from Earth during opposition). For this reason, the combined displacement of the apparent position due to the effects of light-time correction and aberration is known as planetary aberration.

Light time correction is negligible for stars, as they are so far away that their motion during the time taken by their light to reach Earth is negligible.

As it turns out however, aberration and light time correction are not independent of each other, but are in fact two aspects of the same phenomenon, namely the finite speed of light, just as seen in two different frames. In the frame of the observer, the effect is seen as aberration, while in the frame of the object, it is seen as light time correction. This [wikipedia article](https://en.wikipedia.org/wiki/Aberration_(astronomy)#Relationship_to_light-time_correction_and_relativistic_beaming) has a detailed discussion on the relationship between aberration and light time correction.

## Parallax

The difference in observed positions of celestial objects when seen from different locations is called parallax. It is the apparent shift of the object against the background of more distant objects, due to the change in the observer's position. The shift in the direction of a star due to annual motion of the Earth around the Sun is called annual parallax or stellar parallax, while the shift in the direction of a star due to the observer's position on the Earth is called diurnal parallax.

During the course of a year, a star will appear to describe a circle if it is at the ecliptic pole, a line segment if it is in the ecliptic plane, and an ellipse otherwise, called as its parallactic ellipse. The semi-major axis of this ellipse is the object's stellar parallax.

For an object with stellar parallax $\pi$, its distance $d$ is given by

$$\tag{1.4.4} d = \frac{1 \mathrm{AU}}{\pi}$$

where 1 AU is the distance from the Earth to the Sun. If $\pi$ is expressed in arcseconds, then

$$\tag{1.4.5} d = \frac{1}{\pi}$$

gives the distance $d$ in units of parsecs. More precisely, one parsec is defined as the distance at which an object has an stellar parallax of one arcsecond.

{{< callout type="trivia" >}}
Stellar parallaxes are so small that they were unobservable until the 19th century, and their apparent absence was used as a scientific argument against heliocentrism during the early modern age. The first experiment to measure parallax was conducted by James Bradley in 1729, but he ended up discovering the aberration of light and nutation of Earth's axis instead. The first successful measurement of stellar parallax was made by Friedrich Bessel in 1838, who measured the parallax of the star 61 Cygni to be $0.3''$, using a device called a heliometer.
{{< /callout >}}

When measuring distances to nearby objects, such as the Moon, planets and asteroids, instead of stellar parallax, diurnal parallax is used. The diurnal parallax is the angle subtended at the object by the radius of the Earth. If $R_\oplus$ is the radius of the Earth, and $d$ is the distance to the object, then the diurnal parallax $\pi_d$ is given by

$$\tag{1.4.6} \pi_d = \frac{R_\oplus}{d}$$

{{< tabs >}}
    {{< tab name="P1" >}}

    Knowing the distance of Sun from Earth is $1 \, \mathrm{AU} = 1.496 \times 10^{11}\, \mathrm{m}$, and the radius of Earth is $R_\oplus = 6.3781 \times 10^{6} \,\mathrm{m}$, find the solar parallax (diurnal parallax of the Sun).

    {{< /tab >}}

    {{< tab name="Solution" >}}

    Using equation (1.4.6), we get that

    $$\pi_d = \frac{R_\oplus}{d} = \frac{6.3781 \times 10^{6}}{1.496 \times 10^{11}} \approx \boxed{8.8''}$$

    Historically, the value of the astronomical unit was unknown, and was determined by measuring the solar parallax. The first attempts at measuring the solar parallax were made during transits of Venus across the Sun, in 1761 and 1769. The currently accepted value of the solar parallax is $8.794''$.

    {{< /tab >}}
{{< /tabs >}}

## Precession

The non-spherical geometry of Earth leads to the sun and moon (and other planets, namely Jupiter) pulling on the Earth's equatorial bulge, which exerts a torque on the planet. Since it is rotating, the torque cannot change the inclination of the equator with respect to the ecliptic, but it can change the direction of the axis of rotation. This results in a slow rotation of the Earth's axis, termed precession. The rotation axis of Earth thus describes a cone about the ecliptic pole having a radius of approximately $23.5^\circ$, with a period of about 25,800 years.

The precession of the axis of rotation is also called precession of the equinoxes, as it causes the equinoxes to shift slowly along the ecliptic. The precession of the equinoxes is about $50.2''$ per year, i.e. the equinoxes move backwards (clockwise) along the ecliptic at a rate of $50.2''$ each year.

Presently, the star closest to the north celestial pole is Polaris (α UMi), but due to precession, the north celestial pole will move away from Polaris and towards the star Vega (α Lyr), which will be closest to the north celestial pole in about 12,000 years. Similarly, the south celestial pole will move towards the star Achernar (α Eri) in about 12,000 years. Thuban (α Dra) was the closest star to the north celestial pole about 4,000 years ago.

The tropical year - the time interval between successive passages of sun through the vernal equinox - is about 20 minutes shorter than the sidereal year - the time interval between successive passages of sun through the same point in the ecliptic, because of the precession of equinoxes.

## Nutation

Moon's orbital plane is tilted with respect to the eliptic, resulting in precession of its orbital plane with a period of about 18.6 years. This causes the ecliptic to oscillate slightly, resulting in a small oscillation of the celestial poles and equinoxes, called nutation.

The nutation is superimposed on the precession of the equinoxes, and has a maximum amplitude of about $9.2''$, i.e. nutation leads to change in ecliptic obliquity of Earth with a period of about 18.6 years, with a maximum amplitude of about $9.2''$.

We studied in chapter 1.3 that the vernal equinox ♈︎ is the intersection of the celestial equator and the ecliptic, and is a point fixed to the celestial sphere, unchanging with time. However, now we know that the celestial poles and the celestial equator slowly change their positions over time, and so do the equinoxes. Taking into account precession and nutation, the position of ♈︎ can be calculated for any time. If nutation variations are ignored, the position of ♈︎ at any time defined the mean sidereal time (MST). If nutational variations are included, the position of ♈︎ at any time defines the apparent sidereal time (AST). The equation of equinoxes is defined as

$$ \mathcal{E}_\gamma = \text{AST} - \text{MST} $$

It fluctuates around $-1^s$.

## Correction for observer's altitude

If the observer is at some altitude $h$ above the sea level, the observer's horizon will no longer be a straight line. The observer will be able to see more than half of the sky at any given time, due to the curvature of the Earth. This leads to change in rise and set times of celestial objects.

The dip of the horizon $\delta$ is defined as the angle between the true horizontal and the line of sight to the horizon. It is given by

$$\tag{1.4.7} \cos \delta = \frac{R_\oplus}{R_\oplus + h} \implies \delta \approx \sqrt{\frac{2 h}{R_\oplus}}$$

The horizon distance $d_h$ is defined as the distance to the point (along the surface of the Earth) where a horizontal line from the observer's eye intersects the sea level. It is given by

$$\tag{1.4.8} d_h = R_\oplus \delta \approx \sqrt{2 h R_\oplus}$$

If $h$ is measured in meters,

$$\delta \approx 1.93' \sqrt{h}$$
$$d_h \approx 3.57 \sqrt{h} \,\, \mathrm{km}$$

## Proper Motion

Stars are not fixed in the sky, but move slowly relative to the Sun and the Earth. The motion of a star relative to the Sun is called its proper motion. It is usually expressed in terms of the projected angular velocity, i.e. the change in position of the star on the celestial sphere per year, in units of arcseconds per year. This only gives the tangential component of the motion, as it does not take into account the radial component of the motion, i.e. the change in distance of the star from the Sun. The radial component of motion, called the radial velocity can be measured using the Doppler effect, and is usually expressed in km/s.

If $\mu_\alpha$ is the rate of change of the RA of a star, and $\mu_\delta$ is the rate of change of the declination, then the proper motion is given by

$$\tag{1.4.9} \mu = \sqrt{\mu_\alpha^2 \cos^2 \delta + \mu_\delta^2}$$

If the star is at a distance $r$ from the observer, then the tangential velocity $v_t$ of the star is given by

$$\tag{1.4.10} v_t = \mu r$$

If $\mu$ is expressed in arcseconds per year, and $r$ in parsecs, then the tangential velocity $v_t$ in km/s is given by

$$v_t \approx 4.74 \, \mu r$$

The star with the greatest proper motion is Barnard's star, which has a proper motion of about $10.3''$ per year, and a tangential velocity of about $90$ km/s.

If the radial component of a star's velocity is $v_r$, its net velocity $v$ is given by

$$\tag{1.4.11} v = \sqrt{v_t^2 + v_r^2}$$
