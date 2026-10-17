# Exercise 10. Columns of a Matrix Product

### Statement & Solution Overview
Given:
```text
A = [ 1   2   0 ]       B = [  1   2 ]
    [ 0   1   1 ]           [ -1   0 ]
                            [  3   1 ]
1. Identify Column Vectors of B:
   b_1 = [  1 ]      b_2 = [ 2 ]
         [ -1 ]            [ 0 ]
         [  3 ]            [ 1 ]

2. Compute Ab_1:
   Ab_1 = [ 1   2   0 ] [  1 ] = [ (1)(1) + (2)(-1) + (0)(3) ] = [ 1 - 2 + 0 ] = [ -1 ]
          [ 0   1   1 ] [ -1 ]   [ (0)(1) + (1)(-1) + (1)(3) ]   [ 0 - 1 + 3 ]   [  2 ]
                            [  3 ]

3. Compute Ab_2:
   Ab_2 = [ 1   2   0 ] [ 2 ] = [ (1)(2) + (2)(0) + (0)(1) ] = [ 2 + 0 + 0 ] = [ 2 ]
          [ 0   1   1 ] [ 0 ]   [ (0)(2) + (1)(0) + (1)(1) ]   [ 0 + 0 + 1 ]   [ 1 ]
                            [ 1 ]

4. Compute Matrix AB:
   AB = [ 1   2   0 ] [  1   2 ] = [ (1)(1)+(2)(-1)+(0)(3)   (1)(2)+(2)(0)+(0)(1) ] = [ -1   2 ]
        [ 0   1   1 ] [ -1   0 ]   [ (0)(1)+(1)(-1)+(1)(3)   (0)(2)+(1)(0)+(1)(1) ]   [  2   1 ]
                      [  3   1 ]

5. Comparison and Explanation:
   - The first column of AB is [-1, 2]^T, which matches Ab_1.
   - The second column of AB is [2, 1]^T, which matches Ab_2.
   - Therefore, the columns of the product matrix AB are precisely the matrix-vector products of A with each column of B: AB = [Ab_1  Ab_2].
