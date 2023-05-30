# Ex-08-Data-Visualization-

## AIM
To Perform Data Visualization on a complex dataset and save the data to a file. 

# Explanation
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Clean the Data Set using Data Cleaning Process
### STEP 3
Apply Feature generation and selection techniques to all the features of the data set
### STEP 4
Apply data visualization techniques to identify the patterns of the data.


# CODE
```
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
tips = sns.load_dataset("tips")






tips_df = sns.load_dataset("tips")
print(tips_df)


sns.relplot(data = tips,x = "total_bill",y = "tip", hue = "day")
sns.relplot(
    data = tips,
    x = "total_bill", y="tip",hue = "smoker", style = "smoker"
)




sns.relplot(
    data = tips,
    x = "total_bill", y="tip",hue = "smoker", style = "time"
)


sns.relplot(
    data = tips,
    x = "total_bill", y="tip",hue = "smoker", style = "size"
)

sns.relplot(data = tips, x ="total_bill", y = "tip", size ="size")


sns.relplot(data = tips, x ="total_bill", y = "tip", hue = "day", col = "time")

sns.relplot(data = tips, x = "total_bill",y = "tip", col="day",col_wrap=2)

sns.lineplot(x = "total_bill", y = "tip", data = tips_df, hue = "sex",
style = "sex",
markers = ["o","<"], legend = "auto")
```
# OUPUT
![image](https://github.com/VaishaliBalamurugan22008813/Ex-08-Data-Visualization_1/assets/119390134/9524e647-aa67-4c55-8d7f-1f70a7399afc)
![image](https://github.com/VaishaliBalamurugan22008813/Ex-08-Data-Visualization_1/assets/119390134/28b59057-3a9c-416f-86f3-e85fc3dab66e)
![image](https://github.com/VaishaliBalamurugan22008813/Ex-08-Data-Visualization_1/assets/119390134/6e1de46f-4f56-4f6c-a33b-a71f7eada11a)
![image](https://github.com/VaishaliBalamurugan22008813/Ex-08-Data-Visualization_1/assets/119390134/6f87402d-b8b1-45fa-a411-ebbf85305768)
![image](https://github.com/VaishaliBalamurugan22008813/Ex-08-Data-Visualization_1/assets/119390134/9d9e32f8-9746-4a5c-83a6-2525899ba0c3)
![image](https://github.com/VaishaliBalamurugan22008813/Ex-08-Data-Visualization_1/assets/119390134/aa17744f-ae24-4101-9e83-29108aab42cb)
![image](https://github.com/VaishaliBalamurugan22008813/Ex-08-Data-Visualization_1/assets/119390134/deb25519-23d9-4002-8b2b-1ccc563c08d7)
![image](https://github.com/VaishaliBalamurugan22008813/Ex-08-Data-Visualization_1/assets/119390134/f94b6128-06bd-48ce-812a-638466d96e74)
![image](https://github.com/VaishaliBalamurugan22008813/Ex-08-Data-Visualization_1/assets/119390134/37fd4d78-be84-441e-813a-96524d10b4c9)

RESULT:
Thus, Data Visualization is performed on the given dataset and save the data to a file.
