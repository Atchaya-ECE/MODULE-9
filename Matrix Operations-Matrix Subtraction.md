# # ➖ Matrix Operations-Matrix Subtraction in Python

## 🎯 AIM:
To write a Python Program to subtract two matrices by reading the matrix from the user.

---

## 🧠 ALGORITHM:

1. **Start**
2. Create variables `r` and `c` for rows and columns
3. Get the values of `r` and `c` from the user
4. Define a function `create_matrix(n, m)` to:
   - Prompt user for each matrix element
   - Append each row to form a complete matrix
5. Call the `create_matrix()` function twice to read two matrices `A` and `B`
6. Define a loop to subtract the elements of matrix `B` from matrix `A`
7. Store the result in a new matrix `C`
8. Print the resulting matrix `C`
9. **Stop**

---

## 💻 PROGRAM:
```
def create_matrix(n,m):
    M=[]
    for i in range(n):
        row=[]
        for j in range(m):
            x=int(input())
            row.append(x)
        M.append(row)
    return M
r,c=input().split()
A=create_matrix(int(r),int(c))
B=create_matrix(int(r),int(c))
C=[]
for i in range(int(r)):
    R=[]
    for j in range(int(c)):
        item=A[i][j]-B[i][j]
        R.append(item)
    C.append(R)
print(A)
print(B)
print(C)
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/c13e49c9-e679-4b64-85af-4df96445863d)

## RESULT:
      Thus ,the Python Program to subtract two matrices by reading the matrix from the user.
