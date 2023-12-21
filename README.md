# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. read the elements of augmented matrix into array a and b
2.calculate elements of L and U
3.print L and U matrix
4.find V by solving LV = B by forwrd substitution
5.find X by solving UX = V by backward substitution
6.print array X as the solution
   

## Program:
(i) To find the L and U matrix
'''Program to find L and U matrix using LU decomposition.
Developed by: SARON XAVIER A.
RegisterNumber: 23005103
'''
from scipy.linalg import lu
import numpy as np
arr=eval(input())
A=np.array(arr)
P,L,U=lu(A)
print(L)
print(U)

(ii) To find the LU Decomposition of a matrix
'''Program to solve a matrix using LU decomposition.
Developed by: SARON XAVIER A.
RegisterNumber: 23005103
'''
from scipy.linalg import lu_factor,lu_solve
import numpy as np
arr=eval(input())
constant=eval(input())
A=np.array(arr)
B=np.array(constant)
result=lu_factor(A)
solution=lu_solve(result,B)
print(solution)

# To print X matrix (solution to the equations)


## Output:
![image](https://github.com/saron2006/LU-Decomposition/assets/138849343/a47aebab-6d23-4ab4-9561-f1067c3562d7)

![image](https://github.com/saron2006/LU-Decomposition/assets/138849343/60432d39-5501-4974-a741-6e354e44aff0)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

