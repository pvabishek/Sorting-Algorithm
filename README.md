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
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: P.V.Abishek
RegisterNumber: 212222230003
'''
def selection_sort(nums):
    for i in range(len(nums)):
        low=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[low]:
               low=j
        nums[i],nums[low]=nums[low],nums[i]
    print(nums)
list_of_nums = eval(input())
selection_sort(list_of_nums)




```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: P.V.Abishek
RegisterNumber: 212222230003
'''
def insertion_sort(nums):
    for i in range(1,len(nums)):
        insert=nums[i]
        j=i-1
        while j>=0 and nums[j]>insert:
              nums[j+1]=nums[j]
              j-=1
        nums[j+1]=insert
    print(nums)
 
  
    
    
list_of_nums = eval(input())
insertion_sort(list_of_nums)







```

## Output:
![Screenshot 2023-06-07 075646](https://github.com/pvabishek/Sorting-Algorithm/assets/119405626/14e85061-7935-4ab1-b406-e74a8922b8f5)

![Screenshot 2023-06-07 075701](https://github.com/pvabishek/Sorting-Algorithm/assets/119405626/56261e84-d23c-4114-9112-b6d09d9e07a8)


## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
