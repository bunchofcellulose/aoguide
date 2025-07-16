---
title: Kepler's Laws
prev: /guide/celestial-mechanics/
weight: 1
---

We start here by a study of "celestial mechanics", studying the interaction of bodies through gravitation forces. 

<<<<<<< HEAD
The basic law preluding it is Newton's law of universal gravitation, which is the classical description of gravity (we'll see a bit of the modern modification to it, the study of general relativity later on). Consider two bodies of masses $m_1$ and $m_2$, with position vectors $\mathbf{r_1}$ and $\mathbf{r_2}$. The force exerted on body 2 due to body 1, described by Newton's law of universal gravitation is:
=======
The basic law preluding it is Newton's law of universal gravitation, which is the classical description of gravity (we'll see a bit of the modern modification to it, the study of general relativity later on). 

Consider two bodies of masses $m_1$ and $m_2$, with position vectors $\mathbf{r_1}$ and $\mathbf{r_2}$. The force exerted on body 2 due to body 1, described by Newton's law of universal gravitation is:
>>>>>>> 7e30e386a5e13892d95d8dcb3702b0e45221b6a8

$$\tag{3.1.1} \mathbf{F} = -\frac{G m_1 m_2}{|\mathbf{r_2} - \mathbf{r_1}|^3} (\mathbf{r_2} - \mathbf{r_1}) $$

Here G is the universal gravitational constant, equal to $6.67430 \times 10^{-11} \: \mathrm{m^3\,kg^{-1}\,s^{-2}}$.

<<<<<<< HEAD
The problem we're going to tackle is Kepler's two body problem, which asks to calculate and predict the motion of two bodies under the influence of their mutual gravitational attraction. The two bodies are assumed to be point masses, and the force acting on them is given by Newton's law of gravitation. We'll see later that the problem for a higher amount of bodies is unsolvable, but we can still talk about some reduced cases.
=======
The problem we're going to tackle is Kepler's two body problem, which asks to calculate and predict the motion of two bodies under the influence of their mutual gravitational attraction. The two bodies are assumed to be point masses, and the force acting on them is given by Newton's law of gravitation. 

We'll see later what we can say about the other cases of the $n$ body problem.
>>>>>>> 7e30e386a5e13892d95d8dcb3702b0e45221b6a8

To solve for the trajectories of the two bodies, it is most convenient to work in the center of mass frame. The center of mass $\mathbf{R}$ of the two body system is given by

$$ \mathbf{R} = \frac{m_1 \mathbf{r_1} + m_2 \mathbf{r_2}}{m_1 + m_2} $$

The position vectors of the two bodies with respect to the center of mass are given by

$$
\mathbf{r_1} = \frac{-m_2}{M} \mathbf{r} + \mathbf{R} \qquad \qquad
\mathbf{r_2} = \frac{m_1}{M} \mathbf{r} + \mathbf{R}
$$

where $M = m_1 + m_2$ is the total mass of the system, and $\mathbf{r} = \mathbf{r_2} - \mathbf{r_1}$ is the vector joining the two bodies, also called the separation vector.

Working in the center of mass frame, $\mathbf{R} = \dot{\mathbf{R}} = \mathbf{0}$, since there are no external forces. With this, we now only have to solve for the trajectory of the separation vector $\mathbf{r}$, as a function of time. Note that the center of mass frame is an inertial frame, so we can apply Newton's second law to it.

To simplify the algebra, we define the reduced mass $m$ of the two body system as

$$\tag{3.1.2} m = \frac{m_1 m_2}{m_1 + m_2} $$

such that $Mm = m_1 m_2$. Further, we define the gravitational parameter $\mu$ as

$$\tag{3.1.3} \mu = G M = G (m_1 + m_2) $$

The force acting on the two bodies are

$$
\mathbf{F_1} = \mu m \frac{\mathbf{r}}{r^3} \qquad \qquad
\mathbf{F_2} = -\mu m \frac{\mathbf{r}}{r^3}
$$

Using Newton's second law $\mathbf{F} = m \mathbf{a}$, we can write

$$
\ddot{\mathbf{r}}_1 = \frac{\mu m}{m_1} \frac{\mathbf{r}}{r^3} \qquad \qquad
\ddot{\mathbf{r}}_2 = -\frac{\mu m}{m_2} \frac{\mathbf{r}}{r^3}
$$

Subtracting the two equations, we get

$$\tag{3.1.4} \boxed{\ddot{\mathbf{r}} = -\mu \frac{\mathbf{r}}{r^3}} $$

{{< callout type="remark" >}}
In the limit $m_1 \gg m_2$, we get that

- $M = m_1$
- $m = m_2$
- $\mathbf{r_1} = \mathbf{0}$
- $\mathbf{r_2} = \mathbf{r}$

We see that the trajectory of the separation vector is simply the trajectory of the smaller mass, $m_2$, in the center of mass frame, while the larger mass $m_1$ is at rest. This is the case when one of the bodies is much heavier, for instance the motion of Earth around the Sun.  

The separation vector $\mathbf{r}$ also gives the trajectory of one of the bodies when viewed in the frame of the other body (which is a non-inertial frame).
{{< /callout >}}

## Constants of Motion

There are a couple of observations we can make here to simplify the tasks. The first is to look for invariants, quantities that don't change. These turn out to be quite helpful (and sometimes we can't
even solve the problem without them!). Because the force is along the line joining the two masses, it makes sense to think about the angular momentum, because the force is central in a sense. 

In particular, because the force on the reduced mass is $f(r) \mathbf{\hat{r}}$, the "angular momentum", $\mathbf{r} \times m\mathbf{\dot{r}}$ is constant.

The total orbital angular momentum is given by
$$
\begin{align*}
\mathbf{L} &= m_1 \mathbf{r_1} \times \mathbf{v_1} + m_2 \mathbf{r_2} \times \mathbf{v_2}   \\
& = m \mathbf{r} \times \mathbf{v} \\
\end{align*}
$$

where $\mathbf{v} = \dot{\mathbf{r}}$. The algebra is a little tricky, 
and offers no insight, so I've ommited it, but you should go through it once (you'll actually get a $\mathbf{\dot{R}}$ term as well, but see the energy discussion later). Anyway, from our previous discussion, this is an invariant.

The total energy of the system is given by

$$
\begin{align*}
E &= \frac{1}{2} m_1 v_1^2 + \frac{1}{2} m_2 v_2^2 - \frac{G m_1 m_2}{|\mathbf{r_1} - \mathbf{r_2}|^2} \\
  &= \frac{1}{2} m_1 \left(\mathbf{\dot{R}} - \frac{m_2}{M} \mathbf{\dot{r}}\right)^2 + \frac{1}{2} m_2 \left(\mathbf{\dot{R}} + \frac{m_1}{M} \mathbf{\dot{r}}\right)^2 - \frac{G m_1 m_2}{|\mathbf{r_1} - \mathbf{r_2}|^2}\\
  &= \frac{1}{2}M\mathbf{\dot{R}}^2 + \frac{1}{2} m v^2 - \mu \frac{m}{r^2}
\end{align*}
$$

but since the COM does not experience a net force, $\mathbf{\dot{R}}$ is constant, so we might as well discard it. Then our modified energy becomes, 

$$
E \to \frac{1}{2} m v^2 - \mu \frac{m}{r^2}
$$
which is an invariant because the gravitational force is conservative. Alternatively, $\mathbf{\dot{R}}$ is just 0 in the com frame, so the energy in the COM frame is simply this.

We define the specific angular momentum and specific energy as

$$
\begin{align*}
\mathbf{h} &= \frac{\mathbf{L}}{m} = \mathbf{r} \times \dot{\mathbf{r}}\\
\tag{3.1.1} \varepsilon &= \frac{E}{m} = \frac{1}{2} v^2 - \frac{\mu}{r}
\end{align*}
$$

Since both energy and angular momentum are invariants, so are $\mathbf{h}$ and $\varepsilon$.

Since $\mathbf{h} \cdot \mathbf{r} = 0$, $\mathbf{h}$ lies perpendicular to the plane of motion, and hence defines the plane of motion, which must be fixed because $\mathbf{h}$ is constant. 

We define the eccentricity vector as

$$\tag{3.1.2} \mathbf{e} = -\frac{\mathbf{h} \times \dot{\mathbf{r}}}{\mu} - \frac{\mathbf{r}}{r} $$

Taking its time derivative

$$
\begin{align*}
\frac{d}{dt} \mathbf{e} &= \frac{d}{dt} \left( -\frac{\mathbf{h} \times \dot{\mathbf{r}}}{\mu} - \frac{\mathbf{r}}{r} \right) \\
&= -\frac{1}{\mu} \left(\mathbf{h} \times \ddot{\mathbf{r}} \right) - \left( \frac{\dot{{\mathbf{r}}}}{r} - \frac{\dot{r}}{r^2} \mathbf{r} \right)\\
&= -\frac{1}{\mu} \left( \left( \mathbf{r} \times \dot{\mathbf{r}} \right) \times \left(-\mu \frac{\mathbf{r}}{r^3} \right) \right) - \left( \frac{\dot{{\mathbf{r}}}}{r} - \frac{\dot{r}}{r^2} \mathbf{r} \right)\\
&= \frac{1}{r^3} \left[(\mathbf{r} \cdot \mathbf{r}) \dot{\mathbf{r}} - (\mathbf{r} \cdot \dot{\mathbf{r}}) \times \mathbf{r} \right] - \left( \frac{\dot{{\mathbf{r}}}}{r} - \frac{\dot{r}}{r^2} \mathbf{r} \right)\\
&= \frac{1}{r^3} \left( r^2 \dot{\mathbf{r}} - r \dot{r} \mathbf{r} - r^2 \dot{\mathbf{r}} + r \dot{r} \mathbf{r} \right)\\
&= 0\\
\end{align*}
$$

we find that the eccentricity vector does not change with time, hence is also a constant of motion. It lies in the plane of motion ($\mathbf{h} \cdot \mathbf{e} = 0$) and points in the direction of the periapsis. The magnitude of the eccentricity vector is given by

$$\tag{3.1.3} e = \sqrt{1 + \frac{2 \varepsilon h^2}{\mu^2}} $$

I can't quite give you a motivation for the eccentricity vector, there is *some* rhyme or reason to it, but justifying it is a great task in itself, so I must ask you to take my word for this. If you want, you can read more: (TODO: Maybe add some optional reading on this?)
The magnitude of the eccentricity vector (as we'll see in a bit), determins the eccentricity of a planetary orbit, but this is sadly not
very apparent from our definition.

## First Law

Kepler's first law of planetary motion states that the orbit of a planet is an ellipse with the sun at one of the foci.

First, we can ask what the solutions for the trajectories of particles in such a system are. Also we'll be using properties 
of ellipse somewhat freely for the next sections, so if you aren't familiar with them, I'd recommend reading the wikipidea page: https://en.wikipedia.org/wiki/Ellipse. The sections of importance are mostly the cartesian co-ordinates one, and metric properties.

To do this we define a new quantity (we don't necessarily need it, but its very useful later, so I might as well define it here), we call the angle between the eccentricity vector and the position vector the *true anamoly*, $\theta$. We can use this to take the dot product:

$$ \mathbf{r} \cdot \mathbf{e} = r e \cos \theta = \mathbf{r} \cdot \left( -\frac{\mathbf{h} \times \dot{\mathbf{r}}}{\mu} - \frac{\mathbf{r}}{r} \right) = \frac{h^2}{\mu} - r$$

$$\tag{3.1.4} \implies \boxed{r = \frac{h^2 / \mu}{1 + e \cos \theta}} $$

Note that this, if you have seen it before, is the equation of a conic section in polar coordinates, with the focus being at origin, the eccentricity being $e$ and the length of the semi-latus rectum being $p = \frac{h^2}{\mu}$, which gives the relation

$$\tag{3.1.5} h = \sqrt{\mu p}$$

The magnitude of $\mathbf{e}$ determines the shape of the trajectory:

- $e = 0$: Circle
- $0 \leq e < 1$: Ellipse
- $e = 1,\, h \neq 0$: Parabola
- $e > 1$: Hyperbola
- $e = 1,\, h = 0$: Straight line (degenerate conic section)

where the focus of the conic section lies at the origin of our system, i.e at the center of mass of the system.

The individual trajectories of the two bodies in the center of mass frame is therefore

$$ r_1 = \frac{m_2}{M} \frac{h^2 / \mu}{1 + e \cos \theta} \,, \qquad \qquad r_2 = \frac{m_1}{M} \frac{h^2 / \mu}{1 + e \cos \theta} $$

Of course because the centre of mass is fixed, the trajectories of the two bodies however will be oriented opposite to each other in our frame, with an angle of $\pi$ radian between them, to keep the center of mass fixed.

We can actually determine the energy of the system can by just the eccentricity $e$ and length of semi-latus rectum $p$ of the trajectory. Consider the dot product, $\mathbf{e} \cdot \mathbf{e} = ||\mathbf{e}||^2$ (TODO: expand the calculation)

$$e^2 = 1 + \frac{2h \varepsilon}{\mu^2} \implies \varepsilon = \frac{1}{2} \left( e^2 - 1 \right) \frac{\mu^2}{h^2}$$

$$\tag{3.1.6} \implies \varepsilon = -\frac{1}{2} \frac{\mu (1 - e^2)}{p}$$

From here we can see that the sign of the total energy depends on the eccentricity of the trajectory.

- $0 \leq e < 1$: An elliptical trajectory gives a negative total energy, and hence a *bound* orbit
- $e = 1$: A parabolic trajectory gives a zero total energy, and hence an *unbound* orbit
- $e > 1$: A hyperbolic trajectory gives a positive total energy, and hence an *unbound* orbit

(TODO: add why bound maybe? I mean its sorta apparent Ig? A diagram might help, I'll add that.)

Therefore all bound orbits are ellipses, and all unbound orbits are hyperbolae or parabolae.

For our solar system, the orbits of the planets are bound. The sun is much more massive than any of the planets, hence is nearly at the center of mass, or the focus of the elliptical orbits of all planets, which proves the first law. Of course this isn't exactly true, the orbits influence each other a bit, but its still good enough.
## Second Law

Kepler's second law of planetary motion states that a line segment joining a planet and the sun sweeps out equal areas during equal intervals of time.

The proof of it relies on the fact that the cross product of two vectors gives the area of a parallelogram possessing sides of those vectors. Hence, the triangular area $dA$ swept out in a short period of time is given by half the cross product of the $\mathbf{r}$ and $\mathbf{dr}$ vectors, for some short piece of the orbit, $\mathbf{dr}$.

{{< callout type="image" >}}
{{< svg "images/celmech/secondlaw.svg" "Sweeping out area $dA$" "Sweeping out area dA" >}}
{{% /callout %}}

$$ dA = \frac{1}{2}|\mathbf{r} \times \mathbf{dr}| = \frac{1}{2}|\mathbf{r} \times \mathbf{v} dt| = \frac{h}{2} dt $$

$$\tag{3.1.7} \implies \boxed{\frac{dA}{dt} = \frac{h}{2}} $$

which is constant. Thus, we are done. 

## Third Law

Kepler's third law of planetary motion, states that the square of the period of revolution of a planet is directly proportional to the cube of the semi-major axis of its orbit.

Consider two bodies moving in bound elliptical orbits, with the semi-major axis of the orbit being $a$, and the semi-minor axis being $b$. The lengths of the two axes are related by the eccentricity of the orbit, $e$, as

$$ e^2 = 1 - \frac{b^2}{a^2} $$

The area of an ellipse is $\pi a b = \pi a^2 \sqrt{1 - e^2}$. Moreover, the length of the semi-latus rectum is $p = {b^2}/{a} = a (1 - e^2)$, hence $h = \sqrt{\mu a (1 - e^2)}$ because as we had shown in eqn. ($3.1.5$), $h = \sqrt{\mu p}$.

Integrating the equation of areal velocity, from the previous law we have:

$$
\begin{align*}
dA &= \frac{h}{2} dt\\
\int dA &= \frac{h}{2} \int dt\\
\pi a^2 \sqrt{1 - e^2} &= \frac{1}{2} \sqrt{\mu a (1 - e^2)} P\\
\end{align*}
$$
where $P$ is the time period of revolution.

Rearranging, we get

$$\tag{3.1.8} \boxed{P^2 = \frac{4 \pi^2}{\mu} a^3} $$

where $P$ is the period of one revolution. This is known as Newton's form of the third law. If we work in the units of AU, sidereal years, and solar masses, we have $G M_\odot = 4 \pi^2$. Hence the equation simplifies to

$$\tag{3.1.9} \boxed{a^3 = M P^2} $$

In our solar system, $M = M_\odot + m_{planet} \approx M_\odot = 1$, we get the relation $P^2 = a^3$. This gives us the third and final law!