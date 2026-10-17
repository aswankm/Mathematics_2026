# Exercise 13. A Recurrence Written in Matrix Form

### Statement & Solution Overview
Let:
```text
F = [ 1   1 ]
    [ 1   0 ]
1. Compute Successive Powers (F^2, F^3, F^4, F^5):
   - F^2 = [ 1   1 ] [ 1   1 ] = [ (1)(1)+(1)(1)   (1)(1)+(1)(0) ] = [ 2   1 ]
           [ 1   0 ] [ 1   0 ]   [ (1)(1)+(0)(1)   (1)(1)+(0)(0) ]   [ 1   1 ]

   - F^3 = F^2 F = [ 2   1 ] [ 1   1 ] = [ (2)(1)+(1)(1)   (2)(1)+(1)(0) ] = [ 3   2 ]
                   [ 1   1 ] [ 1   0 ]   [ (1)(1)+(1)(1)   (1)(1)+(1)(0) ]   [ 2   1 ]

   - F^4 = F^3 F = [ 3   2 ] [ 1   1 ] = [ (3)(1)+(2)(1)   (3)(1)+(2)(0) ] = [ 5   3 ]
                   [ 2   1 ] [ 1   0 ]   [ (2)(1)+(1)(1)   (2)(1)+(1)(0) ]   [ 3   2 ]

   - F^5 = F^4 F = [ 5   3 ] [ 1   1 ] = [ (5)(1)+(3)(1)   (5)(1)+(3)(0) ] = [ 8   5 ]
                   [ 3   2 ] [ 1   0 ]   [ (3)(1)+(2)(1)   (3)(1)+(2)(0) ]   [ 5   3 ]

2. Compare with the Sequence (0, 1, 1, 2, 3, 5, 8, ...):
   - The entries of the matrices F^n are consecutive Fibonacci numbers. Specifically, F^n contains 
     F_(n+1), F_n, F_n, and F_(n-1) respectively.

3. Compute Product F * [a, b]^T:
   - F [ a ] = [ 1   1 ] [ a ] = [ (1)(a) + (1)(b) ] = [ a + b ]
       [ b ]   [ 1   0 ] [ b ]   [ (1)(a) + (0)(b) ]   [   a   ]

4. Explanation of the Recurrence Step:
   - Multiplying the vector by F creates the sum of two consecutive terms (a + b) for the new top entry, 
     and passes the current term (a) down as the next bottom entry, effectively advancing the sequence by one step.
