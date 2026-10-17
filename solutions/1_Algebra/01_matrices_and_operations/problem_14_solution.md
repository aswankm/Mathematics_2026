# Exercise 14. Rotation Matrices

### Statement & Solution Overview
The matrix for a rotation through an angle $\theta$ is:
```text
R(theta) = [ cos(theta)  -sin(theta) ]
           [ sin(theta)   cos(theta) ]
1. Compute Product R(alpha)R(beta):
   R(alpha)R(beta) = [ cos(alpha)  -sin(alpha) ] [ cos(beta)  -sin(beta) ]
                   [ sin(alpha)   cos(alpha) ] [ sin(beta)   cos(beta) ]

   - Row 1, Col 1: cos(alpha)cos(beta) - sin(alpha)sin(beta) = cos(alpha + beta)
   - Row 1, Col 2: -cos(alpha)sin(beta) - sin(alpha)cos(beta) = -[sin(alpha)cos(beta) + cos(alpha)sin(beta)] = -sin(alpha + beta)
   - Row 2, Col 1: sin(alpha)cos(beta) + cos(alpha)sin(beta) = sin(alpha + beta)
   - Row 2, Col 2: -sin(alpha)sin(beta) + cos(alpha)cos(beta) = cos(alpha + beta)

2. Resulting Matrix via Angle-Sum Identities:
   R(alpha)R(beta) = [ cos(alpha + beta)  -sin(alpha + beta) ]
                     [ sin(alpha + beta)   cos(alpha + beta) ]
                   = R(alpha + beta)

3. Geometric Explanation:
   - Multiplying the rotation matrices algebraically combines their rotation angles. 
   - Geometrically, rotating by beta first and then by alpha is equivalent to a single net rotation by the sum of the two angles, (alpha + beta).
