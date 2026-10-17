# Exercise 15. Associativity of Multiplication and Different Calculation Paths

### Statement & Solution Overview
Given:
```text
A = [ 1  2  0 ]     B = [  1  0 ]     C = [ 2   1 ]
    [ 0  1  1 ]         [  2  1 ]         [ 0  -1 ]
                        [ -1  3 ]
1. Compute (AB)C (Grouping AB first):
   - Step A (Compute AB):
     AB = [ 1  2  0 ] [  1  0 ] = [ (1)(1)+(2)(2)+(0)(-1)   (1)(0)+(2)(1)+(0)(3) ] = [ 5   2 ]
          [ 0  1  1 ] [  2  1 ]   [ (0)(1)+(1)(2)+(1)(-1)   (0)(0)+(1)(1)+(1)(3) ]   [ 1   4 ]
                      [ -1  3 ]

   - Step B (Compute (AB)C):
     (AB)C = [ 5   2 ] [ 2   1 ] = [ (5)(2)+(2)(0)   (5)(1)+(2)(-1) ] = [ 10   3 ]
             [ 1   4 ] [ 0  -1 ]   [ (1)(2)+(4)(0)   (1)(1)+(4)(-1) ]   [  2  -3 ]

2. Compute A(BC) (Grouping BC first):
   - Step A (Compute BC):
     BC = [  1  0 ] [ 2   1 ] = [ (1)(2)+(0)(0)   (1)(1)+(0)(-1) ] = [  2   1 ]
          [  2  1 ] [ 0  -1 ]   [ (2)(2)+(1)(0)   (2)(1)+(1)(-1) ]   [  4   1 ]
          [ -1  3 ]             [ (-1)(2)+(3)(0)  (-1)(1)+(3)(-1)]   [ -2  -4 ]

   - Step B (Compute A(BC)):
     A(BC) = [ 1  2  0 ] [  2   1 ] = [ (1)(2)+(2)(4)+(0)(-2)   (1)(1)+(2)(1)+(0)(-4) ] = [ 10   3 ]
             [ 0  1  1 ] [  4   1 ]   [ (0)(2)+(1)(4)+(1)(-2)   (0)(1)+(1)(1)+(1)(-4) ]   [  2  -3 ]
                         [ -2  -4 ]

3. Comparison and Explanation:
   - Results: Both calculation paths yield the exact same matrix: [[10, 3], [2, -3]][cite: 14].
   - Associativity Meaning: This demonstrates that matrix multiplication is associative—changing how 
     the matrices are grouped into pairs does not change the final product[cite: 14]. However, the choice 
     of grouping path can change the number of scalar multiplications required depending on matrix dimensions.
