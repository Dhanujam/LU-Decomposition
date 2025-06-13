# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the numpy module and lu module from scipy.linalg to use the built-in functions for calculation
2. Prepare the lists from each linear equations and assign in np.array()
3. Using the lu(), we get three results (first is P, second is L and third is U) of the given matrix.
4. Define a package as "from scipy.linalg import lu_factor, lu_solve" and create the variable as 'X' include the package in that variable.
5. End the program

## Program:
(i) To find the L and U matrix
```
Program to find the L and U matrix.
Developed by: DHANUJA M
RegisterNumber: 212224230057
```
```
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
## Algorithm
1. Read the Input:
  Read matrix A from the user input.
  Read matrix or vector B from the user input.
2. Convert Inputs to NumPy Arrays:
  Convert A and B into NumPy arrays for computation.
3. Perform LU Decomposition:
  Use lu_factor(A) from SciPy to decompose matrix A into:
      lu: Combined lower and upper triangular matrices.
      piv: Pivot indices representing row permutations.
4. Solve the System:
   Use lu_solve((lu, piv), B) to compute the solution X.
5. Display the Result:
  Print the resulting solution vector X.

(ii) To find the LU Decomposition of a matrix
```
Program to find the LU Decomposition of a matrix.
Developed by: DHANUJA M
RegisterNumber: 212224230057
```
```
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
piv,lu=lu_factor(A)
result=lu_solve((piv,lu),B)
print(result)
```
## Output:

![alt text](<Screenshot (48).png>)

![alt text](<Screenshot (49).png>)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

