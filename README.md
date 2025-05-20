# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step1 : Import the numpy module to use the built-in functions for calculation
### Step 2: Prepare the lists from each equations and assign in np.array() 
### Step 3: Using the np.linalg.matrix_rank(), we can find the inverse of the given matrix 
### Step 4: End the program

## Program:
~~~
'''Program to find L and U matrix using LU decomposition.
Developed by:S.Sandeep
RegisterNumber:212224230239
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
~~~
~~~
'''Program to solve a matrix using LU decomposition.
Developed by:S.Sandeep
RegisterNumber:212224230239
'''


import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,piv=lu_factor(A)
X=lu_solve((lu,piv),B)
print(X)
~~~

## Output:
![image](https://github.com/user-attachments/assets/3d861ff8-4dee-456d-a382-5c77883aa042)
![image](https://github.com/user-attachments/assets/3ba5396e-b120-4225-813f-2f525c5a2382)




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

