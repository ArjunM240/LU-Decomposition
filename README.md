# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### 5(a)
### step 1. import numpy for multi-dimensional array operations
### step 2. bring lu from scipy.linalg to handle the actual matrix decomposition 
### step 3. call the lu(A) function. This splits the target matrix inoto three seperate output matrices P,L and U
### step 4. stop the program
### 5(b)
### step 1. import numpy for multi-dimensional array operations
### step 2. bring lu from scipy.linalg to handle the actual matrix decomposition
### step 3. pass the factorized components (lu,p) along with the right-hand side matrix b into the lu_solve() function to compute the solution matrix x
### step 4. stop the program

## Program:
(i) To find the L and U matrix
### '''Program to find L and U matrix using LU decomposition.
### Developed by: Arjun M
### RegisterNumber: 26017171
### '''
### import os
### os.environ["OPENBLAS_NUM_THREADS"]="1"
### import numpy as np
### from scipy.linalg import lu
### A=np.array(eval(input()),dtype=float)
### P,L,U=lu(A)
### print(L)
### print(U)

(ii) To find the LU Decomposition of a matrix

 '''Program to solve a matrix using LU decomposition.
 Developed by: Arjun M
 RegisterNumber: 26017171
 '''

 # To print X matrix (solution to the equations)
 import os
 os.environ["OPENBLAS_NUM_THREADS"]="1"
 import numpy as np
 from scipy.linalg import lu_factor,lu_solve

 a=np.array(eval(input()))
 b=np.array(eval(input()))

 l,p = lu_factor(a)
 x = lu_solve((l,p),b)
 print(x)


## Output:
![lu decomposition]()
<img width="1242" height="787" alt="image" src="https://github.com/user-attachments/assets/f5c2bd98-0b7c-41c7-b5c1-522954dd84d5" />
<img width="1203" height="786" alt="image" src="https://github.com/user-attachments/assets/f46e0d46-ce34-4954-907b-592c6920d567" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

