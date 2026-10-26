### Exercise 5. The Classical Limit Leading to the Number e

**Statement:**  
Compute

$$
\lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n.
$$

Calculate several values for increasing $n$ and compare the observed behavior with the value of the limit. Explain why a few values do not constitute a proof.

> **Why this exercise:** connects a central limit with intuition based on concrete terms of a sequence.

---

### Solution

#### 1. Numerical Calculation for Increasing $n$
Let us compute the value of the expression $a_n = \left(1 + \frac{1}{n}\right)^n$ for progressively larger values of $n$:

* For $n = 1$:  

$$
  \left(1 + \frac{1}{1}\right)^1 = 2^1 = 2
$$

* For $n = 10$:  

$$
  \left(1 + \frac{1}{10}\right)^{10} = (1.1)^{10} \approx 2.59374
$$

* For $n = 100$:  

$$
  \left(1 + \frac{1}{100}\right)^{100} = (1.01)^{100} \approx 2.70481
$$

* For $n = 1,000$:  

$$
  \left(1 + \frac{1}{1000}\right)^{1000} = (1.001)^{1000} \approx 2.71692
$$

* For $n = 10,000$:  

$$
  \left(1 + \frac{1}{10000}\right)^{10000} = (1.0001)^{10000} \approx 2.71815
$$

---

#### 2. Comparison with the Limit
As $n$ increases toward infinity, the terms of the sequence grow closer and closer to Euler's number:

$$
\lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n = e \approx 2.718281828...
$$

The numerical calculations demonstrate a clear stabilization trend converging toward the constant $e$.

---

#### 3. Why a Few Values Do Not Constitute a Proof
* **Finite vs. Infinite:** Calculating a finite number of discrete values only provides empirical evidence or an approximation for specific test points. It does not account for the infinite behavior of $n$ as $n \to \infty$.
* **Misleading Trends:** In mathematics, sequences can exhibit deceptive behaviors where terms grow very slowly or plateau for large initial values before shifting behavior. 
* **Requirement for Proof:** A rigorous mathematical proof requires analytical techniques (such as bounds via the Binomial Theorem, monotonic convergence, and the sandwich theorem or continuity of exponential/logarithmic functions) to guarantee that the limit exists and equals $e$ for all arbitrarily large $n$.
