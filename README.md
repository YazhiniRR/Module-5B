# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np
a=np.array(eval(input()))
print("Given array")
print(end=" ")
print(a)
print()
print(np.sort(a,axis=0))
```

## Output
![441083508-541029ec-c844-4f85-b04f-69b54f623f29](https://github.com/user-attachments/assets/fcf5ff6d-eb42-4946-b8ef-b176adac89af)

## Result
Thus the python program for sorting each column in numpy has been implemented and executed successfully.
# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program
```
import numpy as np 
x=eval(input())
y=eval(input())
l1=np.array(x)
l2=np.array(y)
 
print(np.where(l1>l2))
print(np.where(l1==l2))
```

## Output
![441083879-4b201760-2d96-4f59-89bc-ef45e345ce50](https://github.com/user-attachments/assets/0a78394b-649f-4694-9ee6-6a1a65bedf76)

## Result
Thus the python program for element wise comparison between two numpy array has been implemented and executed successfully.
# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
```
a=np.array(eval(input()))
b=np.array(eval(input()))
print("Printing Original array")
print(a)
print("Array after deleting column 2 on axis 1")
c=np.delete(a,1,axis=1) 
print(c)
print("Array after inserting column 2 on axis 1")
print(np.insert(c,1,b,axis=1))
```


## Output
![441084198-a0e3777c-4c9e-4352-bce2-73ef0ff78ad3](https://github.com/user-attachments/assets/fd9476cb-e474-4754-a69b-487ed159705d)

## Result

Thus the python program for replacing column in numpy has been implemented and executed successfully.
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
import pandas as pd
import numpy as np
exam_data = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew','Laura', 'Kevin', 'Jonas'],
 'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
 'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
 'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']
df = pd.DataFrame(exam_data , index=labels)
print(df)
```

## Output
![441084511-eea054b4-a18c-4e19-b2d3-856898a5664d](https://github.com/user-attachments/assets/d4982194-4418-4111-824a-61093029be67)

## Result
Thus the python program for replacing column in numpy has been implemented and executed successfully.
# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program
```
import pandas as pd
student_data1 = pd.DataFrame({
 'student_id': ['S1', 'S2', 'S3', 'S4', 'S5'],
 'name': ['Danniella Fenton', 'Ryder Storey', 'Bryce Jensen', 'Ed Bernal', 'Kwame Morin'], 
 'marks': [200, 210, 190, 222, 199]})
student_data2 = pd.DataFrame({
 'student_id': ['S4', 'S5', 'S6', 'S7', 'S8'],
 'name': ['Scarlette Fisher', 'Carla Williamson', 'Dante Morse', 'Kaiser William', 'Madeeha Preston'], 
 'marks': [201, 200, 198, 219, 201]})
print("Original DataFrames:")
print(student_data1)
print("-------------------------------------")
print(student_data2)
print("\nJoin the said two dataframes along rows:")
result_data = pd.concat([student_data1, student_data2])
print(result_data)
```

## Output
![441084815-3600ef6d-183b-4e8d-964c-83984656974e](https://github.com/user-attachments/assets/da96be0f-7f8c-48a4-bf2d-2c4aaab80c98)
![441084870-ec6606d3-3810-434c-9730-6d22493ed409](https://github.com/user-attachments/assets/ff545b6e-5fbd-48c0-aadc-65ce24f7cd4a)

## Result
Thus, the Python program has been successfully created and executed successfully to join the two DataFrames row-wise using pd.concat() and all records from both DataFrames were included in the final output.
