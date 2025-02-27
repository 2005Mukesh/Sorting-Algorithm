# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
def selection_sort(array,size):
    for ind in range(size):
        min_index= ind
        for j in range(ind+1,size):
            if array[j] < array[min_index]:
               min_index=j
        (array[ind],array[min_index]) = (array[min_index],array[ind])
arr = eval(input())
size=len(arr)
selection_sort(arr,size)
print(arr)
```
ii)	#Insertion Sort
```
def insertion_sort(arr):
    n=len(arr)
    if n<=1:
        return
    for i in range(1,n):
        key=arr[i]
        j=i-1
        while j>=0 and key<arr[j]:
            arr[j+1]=arr[j]
            j-=1
        arr[j+1]=key
arr = eval(input())
insertion_sort(arr)
print(arr)
```

## Output:
i)	#Selection Sort.
![Screenshot 2023-11-20 141539](https://github.com/2005Mukesh/Sorting-Algorithm/assets/138849308/14557caa-a4a0-484d-98f4-537a842bda2f)


ii)	#Insertion Sort.
![Screenshot 2023-11-20 141607](https://github.com/2005Mukesh/Sorting-Algorithm/assets/138849308/1fb364af-1068-4c25-97d0-9fe15f468b95)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
