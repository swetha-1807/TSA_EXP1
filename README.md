# Ex.No: 01A PLOT A TIME SERIES DATA

###  Date:  20:4:2026

# AIM:
To develop a Python program to plot a time series graph using the given Salary dataset, where Age is taken as the x-axis and Salary is taken as the y-axis, in order to analyze the relationship and trend between age and salary.

# Software Required:

Google Colab

# Dataset : 

Salary.csv


# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.

# PROGRAM:

```
from matplotlib import pyplot as plt
import pandas as pd

# Read dataset
df = pd.read_csv("/content/Salary_Data.csv")

# Scatter plot
plt.figure(figsize=(8,5))
plt.scatter(df['Age'], df['Salary'], color='blue')

# Title and labels
plt.title("Age vs Salary")
plt.xlabel("Age")
plt.ylabel("Salary")

# Grid
plt.grid(True)

# Show plot
plt.show()
```

# OUTPUT:

<img width="721" height="470" alt="image" src="https://github.com/user-attachments/assets/874b56aa-cdae-436d-9b87-3c0b79a59b9f" />

# RESULT:
Thus we have created the python code for plotting the time series of given data.
