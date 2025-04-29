# EX 1C Quick Sort
## AIM:
To write a python program to implement quick sort using tha last element as pivot on the list of float values.

## Algorithm
1. Select a pivot element from the array (commonly the first or last element).
2. Partition the array into two subarrays: elements less than pivot and elements greater than or equal to pivot.
3. Place the pivot between the two subarrays at its correct position.
4. Recursively apply Quick Sort to the left subarray.
5. Recursively apply Quick Sort to the right subarray.
   

## Program:
```
/*
Program to implement implement quick sort using the last element as pivot on the list of float values.
Developed by: kabilan T
Register Number: 212222230059
*/
```
```
def partition(array, low, high):
    pivot = array[low]
    start = low + 1
    end = high
    print("pivot: ",pivot)
    while True:
        while start <= end and array[end] >= pivot:
            end = end - 1
        while start <= end and array[start] <= pivot:
            start = start + 1
        if start <= end:
            array[start], array[end] = array[end], array[start]
        else:
            break
    array[low], array[end] = array[end], array[low]
    return end
def quick_sort(array, start, end):
    if start < end:
        idx = partition(array, start, end)
        quick_sort(array, start, idx-1)
        quick_sort(array, idx+1, end)
arr1=[]
n=int(input())
for i in range(n):
    arr1.append(int(input()))
print("Input List\n",arr1)
quick_sort(arr1, 0, len(arr1)-1)
print("Sorted List\n",arr1)
```

## Output:
![193](https://github.com/user-attachments/assets/a1fa179f-6bea-4c2a-b1c8-99bce3dc15e8)



## Result:
The program successfully sorts the input array using the QuickSort algorithm, arranging the elements in ascending order.
