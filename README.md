# TSA_EXP1A

### Developed By: Moenish Baalan
### Reg No: 212223220057
###  Date: 12.08.2025
# Ex.No: 01A PLOT A TIME SERIES DATA

# AIM:
To Develop a python program to Plot a time series data (Books & their Publication year)
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Using pd.to_datetime we're coverting date/month/year to only year.
4. Plot the data according to need and can be altered yearly.
5. Display the graph.

# PROGRAM:
Python

```
import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv("results.csv")

df['date'] = pd.to_datetime(df['date'])

plt.figure(figsize=(12, 6))
plt.plot(df['date'], df['home_score'], marker='o', markersize=2, linestyle='-', alpha=0.6)

plt.title('Home Score Over Time')
plt.xlabel('Date')
plt.ylabel('Home Score')
plt.grid(True, linestyle='--', alpha=0.5)
plt.tight_layout()

plt.show()

```

# OUTPUT:

![image](https://github.com/user-attachments/assets/6ba6fe40-2fda-490a-952c-033d6f2b0408)

# RESULT:
Thus we have created the Python code for plotting the time series of given data.
