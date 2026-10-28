## Problem 7. Exponential Growth

Assume the model 

$$N(t) = N_0 e^{kt}, \quad k > 0$$[cite: 3].

1. Verify by differentiation that the model satisfies the relation $N'(t) = kN(t)$[cite: 3].
2. Find the population doubling time[cite: 3].
3. Explain why the doubling time does not depend on $N_0$[cite: 3].

> Why this problem: it shows the connection between the exponential function and a growth rate proportional to the current value, without introducing a separate technique for solving differential equations[cite: 3].

---

### Solution

#### 1. Verification by Differentiation
To find the derivative $N'(t)$, we differentiate $N(t) = N_0 e^{kt}$ with respect to time $t$ using the chain rule:

$$N'(t) = \frac{d}{dt} \left( N_0 e^{kt} \right) = N_0 \cdot k \cdot e^{kt} = k \left( N_0 e^{kt} \right)$$

Since $N(t) = N_0 e^{kt}$, this can be rewritten as:

$$N'(t) = kN(t)$$

Thus, the differential model is satisfied[cite: 3].

---

#### 2. Population Doubling Time
The doubling time $t_d$ is the time it takes for the population to reach twice its initial size, meaning $N(t_d) = 2N_0$.

Substitute this into the exponential model:
$$2N_0 = N_0 e^{kt_d}$$

Divide both sides by $N_0$ (assuming $N_0 > 0$):
$$2 = e^{kt_d}$$

Take the natural logarithm of both sides:
$$\ln(2) = kt_d$$

Solve for the doubling time $t_d$:
$$t_d = \frac{\ln(2)}{k}$$

---

#### 3. Why Doubling Time Does Not Depend on $N_0$
From the derivation in step 2, the initial population term $N_0$ canceled out when dividing both sides of the equation by $N_0$. Consequently, the formula for the doubling time $t_d = \frac{\ln(2)}{k}$ depends exclusively on the growth rate constant $k$[cite: 3]. This means that a population grows by a factor of 2 in the exact same amount of time regardless of whether it starts with 10 individuals or 10,000 individuals[cite: 3].
