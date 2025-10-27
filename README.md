# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

```
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df=pd.read_csv("titanic_dataset.csv")
df.head()
```
<img width="1516" height="249" alt="Screenshot 2025-10-27 113347" src="https://github.com/user-attachments/assets/a47c3a7a-743c-4705-b2d0-28b3d303f415" />

```
x=[1,2,3,4,5]
y=[3,6,2,7,1]
sns.lineplot(x=x,y=y)
plt.title('Line Plot')
```
<img width="775" height="582" alt="Screenshot 2025-10-27 113358" src="https://github.com/user-attachments/assets/a5254e11-e2ac-4bcf-a066-3d7bfb377a69" />

```
x=[1,2,3,4,5]
y1=[3,5,2,6,1]
y2=[1,6,4,3,8]
y3=[5,2,7,1,4]
sns.lineplot(x=x,y=y1)
sns.lineplot(x=x,y=y2)
sns.lineplot(x=x,y=y3)
plt.title('Multi Line Plot')
```
<img width="757" height="582" alt="Screenshot 2025-10-27 113409" src="https://github.com/user-attachments/assets/bdcada7d-186c-4a63-b67f-00fe74d24ab6" />

```
plt.figure(figsize=(8,5))
sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
plt.title("Fare Of Passenger By Embarked Town")
```
<img width="906" height="604" alt="Screenshot 2025-10-27 113422" src="https://github.com/user-attachments/assets/2bc393d5-77d3-4f73-b86e-273d10828c22" />

```
sns.scatterplot(x="Age", y="Fare", data=df)
plt.title('Scatterplot of Age vs Fare')
plt.show()
```
<img width="770" height="585" alt="Screenshot 2025-10-27 113433" src="https://github.com/user-attachments/assets/f9e61ab6-a070-4a10-ab34-a0229d840689" />

```
sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
plt.show()
```
<img width="751" height="591" alt="Screenshot 2025-10-27 113445" src="https://github.com/user-attachments/assets/6e662a32-fd00-4453-8260-5fd01d98ad90" />

```
sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
```
<img width="770" height="577" alt="Screenshot 2025-10-27 113513" src="https://github.com/user-attachments/assets/5b432bb1-303d-464e-af5a-27b61f526402" />

```
sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
plt.title("Age By Passenger Class")
```
<img width="721" height="606" alt="Screenshot 2025-10-27 113522" src="https://github.com/user-attachments/assets/639406d5-0022-46ce-8c52-eac36190f043" />

```
sns.violinplot(x="Pclass", y="Fare", data=df)
plt.title('Violin Plot of Fare by Passenger Class')
plt.show()
```
<img width="742" height="588" alt="Screenshot 2025-10-27 113532" src="https://github.com/user-attachments/assets/f080bac7-a5aa-45f8-a58d-9468ae8d46f8" />

```
sns.kdeplot(data=df['Age'], shade=True)
plt.title('Density Plot of Passenger Ages')
plt.show()
```
<img width="763" height="613" alt="Screenshot 2025-10-27 113543" src="https://github.com/user-attachments/assets/04e59d71-7a5d-46bb-ba3c-8ae767275b3b" />

# Result:
 Thus, the Data Visualization using seaborn python library for the given data is implemented successfully
