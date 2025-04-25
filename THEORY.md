# Study on Applications of Differential Equations

This document explores the practical use of differential equations in real-world systems through three major applications:
- Lotka-Volterra Predator-Prey System
- Satellite Motion
- Tacoma Narrows Bridge Collapse

---

## Introduction

Differential equations describe systems where change occurs continuously. They are used in physics, engineering, biology, economics, and more. This project outlines definitions, classifications (ODEs, PDEs), and general forms such as linear, nonlinear, order, degree, and solution types (general, particular, singular).

---

## 1. Lotka-Volterra Predator-Prey Model

This classical ecological model shows how predator and prey populations interact using a nonlinear first-order differential system. It assumes exponential growth for prey and predator death in absence of prey, with interaction terms modeling encounters.

Equations:
- dx/dt = ax - bxy
- dy/dt = -cy + dxy

Equilibrium and phase portraits show the dynamics. Jacobian matrix and eigenvalues at critical points help determine local stability and behavior (center, saddle).

---

## 2. Satellite Motion

Using Newton's laws, satellite paths are modeled as conic sections (ellipses, parabolas, hyperbolas) using polar coordinates. Central force systems yield equations based on gravitational pull:

- F = -GMm/r^2
- r(θ) = l / (1 + e cosθ)

Kepler’s laws are derived from Newton’s laws. Equations help calculate orbit radius, velocity, escape speed, and orbital time. Applications include space engineering and astrophysics.

---

## 3. Tacoma Narrows Bridge Collapse

The 1940 collapse of the Tacoma Narrows Bridge is modeled with forced vibrations and resonance phenomena. A differential equation involving periodic forcing explains oscillations caused by vortex shedding (aeroelastic instability).

Key concepts:
- Vortex street
- Forced vibration
- Mechanical resonance
- Eigenfunctions of oscillating structures

Differential equations describe how natural frequencies and external forces interact, leading to structural failure if not properly damped.

---

## Visual Concepts Explained

- **Jacobian Matrix**: Used to analyze the stability of equilibria in nonlinear systems.
- **Isoclines**: Curves where the slope of the direction field is constant.
- **Phase Plane & Portrait**: Visual tools showing system trajectories based on initial conditions.
- **Types of Equilibria**: Node, Saddle, Spiral, Center, etc.

---

## References

- Elementary Differential Equations by Boyce and DiPrima
- Mathematics Stack Exchange
- Scholarpedia.org – Equilibrium
- Differential Equations and Their Applications by Martin Braun