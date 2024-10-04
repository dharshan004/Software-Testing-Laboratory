# Ex.No: 1 Write programs in Python Language to demonstrate the working of followingconstructs with possible test cases: a) do…while b) while…do c) if …else d) switch e) for 

### DATE:                                                                            
### REGISTER NUMBER : 

### AIM:  
To write python programs for do…while, while, for, switch and if…else and test with possible test 
Cases 

### Algorithm:
1. Start the program.
2. Create separate files for each given program.
3. Write simple program for each construct.
4.  the program with possible test cases.
5. Stop the program.
### Program:
r1,c1=input("enter row and column count in matrix 1: ").split()
r2,c2=input("enter row and column count in matrix 2: ").split()
matrix1=[ ]
matrix2=[ ]
result=[ ]
if(r1.isnumeric() and c1.isnumeric() and r2.isnumeric() and c2.isnumeric()):
    r1=int(r1)
    r2=int(r2)
    c1=int(c1)
    c2=int(c2)
    if(c1!=r2):
        print("Matrix multiplication not possible")
    elif (max(r1,c1,r2,c2)>20 or min(r1,c1,r2,c2)==0):
        print("Matrix multiplication not possible")
else:
    for i in range(r1):
        a=[]
        for j in range(c1):
            a.append(int(input("<-")))
            matrix1.append(a)
for i in range(r2):
    a=[]
    for j in range(c2):
        a.append(int(input("<-")))
        matrix2.append(a)
        for i in range(r1):
            inter=[]
            for j in range(c2):
                sum=0
                for k in range(r2):
                    sum += matrix1[i][k] * matrix2[k][j]
                    inter.append(sum)
                    result.append(inter)

for i in range(r1):
    for j in range(c2):
        print(result[i][j],end=" ")
        print()
else:
    print("enter a valid number") 














### Output:







### Result:
Thus, the python program to demonstrate the working of given constructs is implemented and the output is verified successfully.


