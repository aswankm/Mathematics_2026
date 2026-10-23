# Exercise 5. Matrix Times Vector

### Statement

$$
Let A = [ 2  -1 ] and x = [ 4 ][cite: 15]. Compute Ax. Then express Ax as a linear combination of the columns of A, with coefficients coming from the vector x[cite: 15].
        [ 1   3 ]          [ 2 ]
$$


### Theory
* **Matrix-Vector Multiplication:** Multiplying a matrix by a vector can be understood as taking the dot products of the rows of the matrix with the vector, or equivalently, as a linear combination of the columns of the matrix weighted by the entries of the vector[cite: 15].

### Essential Steps & Solution
1. **Compute Ax:**
   ```text
   Ax = [ 2  -1 ] [ 4 ] = [ (2)(4) + (-1)(2) ] = [ 8 - 2 ] = [ 6  ]
        [ 1   3 ] [ 2 ]   [ (1)(4) + (3)(2) ]   [ 4 + 6 ]   [ 10 ]
