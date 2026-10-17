1. Compute Transposes A^T and B^T:
   A^T = [ 1  4 ]        B^T = [  1  2  -1 ]
         [ 2  5 ]              [  0   1   3 ]
         [ 3  6 ]

2. Compute Matrix Product AB:
   AB = [ (1)(1)+(2)(2)+(3)(-1)   (1)(0)+(2)(1)+(3)(3) ]
        [ (4)(1)+(5)(2)+(6)(-1)   (4)(0)+(5)(1)+(6)(3) ]

      = [ 1 + 4 - 3   0 + 2 + 9 ]
        [ 4 + 10 - 6  0 + 5 + 18 ]

      = [  2  11 ]
        [  8  23 ]

3. Compute Transpose of Product (AB)^T:
   (AB)^T = [  2   8 ]
            [ 11  23 ]

4. Compute Product of Transposed Factors B^T A^T:
   B^T A^T = [ (1)(1)+(2)(2)+(-1)(3)   (1)(4)+(2)(5)+(-1)(6) ]
             [ (0)(1)+(1)(2)+(3)(3)   (0)(4)+(1)(5)+(3)(6) ]

           = [ 1 + 4 - 3   4 + 10 - 6 ]
             [ 0 + 2 + 9   0 + 5 + 18 ]

           = [  2   8 ]
             [ 11  23 ]

5. Final Verification:
   Since (AB)^T equals B^T A^T (both resulting in [[2, 8], [11, 23]]), the property is verified[cite: 7].
   
