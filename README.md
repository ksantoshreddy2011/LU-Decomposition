# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
##Step 1:Import the numpy module to use the built-in functions for calculation

##Step 2:Prepare the lists from matrix and assign in np.array()

##Step 3:Using the np.linalg.solve(), we can find the solutions.

##Step 4:End the program

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: SANTHOSH REDDY K
RegisterNumber: 212225240137
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"


import numpy as np
from scipy.linalg import lu

A = np.array(eval(input()))

P, L, U = lu(A)

print(L)
print(U)
```


(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: SANTHOSH REDDY K
RegisterNumber: 212225240137
*/
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"


import numpy as np

from scipy.linalg import lu_factor, lu_solve

A = np.array(eval(input()))

B = np.array(eval(input()))

lu, pivot = lu_factor(A)

x = lu_solve((lu, pivot), B)

print(x)
```

## Output:
![lu decomposition]()<img width="1234" height="486" alt="Screenshot 2026-06-11 113237" src="https://github.com/user-attachments/assets/a6f870e2-696c-4d1d-99c3-02066ef163e4" />




<img width="1236" height="223" alt="image" src="https://github.com/user-attachments/assets/46f87335-6dfa-428e-8764-a0d97c4dae5f" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

