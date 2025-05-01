# 🛰️ Satellite Motion

In **astrodynamics**, an orbit equation defines the path of an orbiting body $m_2$ around a central body $m_1$ (relative to $m_1$), without specifying position as a function of time, under standard assumptions.

A body moving under the influence of a force directed toward a central body, with a magnitude **inversely proportional to the square of the distance** between them (e.g., gravity) — follows an **orbit** that is a **conic section**:  
- Circular  
- Elliptical  
- Parabolic  
- Hyperbolic  
- Radial  

The central body is located at **one of the foci** of the orbit.

---

## 🌍 Gravity and Satellite Motion

In space, **gravity supplies the centripetal force** that causes satellites (like the Moon) to orbit larger bodies (like the Earth). Thanks to **differential equations**, if you know the **mass** and **altitude** of a satellite in orbit around Earth, you can compute how fast it needs to travel to maintain that orbit.

The **motion of orbits is governed by Newton’s laws**.  
The same laws that govern motion on Earth also extend to the heavens, controlling the movement of **planets, moons, and artificial satellites**.

---

## 🔁 Geosynchronous Orbits

When a satellite travels in a **geosynchronous orbit** around Earth, it must travel at a specific **orbital radius** and **orbital period** to maintain synchronization.

Because **radius** and **period** are related, you can use equations to calculate one if you know the other.

- The **orbital period** is the time it takes to make one full revolution around the object.  
  For example, the Earth's orbital period around the Sun is one year.

- If you know the satellite’s **orbital speed** and **radius**, you can calculate its period using orbital mechanics equations.

---

## 📘 What This Section Covers

This section introduces:
- The **central force system**
- **Newton’s law of gravitation**
- **Kepler’s laws of planetary motion**

We will also **derive mathematical equations** to describe satellite motion and describe the **shape of orbits** using these equations.

---

## 🌌 Central Force System, Newton's Law of Gravitation, and Kepler’s Laws of Planetary Motion
![image](https://github.com/user-attachments/assets/78d11813-9602-424f-a566-e0a05d8dac64) A fore F is acting on particle of mass m

In the Figure, the particle of mass $m$ has **position vector** $\mathbf{R}$ and is acted upon by a force $\mathbf{F}$.  
By **Newton’s Second Law**, we have:

$$
\mathbf{F} = m\mathbf{A} = m \frac{d\mathbf{V}}{dt} = \frac{d}{dt}(m\mathbf{V})
$$

where $\mathbf{V}$ and $\mathbf{A}$ denote the **velocity** and **acceleration** of the particle at time $t$.

Hence, taking the **vector cross product** with position vector $\mathbf{R}$:

$$
\mathbf{R} \times \mathbf{F} = \mathbf{R} \times \frac{d}{dt}(m\mathbf{V})
$$

We now consider the case where the force F always acts towards (or away from) the origin O (Fig. 2). A force system of this type is called a central force system. Since R×F=0, 

$$\mathbf{R} \times \frac{d}{dt}(m\mathbf{V})=0$$

![image](https://github.com/user-attachments/assets/aab8ffe4-be06-479b-9ca2-7b8b234d8232)  
Force F is acting towards (or away from) a fixed point O in- central force system.


From Eq. (1), and hence  

$$
\mathbf{R} \times m\mathbf{V} = \text{constant} = m\mathbf{H}
$$


The vector 
$\ m\mathbf{V}\ $
is the linear momentum of the particle, and the vector 
$\ m\mathbf{H} \$ 
is the angular momentum of the particle about the origin. If 
$\ \mathbf{H} = 0 \$
, then 
$\ \mathbf{R} \$ 
and 
$\ \mathbf{V} \$ 
are parallel and the path of the particle passes through the origin. Otherwise, since 
$\ \mathbf{R} \$
and 
$\ \mathbf{V} \$
are perpendicular to 
$\ \mathbf{H} \$
, the path or the orbit of the particle lies in a plane perpendicular to 
$\mathbf{H} \$.

We now find the velocity 
$\ \mathbf{V} \$ 
and acceleration 
$\ \mathbf{A} \$ 
in polar coordinates. We write the position vector 
$\ \mathbf{R} = r\mathbf{L} \$
, where  

$$
\mathbf{L} = \cos\theta \, \mathbf{i} + \sin\theta \, \mathbf{j}
$$ 

is the radial unit vector. Then  

$$
\frac{d\mathbf{L}}{d\theta} = (-\sin\theta) \, \mathbf{i} + \cos\theta \, \mathbf{j} = \mathbf{M}
$$  
 
 is the transverse unit vector (see Fig. 3).
 
![image](https://github.com/user-attachments/assets/887edac7-f4d6-4740-9bbb-d86ff752544a)  Radial and transverse unit vectors. 



The velocity is given by:

```math
\mathbf{V} = \frac{d\mathbf{R}}{dt} = \frac{dr}{dt} \mathbf{L} + r \frac{d\mathbf{L}}{dt} = \frac{dr}{dt} \mathbf{L} + r \frac{d\theta}{dt} \frac{d\mathbf{L}}{d\theta}
```

Since  
```math
\frac{d\mathbf{L}}{d\theta} = \mathbf{M},
```  
we get:


$$
\mathbf{V} = \frac{dr}{dt} \mathbf{L} + r \frac{d\theta}{dt} \mathbf{M}
$$


The scalar 
$\ \frac{dr}{dt} \$ 
is the radial component of 
$\ \mathbf{V} \$
, and the scalar 
$\ r \left(\frac{d\theta}{dt}\right) \$
is the transverse component.

---

Differentiating the above equation, we get the acceleration 
$\mathbf{A}$ 
:

```math
\mathbf{A} = \frac{d\mathbf{V}}{dt} = \frac{dr}{dt} \frac{d\mathbf{L}}{dt} + \frac{d^2 r}{dt^2} \mathbf{L} + \left( r \frac{d\theta}{dt} \right) \frac{d\mathbf{M}}{dt} + \left( r \frac{d^2 \theta}{dt^2} + \frac{dr}{dt} \frac{d\theta}{dt} \right) \mathbf{M}
```

Since

```math
\frac{d\mathbf{L}}{dt} = \frac{d\mathbf{L}}{d\theta} \frac{d\theta}{dt} = \frac{d\theta}{dt} \mathbf{M}, \quad
\frac{d\mathbf{M}}{dt} = \frac{d\mathbf{M}}{d\theta} \frac{d\theta}{dt} = \frac{d\theta}{dt} (-\mathbf{L})
```

Substituting back, we obtain:

```math
\mathbf{A} = \left[ \frac{d^2 r}{dt^2} - r \left( \frac{d\theta}{dt} \right)^2 \right] \mathbf{L} + \left[ r \frac{d^2 \theta}{dt^2} + 2 \frac{dr}{dt} \frac{d\theta}{dt} \right] \mathbf{M} 
```

In Eq. (3), the scalar coefficient of L is the radial component and the scalar coefficient of M is the transverse component of acceleration A.
(If we take the Cartesian coordinates instead of polar coordinates, we have tangential and normal components of velocity and acceleration.)




Let **f** be the magnitude of the force **F** acting on a particle, and let this force act toward the center **O**. Then,

$$
\vec{F} = -f \cdot \vec{L + O(M)}
$$

According to **Newton’s Second Law**, applying the force in radial and transverse directions, we obtain the following equations:

Radial direction:

$$
\frac{d^2 r}{dt^2} - r \left( \frac{d\theta}{dt} \right)^2 = -\frac{f}{m} 
$$

Transverse direction:

$$
r \frac{d^2 \theta}{dt^2} + 2 \frac{dr}{dt} \frac{d\theta}{dt} = 0
$$

Now, the core problem is to solve the system of differential equations (4) and (5), which involve two unknown functions 
$\ r = \phi(t) \$
and 

$\theta = \varphi(t)\$

. These functions together give the **parametric equations** of the orbit of the moving particle.

Another key goal is to express  **r** in terms of 
$\theta\$
, i.e., to find a **polar equation** of the form:

$$
r = \beta(\theta)
$$

To do so, we require:

- Initial conditions
- The form of **f** in Equation (4)

We begin with Equation (5), which notably does **not** include **f**, and derive an important result:

Since 
$r \neq 0 \$
, Equation (5) can be rearranged as:

$$
\frac{1}{r} \frac{d}{dt} \left( r^2 \frac{d\theta}{dt} \right) = 0 
$$



From Equation (6), we deduce:

$$
r^2 \frac{d\theta}{dt} = \text{constant} = h 
$$

This constant  h is related to the **conservation of angular momentum**. It implies that the **areal velocity** is constant.

### Area Swept in Polar Coordinates

Using the formula for the area in polar coordinates, we observe (as in Fig. 4) that the **shaded area** swept out by the particle moving from 
$\ (r_1, \theta_1) \$
at time 
$\t_1 $ 
to 
$\(r, \theta) \$
at time t is given by:

$$
A = \frac{1}{2} \int_{\theta_1}^{\theta} [\beta(u)]^2 \, du
$$

![image](https://github.com/user-attachments/assets/78f7c4d7-0746-49a4-9027-5d2d6f06daf2) area swept out by the radius vector..

![image](https://github.com/user-attachments/assets/243d6057-69f6-4384-b714-4930b1e409c9)



This areal velocity being constant implies that the area swept out is the same for any equal interval of time, i.e., for any duration 
$\ t_2 - t_1 \$
, the area swept by the radius vector remains the same. This leads to the classical result known as the **Law of Areas**.

---

### **Theorem: Law of Areas**

*For a particle moving under a central force, the radius vector drawn from the center of force to the particle sweeps out equal areas in equal intervals of time.*

---

Now, let us **apply this to the planetary motion**, i.e., the motion of a planet around the sun. Consider the system governed by equations:

 Radial direction:
  $$
  \frac{d^2 r}{dt^2} - r \left( \frac{d\theta}{dt} \right)^2 = -\frac{f}{m} 
  $$

 Transverse (angular) direction:

  $$
  r \frac{d^2 \theta}{dt^2} + 2 \frac{dr}{dt} \frac{d\theta}{dt} = 0
  $$


According to **Newton's Law of Universal Gravitation**, the gravitational force between two particles (like the Sun and a planet) is:

$$
f = \frac{GMm}{r^2}
$$

Where:
-  G  is the universal gravitational constant,
- M  is the mass of the Sun,
-  m  is the mass of the planet,
- r is the distance between the planet and the Sun.

Thus, substituting this into Eq. (4), the radial equation becomes:

$$
\frac{d^2 r}{dt^2} - r \left( \frac{d\theta}{dt} \right)^2 = -\frac{GM}{r^2}
$$

(Note:  m  cancels out, which shows that orbital motion does not depend on the mass of the planet.)


This integral provides the total area swept by the radius vector, where 
$\ \beta(\theta) \$ 
is the **polar equation** of the orbit (i.e., 
$\ r = \beta(\theta) \$
.

