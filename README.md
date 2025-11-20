# PYTHON PROGRAMMMINDG MODULE 5

### NAME : SANGAMITHRA B
### REGISTER NUMBER : 212224060035

# NumPy Program: Column-wise Sorting of a 2D Array

## Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## Program
```
import numpy as np
a=eval(input())
array = np.array(a)
print('Given array','\n',array)
print()
print(np.sort(array,axis=0))
```
## Output
<img width="698" height="534" alt="Screenshot 2025-10-21 174345" src="https://github.com/user-attachments/assets/318cf39a-613b-4551-a05e-cb6c2974a63d" />

## Result
Thus,the numpy program that sorts a element of given 2d array in ascending order is created successfully
# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

##  Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

##  Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## Program
```
import numpy as np
x = np.array(eval(input()))
y = np.array(eval(input()))
greater = np.where(x>y)
equal = np.where(x==y)
print(greater)
print(equal)
```
## Output
<img width="1002" height="209" alt="Screenshot 2025-10-21 190452" src="https://github.com/user-attachments/assets/f7536893-c9ba-4b63-9ead-b4a9123c6c73" />

## Result
Thus, a Python program using NumPy that finds the indices where elements in array 'x' are greater than or equal to their corresponding elements in array 'y' is created successfully.
# NumPy Program: Replace the Second Column in a 2D Array

##  Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

##  Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

##  Program
```
import numpy as np
arr_str = input()
arr = np.array(eval(arr_str))
print("Printing Original array")
print(arr)
arr_deleted = np.delete(arr, 1, axis=1)
print("Array after deleting column 2 on axis 1")
print(arr_deleted)
new_col_str = input()
new_col = np.array(eval(new_col_str))
arr_final = np.insert(arr_deleted, 1, new_col, axis=1)
print("Array after inserting column 2 on axis 1")
print(arr_final)

```
## Output
<img width="1162" height="652" alt="Screenshot 2025-10-21 175345" src="https://github.com/user-attachments/assets/a387ecf0-c28a-4992-acd9-36941ad51723" />

## Result
# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
```
import numpy as np
import pandas as pd
a=eval(input())
b=np.array(eval(input()))
df=pd.DataFrame(a,index=b)
print(df)
```
## Output
<img width="949" height="241" alt="Screenshot 2025-10-21 191043" src="https://github.com/user-attachments/assets/7f70f48b-8b00-443c-a98d-ae7f0e2b17d7" />

## Result
Thus,the python program To create and display a DataFrame using the Pandas library in Python from a given dictionary, and apply specific index labels to the rows is created successfully.
#  Pandas Program: Join Two DataFrames Along Rows

##  AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

##  ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

##  Program
```
import pandas as pd
d1=eval(input())
d2=eval(input())
df1=pd.DataFrame(d1)
df2=pd.DataFrame(d2)
print("Original DataFrames:")
print(df1)
print("-------------------------------------")
print(df2)
jd=pd.concat([df1,df2])
print("\nJoin the said two dataframes along rows:")
print(jd)
```
## Output
<img width="1297" height="523" alt="Screenshot 2025-10-21 180828" src="https://github.com/user-attachments/assets/2412a1fb-8766-4a89-b139-88e7b44d641b" />

## Result
Thus,the Python program using Pandas to join two DataFrames along rows and assign all data to a new DataFrame is created successfully.

