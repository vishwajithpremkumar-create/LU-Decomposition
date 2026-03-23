# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm 
```
1. Start the program
2.Import the necessary libraries(numpy,scipy.linalg)
3.Define the matrix using numpy
4.Use lu(),lu_solve(),lu_factor() to get the solutions
5.End the program 
```
## Program:
(i) To find the L and U matrix
```

Program to find the L and U matrix.
Developed by: vishwajith p
RegisterNumber: 212225220122

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

Program to find the LU Decomposition of a matrix.
Developed by: vishwajith p
RegisterNumber: 212225220122

import os 
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np 
from scipy.linalg import lu_factor, lu_solve
A=np.array([[3,2,7],[2,3,1],[3,4,1]])
b=np.array([4,5,7])
lu,piv = lu_factor(A)
x=lu_solve((lu,piv),b)
print(x)
```

## Output:

<img width="1920" height="1080" alt="Screenshot 2026-03-23 224202" src="https://github.com/user-attachments/assets/c59abfaa-d4b4-4a83-8b71-20053da1c292" />

<img width="1920" height="1080" alt="Screenshot 2026-03-23 224216" src="https://github.com/user-attachments/assets/c1c9210d-e653-42ca-90f6-c53be9abed91" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

