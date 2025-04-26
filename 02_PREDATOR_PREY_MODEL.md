# Lotka-Volterra Predator-Prey Model

This model captures how two species (predator and prey) interact.

Let:
- \( x(t) \): Prey population
- \( y(t) \): Predator population

### Equations

\[
\frac{dx}{dt} = ax - bxy \\
\frac{dy}{dt} = -cy + dxy
\]

Where:
- \( a \): Prey birth rate
- \( b \): Predation rate
- \( c \): Predator death rate
- \( d \): Predator growth from consumption

### Equilibrium Points

Set dx/dt = 0 and dy/dt = 0:
- (0, 0): Trivial equilibrium (saddle)
- \( (\frac{c}{d}, \frac{a}{b}) \): Center

### Jacobian

\[
J = \begin{bmatrix}
a - by & -bx \\
dy & -c + dx
\end{bmatrix}
\]

At each equilibrium, we compute the eigenvalues to determine stability.

### Phase Portrait

The system forms closed orbits near the center equilibrium, indicating periodic behavior.

### Example

\[
\frac{dx}{dt} = x(1 - y), \quad \frac{dy}{dt} = y(-1 + x)
\]

This system stabilizes around an equilibrium and shows predator-prey cycles. Predator peaks lag behind prey peaks.