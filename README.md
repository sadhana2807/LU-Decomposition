# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner
 
Algorithm – To Find L and U Matrix

1. Import the NumPy library and the lu function from scipy.linalg.
2. Read the elements of the square matrix from the user.
3. Convert the given matrix into a NumPy array.
4. Use the lu() function to decompose the matrix into P, L, and U matrices.
5. Obtain the Lower triangular matrix (L) and Upper triangular matrix (U).
6. Display the L and U matrices.

Algorithm – To Find LU Decomposition

1. Import NumPy and the lu_factor and lu_solve functions from scipy.linalg.
2. Read the coefficient matrix and the constant vector from the user.
3. Convert the given inputs into NumPy arrays.
4. Use lu_factor() to obtain the LU factorization and pivot information.
5. Use lu_solve() with the factorized matrix to find the solution.
6. Display the obtained solution/result. 

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Sadhana K
RegisterNumber: 212225240128
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Sadhana K
RegisterNumber: 212225240128
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),b)
print(X)
```

## Output:

<img width="1039" height="824" alt="image" src="https://github.com/user-attachments/assets/293f4778-39da-451c-b042-a6c061696753" />

<img width="961" height="676" alt="image" src="https://github.com/user-attachments/assets/6d880adc-f339-4a24-a552-b7effc4afc6a" />


![lu decomposition]()


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

