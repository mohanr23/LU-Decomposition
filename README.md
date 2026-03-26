# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
Step 1: Import the numpy module to use built-in functions for calculations.
Step 2: Import the lu function from scipy.linalg to perform LU decomposition.
Step 3: Read the input matrix, perform LU decomposition using lu(A), and print the L matrix and U matrix.
Step 4: End the program.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: MOHAN R
RegisterNumber: 212224230168
'''
import numpy as np
from scipy.linalg import lu
matrix = eval(input())
p,l,u=lu(matrix)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: MOHAN R
RegisterNumber: 212224230168
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input())) 
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),B)
print(x)
```

## Output:
i)
<img width="1106" height="383" alt="image" src="https://github.com/user-attachments/assets/5883fbf9-061e-451a-b6f1-4779ac7d4fbe" />

ii)
<img width="765" height="165" alt="image" src="https://github.com/user-attachments/assets/768e6172-2761-4e7f-8cc0-f9ed18af7732" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

