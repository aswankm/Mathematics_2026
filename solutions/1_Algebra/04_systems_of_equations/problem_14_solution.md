## Exercise 14. A Small Change in the Right-Hand Side

### Statement
Compare the systems

$$
\begin{cases}
x + y = 2, \\
2x - y = 1, \\
3x = 3
\end{cases}
\quad \text{and} \quad
\begin{cases}
x + y = 2, \\
2x - y = 1, \\
3x = 3.1
\end{cases}
$$

Check the consistency of each system and explain why a small change in one number can change the type of the system.

### Solution

#### 1. System 1 Analysis
* From Equation 3: $3x = 3 \implies x = 1$.
* From Equation 1: $1 + y = 2 \implies y = 1$.
* Checking in Equation 2: $2(1) - 1 = 1$ (Valid).

**Result:** **Consistent** (Unique solution: $(x, y) = (1, 1)$).

#### 2. System 2 Analysis
* Adding Equations 1 and 2 yields $3x = 3 \implies x = 1, y = 1$.
* Equation 3 requires $3x = 3.1 \implies 3(1) = 3.1$, which gives the contradiction $3 = 3.1$.

**Result:** **Inconsistent** (No solution).

#### 3. Explanation
This is an **overdetermined system** (3 equations, 2 unknowns). The first two equations uniquely fix the single intersection point $(1, 1)$. The third equation is only satisfied if its line passes through that exact point. Changing $3$ to $3.1$ shifts the third line, destroying the common point of intersection and making the system inconsistent.
