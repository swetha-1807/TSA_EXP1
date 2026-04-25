# Ex.No: 01A PLOT A TIME SERIES DATA

###  Date:  20:4:2026

# AIM:

To develop a Python program to plot a time series graph using the given stock dataset, where Date is taken as the x-axis and Volume is taken as the y-axis, in order to analyze the trading activity and trends of stock volume over time.

# Software Required:

Google Colab

# Dataset : 

TSLA.csv


# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.

# PROGRAM:

```
import matplotlib.pyplot as plt
import pandas as pd

df = pd.read_csv("/content/TSLA.csv")

df['Date'] = pd.to_datetime(df['Date'])
df.set_index('Date', inplace=True)

plt.figure(figsize=(12,6))

plt.plot(df.index, df['Volume'], linewidth=2, color='red')

plt.xlabel('Date')
plt.ylabel('Volume')
plt.title('Stock Volume Over Time')

plt.xticks(rotation=45)
plt.grid(True)

plt.tight_layout()
plt.show()
```

# OUTPUT:

<img width="1607" height="745" alt="Screenshot 2026-04-25 082113" src="https://github.com/user-attachments/assets/fe4aee7a-89c7-4b7e-9756-268fa861dcb3" />

# RESULT:
Thus we have created the python code for plotting the time series of given data.
