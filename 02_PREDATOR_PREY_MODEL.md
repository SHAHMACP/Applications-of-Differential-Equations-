# Lotka-Volterra Predator-Prey Model

This model captures how two species (predator and prey) interact.

Let:
-  x(t) \: Prey population
-  y(t) \: Predator population

---

In constructing a model of the interaction between two species (prey and predator), we make several assumptions:

1. **Growth of the prey in absence of predator**  
   In the absence of the predator, the prey population grows at a rate proportional to its current population. That is,  
   $\frac{dx}{dt} = x' = ax, a > 0 
   \quad \text{when } y = 0$
   

3. **Decline of the predator in absence of prey**  
   In the absence of prey, the predator population declines (dies out) at a rate proportional to its current size:  
   $\frac{dy}{dt} = y' = -cy, \quad c > 0 \quad \text{when } x = 0$

4. **Interaction between predator and prey**  
   The number of encounters between predator and prey is assumed to be proportional to the product of their populations, $xy$. Each encounter:
   - **Decreases** the growth rate of the prey by a term $-\alpha xy$
   - **Increases** the growth rate of the predator by a term $\gamma xy$  
   where $\alpha, \gamma > 0$ are constants measuring the effect of the interaction.

Combining all of the above, we get the **Lotka-Volterra predator-prey model**:

$$
\frac{dx}{dt} = x' = ax - \alpha xy = x(a - \alpha y)
$$

$$
\frac{dy}{dt} = y' = -cy + \gamma xy = y(-c + \gamma x)
$$

Here:
- $x(t)$: population of the prey at time $t$
- $y(t)$: population of the predator at time $t$
- $a$: natural growth rate of the prey
- $c$: natural death rate of the predator
- $\alpha$: predation rate coefficient (effect of predator on prey)
- $\gamma$: growth rate of predator per prey eaten

Although these are relatively simple equations, they capture the dynamics of a wide class of predator-prey interactions.

---

Here the system has 2 critical points, one is the origin and the other is in the first quadrant.

$$
0 = x' = ax - \alpha xy = x(a - \alpha y) \implies x = 0 \quad \text{or} \quad a - \alpha y = 0
$$

$$
0 = y' = -cy + \gamma xy = y(-c + \gamma x) \implies y = 0 \quad \text{or} \quad -c + \gamma x = 0
$$

Therefore, the critical points are $(0,0)$ and $\left( \frac{c}{\gamma}, \frac{a}{\alpha} \right)$.

The corresponding Jacobian matrix is given by:

$$
J = 
\begin{bmatrix}
a - \alpha y & -\alpha x \\
\gamma y & -c + \gamma x
\end{bmatrix}
$$

At $(0,0)$ the linearized system has coefficient matrix:

$$
A = 
\begin{bmatrix}
a & 0 \\
0 & -c
\end{bmatrix}
$$

The eigenvalues are $a$ and $-c$. Hence, it is an **unstable saddle point**.

We would not care about starting with the population at $(0,0)$, the saddle or negative population. 

The eigenvectors are:

- For eigenvalue $a$: $(1,0)$
- For eigenvalue $-c$: $(0,1)$

Thus, there will be two trajectories entering the equilibrium point vertically (one up and one down) and two leaving horizontally to the right and left.

---
## Stability at the Equilibrium Point

At the equilibrium point:


$\left( \frac{c}{\gamma}, \frac{a}{\alpha} \right)$


the Jacobian matrix is:


$$
J = \begin{bmatrix}
0 & -\alpha c / \gamma \\
\alpha \gamma / \alpha & 0
\end{bmatrix}
$$


Thus, the eigenvalues are purely imaginary:


$$
\pm \sqrt{\alpha c}i
$$

In the linearization, this equilibrium point behaves as a **center**, and the solution near the equilibrium point forms **closed curves**.  
As $t \to \infty$, the trajectories neither approach the equilibrium point nor move away from it.

---

## Nature of the Equilibrium Point

However, this does not tell us whether the equilibrium point in the nonlinear system is a **center** or a **stable/unstable spiral**.

One way to resolve this question is by finding an implicit equation that $x$ and $y$ satisfy.

We find an equation in $x$ and $y$ by dividing the second equation of the system by the first (pretending that $y$ is a function of $x$):


## Solving for Trajectories

The differential equation is:

$$
\frac{dy}{dx} = \frac{y' / x'}{x'} = \frac{y(-c + \gamma x)}{x(a - \alpha y)}
$$

This happens to be separable, so we can solve it:

$$
\frac{a - \alpha y}{y} \, dy = \frac{-c + \gamma x}{x} \, dx
$$

The solution is:

$$
a \ln|y| - \alpha y = -c \ln|x| + \gamma x + k
$$

Thus (at least for $x > 0$ and $y > 0$, which is the region we are interested in), the trajectories are **level curves** of the function:

$$
h(x, y) = a \ln y + c \ln x - \alpha y - \gamma x
$$


Thus, we should have a **center**, not a spiral, at the equilibrium point:

$$
\left( \frac{c}{\gamma}, \frac{a}{\alpha} \right)
$$


The **isoclines**:

- For $x' = 0$ are $x = 0$ and $y = \frac{a}{\alpha}$ (since $x = 0$ is a vertical line, there are trajectories in it — the two trajectories that enter the equilibrium point $(0,0)$).

- The isoclines for $y' = 0$ are $y = 0$ and $x = \frac{c}{\gamma}$ (again, there are trajectories in the $x$-axis — the two that leave the $(0,0)$ point).

---
