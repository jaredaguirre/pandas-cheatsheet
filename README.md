# Jare's Pandas Cheathseet

![](https://user-images.githubusercontent.com/64754731/128677452-ae8634aa-91c4-40c4-b0ef-2e3f7c8b2065.png)

The awesome Data Analysis tool! This cheatsheet will cover the following features and tools from the pandas library:

## Contents

### Most Useful Functions: 

[]

### Datatypes

[Series](#), [Dataframes](#)

### Importing & Exporting Data

### Describing Data

### Viewing and Selecting Data

### Manipulating Data


---

## Series

```python
import pandas as pd
series = pd.Series(["BMW", "Toyota", "Honda"])  # Series are 1-dimensional
series

#0       BMW
#1    Toyota
#2     Honda
#dtype: object

colors = pd.Series(['Red', 'Blue', 'White'])

car_data = pd.DataFrame({'car': series, 'color': colors})   # Dataframes are 2-dimensional
car_data

#car	color
#-------------------
#0	  BMW	Red
#1	  Toyota	Blue
#2	  Honda	White

```


