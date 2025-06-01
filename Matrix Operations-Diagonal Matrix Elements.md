# Matrix Operations-Diagonal Matrix Elements Printer 🧮

This Python program reads a matrix of any size from the user and prints **only the diagonal elements**, leaving other elements blank in the output.

## 📌 Aim

To write a Python program to print the column-wise sum of a matrix.
## 🧠 Algorithm

1. Read the number of rows and columns from the user.
2. Initialize an empty matrix of size `rows × columns`.
3. Populate the matrix with user input.
4. Display the full matrix.
5. Iterate through the matrix and:
   - If `i == j`, print the element (main diagonal).
   - Else, print a blank space.
6. Print a newline after each row.

## 🖥️ Program
```
rows=int(input())
columns=int(input())
matrix=[[0]*columns for row in range(rows)]
print("Matrix:")
for i in range(rows):
    lines=list(map(int,input().split()))
    for j in range(columns):
        matrix[i][j]=lines[j]
for i in range(rows):
    for j in range(columns):
        print(matrix[i][j],end=" ")
    print()
for i in range(columns):
    sum=0
    for j in range(rows):    
        sum=sum+matrix[j][i]
    print('Sum of Columns[',i,'] = ',sum)
```
### Output:
![image](https://github.com/user-attachments/assets/20dbe42a-cc9b-4b7d-9d2c-ce1fe8bafcaa)

## Result
     Thus the Python program to print the column-wise sum of a matrix.
