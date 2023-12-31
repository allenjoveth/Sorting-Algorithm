# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1. start the program to sort and inserting sort fas function
2. then give condition respective to the question in for loop
3. then seperate the values
4. now the sorting and insertion sorting as been done to give output 
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
Developed by: Allen Joveth P
RegisterNumber: 23009582
'''
def selection_sort(nums):
    for i in range(len(nums)):
        lowest_value_index = i
        for j in range(i+1, len(nums)):
            if nums[j] < nums[lowest_value_index]:
                lowest_value_index = j
        nums[i], nums[lowest_value_index] = nums[lowest_value_index],nums[i]
        
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)

```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: Allen Joveth P
RegisterNumber: 23009582
'''
def insertion_sort(nums):

    for i in range(1, len(nums)):

        item_to_insert = nums[i]

        j = i - 1

        while j >= 0 and nums[j] > item_to_insert:

            nums[j+1] = nums[j]

            j -= 1

        nums[j+1] = item_to_insert

        

list_of_nums = eval(input())

insertion_sort(list_of_nums)

print(list_of_nums)
```

## Output:

#Selection Sort
![Screenshot 2023-12-31 135327](https://github.com/allenjoveth/Sorting-Algorithm/assets/139422287/5640645a-00b1-4c38-8b81-7317e2afe646)

#Insertion Sort
![Screenshot 2023-12-31 135442](https://github.com/allenjoveth/Sorting-Algorithm/assets/139422287/d35aa4b8-e9d1-4b43-8849-c4006fb4549f)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
