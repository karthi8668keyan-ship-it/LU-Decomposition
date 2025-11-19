# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
4. Use lu(),lu_solve(),lu_factor() to get the solutions
5. End the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: KARTHIKEYAN A
RegisterNumber: 25016466
'''
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
P,L,U=lu(a)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by:KARTHIKEYAN A
RegisterNumber:25016466
'''
import numpy as np
from scipy.linalg import lu_factor, lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,pivot=lu_factor(a)
x=lu_solve((lu,pivot),b)
print(x)
```

## Output:

<img width="1208" height="784" alt="Screenshot 2025-11-19 160705" src="https://github.com/user-attachments/assets/3181fb30-be6b-4e24-b749-e23d558252d8" />

<img width="1209" height="783" alt="Screenshot 2025-11-19 160729" src="https://github.com/user-attachments/assets/773f38e2-57b0-4662-9a81-b0d959f0769a" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

