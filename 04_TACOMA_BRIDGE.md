# Tacoma Narrows Bridge Collapse

The 1940 collapse of the Tacoma Narrows Bridge in Washington was a dramatic example of structural failure due to forced resonance.

![Tacoma Bridge Collapse](https://upload.wikimedia.org/wikipedia/commons/8/89/Tacoma_Narrows_Bridge.gif)

### Cause

- Wind caused **aeroelastic flutter**.
- Alternating vortex shedding induced oscillating forces.
- Matched the natural frequency of the bridge: **resonance**.

### Resonance in DEs

Modeled as a forced second-order ODE:

\[
m \frac{d^2x}{dt^2} + c\frac{dx}{dt} + kx = F(t)
\]

Where:
- \( m \): mass, \( c \): damping, \( k \): stiffness
- \( F(t) \): external periodic force

### Related Phenomena

- **Millennium Bridge** in London: swaying due to synchronized walking.
- **Broughton Bridge** (1831): collapsed from marching soldiers.

The Tacoma case taught engineers to consider aerodynamics and dynamic vibrations in bridge design.