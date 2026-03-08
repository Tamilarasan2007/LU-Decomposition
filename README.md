# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program and import the required Python libraries NumPy and SciPy.
2. Read the input matrix (and constant matrix for equations) from the user
3. Perform LU Decomposition using the built-in SciPy functions to obtain L and U matrices.
4. Display the L matrix, U matrix, and the solution of the system of equations, then stop the program.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Tamilarasan R
RegisterNumber: 212225040459
'''

import numpy as np
from scipy.linalg import lu
matrix = eval(input())
P,L,U = lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Tamilarasan R 
RegisterNumber: 212225040459
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor, lu_solve

matrix = np.array(eval(input()))
constant = np.array(eval(input()))
piv, lu = lu_factor(matrix)
result = lu_solve((piv, lu), constant)
print(result)
```

## Output:
<img width="1360" height="792" alt="image" src="https://github.com/user-attachments/assets/7b9f6557-85d0-496f-80a1-69acf6fc033c" />

<img width="1342" height="661" alt="image" src="https://github.com/user-attachments/assets/a9ef9598-40e2-4250-bcc3-05e07e68827f" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

