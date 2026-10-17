# Exercise 12. Formula for a Matrix Power

### Statement & Solution Overview
Let:
```text
A = [ 1   1 ]
    [ 0   1 ]
1. Compute Successive Powers (A^2, A^3, A^4):
   - A^2 = [ 1   1 ] [ 1   1 ] = [ (1)(1)+(1)(0)   (1)(1)+(1)(1) ] = [ 1   2 ]
           [ 0   1 ] [ 0   1 ]   [ (0)(1)+(1)(0)   (0)(1)+(1)(1) ]   [ 0   1 ]

   - A^3 = A^2 A = [ 1   2 ] [ 1   1 ] = [ (1)(1)+(2)(0)   (1)(1)+(2)(1) ] = [ 1   3 ]
                   [ 0   1 ] [ 0   1 ]   [ (0)(1)+(1)(0)   (0)(1)+(1)(1) ]   [ 0   1 ]

   - A^4 = A^3 A = [ 1   3 ] [ 1   1 ] = [ (1)(1)+(3)(0)   (1)(1)+(3)(1) ] = [ 1   4 ]
                   [ 0   1 ] [ 0   1 ]   [ (0)(1)+(1)(0)   (0)(1)+(1)(1) ]   [ 0   1 ]

2. Formulate Conjecture for A^n:
   - Observing the top-right entry growing sequentially with the exponent:
     A^n = [ 1   n ]
           [ 0   1 ]

3. Inductive Step (Multiply by A to show n+1):
   - Assume A^n holds. Now compute A^(n+1) = (A^n)A:
     A^(n+1) = [ 1   n ] [ 1   1 ] = [ (1)(1)+(n)(0)   (1)(1)+(n)(1) ] = [ 1   n+1 ]
               [ 0   1 ] [ 0   1 ]   [ (0)(1)+(1)(0)   (0)(1)+(1)(1) ]   [ 0    1  ]
   - Explanation: Multiplying the general power matrix by A adds 1 to the top-right component, perfectly yielding the formula for n + 1.
