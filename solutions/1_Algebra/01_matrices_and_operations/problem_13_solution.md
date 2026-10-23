# Exercise 13. A Recurrence Written in Matrix Form

### Statement & Solution Overview

Let:

$$
F = \begin{bmatrix} 1 & 1 \\ 1 & 0 \end{bmatrix}
$$

---

### 1. Compute Successive Powers ($F^2, F^3, F^4, F^5$)

- **$F^2$:**

$$
  F^2 = \begin{bmatrix} 1 & 1 \\ 1 & 0 \end{bmatrix} \begin{bmatrix} 1 & 1 \\ 1 & 0 \end{bmatrix} = \begin{bmatrix} (1)(1) + (1)(1) & (1)(1) + (1)(0) \\ (1)(1) + (0)(1) & (1)(1) + (0)(0) \end{bmatrix} = \begin{bmatrix} 2 & 1 \\ 1 & 1 \end{bmatrix}
$$

- **$F^3$ ($F^2 F$):**

$$
  F^3 = \begin{bmatrix} 2 & 1 \\ 1 & 1 \end{bmatrix} \begin{bmatrix} 1 & 1 \\ 1 & 0 \end{bmatrix} = \begin{bmatrix} (2)(1) + (1)(1) & (2)(1) + (1)(0) \\ (1)(1) + (1)(1) & (1)(1) + (1)(0) \end{bmatrix} = \begin{bmatrix} 3 & 2 \\ 2 & 1 \end{bmatrix}
$$

- **$F^4$ ($F^3 F$):**

$$
  F^4 = \begin{bmatrix} 3 & 2 \\ 2 & 1 \end{bmatrix} \begin{bmatrix} 1 & 1 \\ 1 & 0 \end{bmatrix} = \begin{bmatrix} (3)(1) + (2)(1) & (3)(1) + (2)(0) \\ (2)(1) + (1)(1) & (2)(1) + (1)(0) \end{bmatrix} = \begin{bmatrix} 5 & 3 \\ 3 & 2 \end{bmatrix}
  $$

- **$F^5$ ($F^4 F$):**

$$
  F^5 = \begin{bmatrix} 5 & 3 \\ 3 & 2 \end{bmatrix} \begin{bmatrix} 1 & 1 \\ 1 & 0 \end{bmatrix} = \begin{bmatrix} (5)(1) + (3)(1) & (5)(1) + (3)(0) \\ (3)(1) + (2)(1) & (3)(1) + (2)(0) \end{bmatrix} = \begin{bmatrix} 8 & 5 \\ 5 & 3 \end{bmatrix}
$$

---

### 2. Compare with the Sequence ($0, 1, 1, 2, 3, 5, 8, \dots$)

- The entries of the matrices $F^n$ correspond to consecutive Fibonacci numbers. Specifically, $F^n$ contains:

$$
  F^n = \begin{bmatrix} F_{n+1} & F_n \\ F_n & F_{n-1} \end{bmatrix}
$$

---

### 3. Compute Product $F \begin{bmatrix} a \\ b \end{bmatrix}$


$$
F \begin{bmatrix} a \\ b \end{bmatrix} = \begin{bmatrix} 1 & 1 \\ 1 & 0 \end{bmatrix} \begin{bmatrix} a \\ b \end{bmatrix} = \begin{bmatrix} (1)(a) + (1)(b) \\ (1)(a) + (0)(b) \end{bmatrix} = \begin{bmatrix} a + b \\ a \end{bmatrix}
$$

---

### 4. Explanation of the Recurrence Step

- Multiplying the sequence vector by $F$ generates the sum of two consecutive terms ($a + b$) for the new top entry, and passes the current term ($a$) down as the new bottom entry, effectively advancing the Fibonacci recurrence relation by one step.
