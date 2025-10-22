# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

# LINE PLOT :

```
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

```
marks = [13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student Name')
plt.show()

student = ['A','B','C','D']
attendence = [90,85,73,88]
plt.plot(student,attendence)
plt.xlabel('Attendence')
plt.ylabel('student Name')
plt.show()
```

<img width="520" height="391" alt="image" src="https://github.com/user-attachments/assets/39feab7a-8e81-4222-ae18-29c04d8e3493" />

<img width="515" height="397" alt="image" src="https://github.com/user-attachments/assets/48af68ac-431a-4f02-a11f-6189c6a8f144" />

# SCATTER PLOT:

```
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()
```

<img width="499" height="378" alt="image" src="https://github.com/user-attachments/assets/11388af8-dfc6-471c-ba48-5c9d5a430f5f" />

```
x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```

<img width="506" height="412" alt="image" src="https://github.com/user-attachments/assets/088804aa-bd94-4efd-8516-71b535eaecf5" />

# PIE CHART:

```
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```

<img width="407" height="375" alt="image" src="https://github.com/user-attachments/assets/fce2bd1b-714e-4cae-9b1a-9a241b320b25" />

```
feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```

<img width="398" height="362" alt="image" src="https://github.com/user-attachments/assets/8e7b9428-876e-479d-a588-84aea73f1807" />

# AREA CHART:

```
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```

<img width="500" height="368" alt="image" src="https://github.com/user-attachments/assets/aea66059-b854-422b-b478-12a57dbe466e" />

# BAR CHART:

```
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```

<img width="508" height="414" alt="image" src="https://github.com/user-attachments/assets/23402013-1311-4b64-88a2-c498c9cd90d6" />

# HISTOGRAM :
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```

<img width="482" height="375" alt="image" src="https://github.com/user-attachments/assets/7d354f44-28ab-443d-b35f-74f3d31485b2" />

# BOX PLOT:

```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```

<img width="556" height="329" alt="image" src="https://github.com/user-attachments/assets/315d7d15-d4b1-458a-8bbb-2e5e640ba33e" />

```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

<img width="565" height="445" alt="image" src="https://github.com/user-attachments/assets/4448e661-9ff0-4004-94de-aa2cb1e862ac" />


# Result:

Thus, all the data visualization techniques of matplotlib has been implemented.
