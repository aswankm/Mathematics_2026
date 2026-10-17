# Exercise 11. When Do Matrices Commute?

### Statement & Solution Overview
Given:
```text
A = [ 1   1 ]       B = [ a   b ]
    [ 0   1 ]           [ c   d ]
1. Compute Product AB:
   AB = [ 1   1 ] [ a   b ] = [ (1)(a)+(1)(c)   (1)(b)+(1)(d) ] = [ a+c   b+d ]
        [ 0   1 ] [ c   d ]   [ (0)(a)+(1)(c)   (0)(b)+(1)(d) ]   [  c     d  ]

2. Compute Product BA:
   BA = [ a   b ] [ 1   1 ] = [ (a)(1)+(b)(0)   (a)(1)+(b)(1) ] = [ a   a+b ]
        [ c   d ] [ 0   1 ]   [ (c)(1)+(d)(0)   (c)(1)+(d)(1) ]   [ c   c+d ]

3. Equate Entries (AB = BA):
   - Top-left:     a + c = a  ==>  c = 0
   - Top-right:    b + d = a + b  ==>  d = a
   - Bottom-left:  c = c  (always true since c = 0)
   - Bottom-right: d = c + d  ==>  c = 0 (consistent with c = 0)

4. Conditions and General Form:
   - Conditions: c = 0 and a = d.
   - General Form of B: Substituting these conditions yields:
     B = [ a   b ]
         [ 0   a ]
