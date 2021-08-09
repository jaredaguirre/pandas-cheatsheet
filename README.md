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

## Series & Dataframes

`(axis=0)` means a row, `(axis=1)` means a column.

```python
import pandas as pd
series = pd.Series(["BMW", "Toyota", "Honda"])  # Series are 1-dimensional
series

#0       BMW
#1       Toyota
#2       Honda
#dtype: object

colors = pd.Series(['Red', 'Blue', 'White'])

car_data = pd.DataFrame({'car': series, 'color': colors})   # Dataframes are 2-dimensional
car_data

#  car	  color
#-------------------
#0 BMW	  Red
#1 Toyota	Blue
#2 Honda	White

```

## Import and export

```python
# Import from local
car_sales = pd.read_csv('car-sales.csv')

# Import from URL
heart_disease = pd.read_csv("https://raw.githubusercontent.com/mrdbourke/zero-to-mastery-ml/master/data/heart-disease.csv")

# Export
car_sales.to_csv('exported_car_sales.csv')
car_sales.to_csv('exported_car_sales.csv', index=False) # To export it with the index column as part of the table
```
The first imported file car_sales would be like this:

|  | Make	   |Colour	|Odometer(KM)	|Doors	  |Price     |
|--|---------|--------|-------------|---------|----------|
|0 |Toyota	 |White	  |150043	      |4	      |$4,000.00 |
|1 |Honda	   |Red	    |87899	      |4	      |$5,000.00 |
|2 |Toyota	 |Blue	  |32549	      |3	      |$7,000.00 |
|3 |BMW	     |Black	  |11179	      |5	      |$22,000.00|
|4 |Nissan	 |White	  |213095	      |4	      |$3,500.00 |


