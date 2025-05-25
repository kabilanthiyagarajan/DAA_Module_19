# EX 1D Linear search
## 25/2/2025
## AIM:
To write a python program for a search function with parameter list name and the value to be searched using string values.



## Algorithm
1. Loop through each element in the tuple.
2. Compare the current element with the target value x.
3. If the element matches x, print that the element was found and stop the search.
4. If no match is found after checking all elements, print that the element was not found.
5. End the function.

## Program:
```
/*
Program to implement a search function with parameter list name and the value to be searched using string values.
Developed by: kabilan T
Register Number: 212222230059
*/
```
```
def search(tuple1,x):
    for value in tuple1:
        if(value==x):
            print("Tuple: %d found"%x)
            return 0
    print("Tuple: %d not found"%x)
    
List=[]
n=int(input())
for i in range(n):
    List.append(int(input()))
tuple1=tuple(List)
x=float(input())
search(tuple1,x)
```
## Output:
![194](https://github.com/user-attachments/assets/968b57a2-84d8-442d-9c3c-37f639ebf17e)



## Result:
The program was executed successfully, and it correctly checks if the input element is present in the list, printing "Found" if the element exists or "Not Found" if it does not.
