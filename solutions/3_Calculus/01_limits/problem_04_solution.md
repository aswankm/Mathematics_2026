### Exercise 4. Powers and Oscillation

**Statement:**  
Analyze

$$
\left(\frac{2}{3}\right)^n, \qquad \left(\frac{3}{2}\right)^n, \qquad (-1)^n, \qquad \frac{(-1)^n}{n}.
$$

For each sequence, describe the type of behavior and justify your answer.

> **Why this exercise:** organizes the basic types of sequence behavior and shows that oscillation does not always rule out convergence.

---

### Solution

#### 1. Analysis of Each Sequence

---

##### **Sequence 1:** $a_n = \left(\frac{2}{3}\right)^n$
* **Behavior Type:** **Convergent** (Monotonically decreasing to $0$)
* **Justification:**  
  This is a geometric sequence $r^n$ with base $r = \frac{2}{3}$.  
  Since $|r| = \frac{2}{3} < 1$, as $n \to \infty$, the terms strictly decrease and approach zero:
  
  $$
  \lim_{n \to \infty} \left(\frac{2}{3}\right)^n = 0
  $$

---

##### **Sequence 2:** $b_n = \left(\frac{3}{2}\right)^n$
* **Behavior Type:** **Divergent** (Diverges monotonically to $+\infty$)
* **Justification:**  
  This is a geometric sequence $r^n$ with base $r = \frac{3}{2} > 1$.  
  Since $r > 1$, the terms grow without bound as $n$ increases:
  
  $$
  \lim_{n \to \infty} \left(\frac{3}{2}\right)^n = +\infty
  $$

---

##### **Sequence 3:** $c_n = (-1)^n$
* **Behavior Type:** **Divergent by Oscillation** (Bounded oscillation)
* **Justification:**  
  The terms strictly alternate between two distinct values:
  
  $$
  c_n = 
  \begin{cases} 
  1 & \text{if } n \text{ is even} \\ 
  -1 & \text{if } n \text{ is odd} 
  \end{cases}
  $$
  
  Since the sequence alternates between $1$ and $-1$ without approaching a single unique limit point, $\lim_{n \to \infty} (-1)^n$ **does not exist**.

---

##### **Sequence 4:** $d_n = \frac{(-1)^n}{n}$
* **Behavior Type:** **Convergent** (Damped/oscillatory convergence to $0$)
* **Justification:**  
  The sequence oscillates in sign, but the absolute magnitude of the terms shrinks to zero.  
  Using the **Squeeze Theorem**:
  
  $$
  -\frac{1}{n} \le \frac{(-1)^n}{n} \le \frac{1}{n}
  $$
  
  Since $\lim_{n \to \infty} \left(-\frac{1}{n}\right) = 0$ and $\lim_{n \to \infty} \left(\frac{1}{n}\right) = 0$, the middle sequence must also converge to zero:
  
  $$
  \lim_{n \to \infty} \frac{(-1)^n}{n} = 0
  $$

---

#### 2. Summary Table of Sequence Behaviors

| Sequence | Formula | Limit as $n \to \infty$ | Behavior Classification |
| :--- | :--- | :--- | :--- |
| $a_n$ | $\left(\frac{2}{3}\right)^n$ | $0$ | Convergent (Monotone) |
| $b_n$ | $\left(\frac{3}{2}\right)^n$ | $+\infty$ | Divergent to $+\infty$ |
| $c_n$ | $(-1)^n$ | Does not exist | Divergent (Oscillating, bounded) |
| $d_n$ | $\frac{(-1)^n}{n}$ | $0$ | Convergent (Oscillating / Damped) |
