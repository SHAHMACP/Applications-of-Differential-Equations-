# Satellite Motion

Satellites follow paths governed by Newton's laws and central force systems.

### Newton’s Law of Gravitation

\[
F = -\frac{GMm}{r^2}
\]

Where:
- \( G \): Gravitational constant
- \( M \): Earth mass
- \( m \): Satellite mass

### Central Force Motion

\[
\frac{d^2r}{dt^2} - r\left(\frac{d\theta}{dt}\right)^2 = -\frac{GM}{r^2}, \quad \frac{d}{dt}(r^2 \frac{d\theta}{dt}) = 0
\]

The second equation leads to **Kepler's second law** (equal areas in equal times).

### Orbit Shape

With polar substitution and angular momentum conservation:

\[
r(\theta) = \frac{l}{1 + e \cos \theta}
\]

Where:
- \( l \): Semi-latus rectum
- \( e \): Eccentricity (determines shape: circle, ellipse, parabola, or hyperbola)

### Escape Velocity

Set \( e = 1 \) (parabola) to find escape speed:

\[
v_{\text{escape}} = \sqrt{\frac{2GM}{r}}
\]

### Example

At Earth's surface (r = 3960 mi), with \( g = 9.8 \, m/s^2 \), the orbital period for a circular satellite is approx. 84.4 minutes.