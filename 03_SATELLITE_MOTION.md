# 🛰️ Satellite Motion

In **astrodynamics**, an orbit equation defines the path of an orbiting body $m_2$ around a central body $m_1$ (relative to $m_1$), without specifying position as a function of time, under standard assumptions.

A body moving under the influence of a force directed toward a central body — with a magnitude **inversely proportional to the square of the distance** between them (e.g., gravity) — follows an **orbit** that is a **conic section**:  
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
![image](https://github.com/user-attachments/assets/78d11813-9602-424f-a566-e0a05d8dac64)

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

![image](https://github.com/user-attachments/assets/aab8ffe4-be06-479b-9ca2-7b8b234d8232)  Force F is acting towards (or away from) a fixed point O- central force system.


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


