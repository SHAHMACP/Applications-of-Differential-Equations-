# Lotka-Volterra Predator-Prey Model

This model captures how two species (predator and prey) interact.

Let:
-  x(t) \: Prey population
-  y(t) \: Predator population

---

In constructing a model of the interaction between two species (prey and predator), we make several assumptions:

1. **Growth of the prey in absence of predator**  
   In the absence of the predator, the prey population grows at a rate proportional to its current population. That is,  
   $$
   \frac{dx}{dt} = x' = ax, $$\quad a > 0 $$
   $\quad \text{when } y = 0
   $

3. **Decline of the predator in absence of prey**  
   In the absence of prey, the predator population declines (dies out) at a rate proportional to its current size:  
   $$
   \frac{dy}{dt} = y' = -cy, \quad c > 0 \quad \text{when } x = 0
   $$

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
