# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner


### Algorithm (i)
1.Import necessary libraries: Import numpy as np and lu from scipy.linalg.

2.Get matrix input: Read the matrix A from the user using input() and convert it to a NumPy array with np.array(eval(input())).

3.Perform LU decomposition: Use lu(A) to decompose matrix A into P, L, and U.

4.Extract results: Get the lower triangular matrix L and upper triangular matrix U.

5.Display output: Print matrices L and U using the print() function.

### Algorthim (ii)
1.Import required libraries: Import numpy as np and lu_factor, lu_solve from scipy.linalg.

2.Take input: Read matrix A and vector b from the user using input() and convert them to NumPy arrays.

3.LU factorization: Use lu_factor(A) to compute the LU decomposition and pivot indices of matrix A.

4.Solve the system: Use lu_solve((lu, piv), b) to find the solution vector X for the equation AX = b.

5.Display the result: Print the solution vector X using print().

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

