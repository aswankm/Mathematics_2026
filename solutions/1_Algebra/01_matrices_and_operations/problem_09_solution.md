# Exercise 9. Composing Transformations

### Statement & Solution Overview
Let:
```text
S = [ 2   0 ]       R = [  0  -1 ]       x = [ 1 ]
    [ 0   1 ]           [  1   0 ]           [ 2 ]
1. Compute RSx (Scale first, then rotate):
   - Step A (Sx):
     Sx = [ 2   0 ] [ 1 ] = [ (2)(1) + (0)(2) ] = [ 2 ]
          [ 0   1 ] [ 2 ]   [ (0)(1) + (1)(2) ]   [ 2 ]
   - Step B (RSx):
     RSx = [  0  -1 ] [ 2 ] = [ (0)(2) + (-1)(2) ] = [ -2 ]
           [  1   0 ] [ 2 ]   [ (1)(2) +  (0)(2) ]   [  2 ]

2. Compute SRx (Rotate first, then scale):
   - Step A (Rx):
     Rx = [  0  -1 ] [ 1 ] = [ (0)(1) + (-1)(2) ] = [ -2 ]
          [  1   0 ] [ 2 ]   [ (1)(1) +  (0)(2) ]   [  1 ]
   - Step B (SRx):
     SRx = [ 2   0 ] [ -2 ] = [ (2)(-2) + (0)(1) ] = [ -4 ]
           [ 0   1 ] [  1 ]   [ (0)(-2) + (1)(1) ]   [  1 ]

3. Comparison and Geometric Explanation:
   - RSx yields [-2, 2]^T, while SRx yields [-4, 1]^T.
   - Geometrically, scaling an object first along the axes alters its orientation/dimensions before it gets rotated, whereas rotating it first changes its spatial axes before scaling occurs. Because matrix multiplication is generally non-commutative, the order of transformations changes the final output coordinates.
