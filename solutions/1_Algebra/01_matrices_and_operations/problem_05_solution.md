"""
Exercise 5: Matrix Times Vector and Linear Combination
Description: Computes matrix-vector multiplication and demonstrates 
that it can be viewed as a linear combination of the matrix columns.
"""

import numpy as np

def solve_exercise_5():
    # Define matrix A and vector x
    A = np.array([[2, -1], 
                  [1, 3]])
    
    x = np.array([4, 
                  2])

    # 1. Compute Ax
    Ax = np.dot(A, x)
    print("Computed Ax:")
    print(Ax)

    # 2. Extract columns of A
    c1 = A[:, 0]
    c2 = A[:, 1]

    # 3. Express Ax as a linear combination of columns using coefficients from x
    linear_combination = x[0] * c1 + x[1] * c2
    print("\nLinear Combination (x[0]*c1 + x[1]*c2):")
    print(linear_combination)

    # Verification
    assert np.allclose(Ax, linear_combination), "Results do not match!"
    print("\nVerification successful: Ax is equivalent to the linear combination of the columns of A.")

if __name__ == "__main__":
    solve_exercise_5()
    
