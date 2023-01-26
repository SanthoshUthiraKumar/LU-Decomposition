# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1:
Import the library numpy using the import command.

### Step 2:
Import lu using from scipy.linalg for first program and inport lu_factor,lu_solve using from scipy.linalg for second program.

### Step 3: 
Assigning a matrix to a variable for first program.For the second program,Assigning two matrices

### Step 4:
Using the lu(), we can find the l and u of the matrix for first program.Using lu_factor and lu_solve find the LU Decomposition for second program.

### Step 5:
Print the results and end the program.

## Program:
(i) To find the L and U matrix
```
'''
Program to find L and U matrix using LU decomposition.
Developed by: Santhosh U
RegisterNumber: 22009224
'''
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```

(ii) To find the LU Decomposition of a matrix
```
'''
Program to solve a matrix using LU decomposition.
Developed by: Santhosh U
RegisterNumber: 22009224
'''

# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,piv=lu_factor(A)
x=lu_solve((lu,piv),B)
print(x)
```

## Output:
(i) To find the L and U matrix
![LU1Output](https://user-images.githubusercontent.com/119477975/214603661-1b54df27-f190-4fb0-9378-497724655a18.png)

(ii) To find the LU Decomposition of a matrix
![LU2Output](https://user-images.githubusercontent.com/119477975/214603694-799b67bc-912f-4076-aa54-a66fcf05c482.png)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

