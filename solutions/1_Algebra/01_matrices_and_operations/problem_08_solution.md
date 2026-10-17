# Exercise 8. Row Operations and Their Reversibility

### Statement & Solution Overview
For:
```text
A = [  1   2  -1 ]
    [  2   4   1 ]
    [ -1   1   3 ]
1. Initial Matrix:
   A = [  1   2  -1 ]
       [  2   4   1 ]
       [ -1   1   3 ]

2. Step 1 (R2 <- R2 - 2R1):
   - Calculation: R2 - 2R1 = (2, 4, 1) - 2(1, 2, -1) = (2-2, 4-4, 1-(-2)) = (0, 0, 3)
   - Matrix after Step 1:
     [  1   2  -1 ]
     [  0   0   3 ]
     [ -1   1   3 ]
   - Reversing Operation: R2 <- R2 + 2R1

3. Step 2 (R3 <- R3 + R1):
   - Calculation: R3 + R1 = (-1, 1, 3) + (1, 2, -1) = (-1+1, 1+2, 3-1) = (0, 3, 2)
   - Matrix after Step 2:
     [  1   2  -1 ]
     [  0   0   3 ]
     [  0   3   2 ]
   - Reversing Operation: R3 <- R3 - R1

4. Step 3 (Interchange R2 and R3):
   - Matrix after Step 3:
     [  1   2  -1 ]
     [  0   3   2 ]
     [  0   0   3 ]
   - Reversing Operation: Interchange R2 and R3 again
