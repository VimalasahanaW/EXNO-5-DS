# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY
## NAME:VIMALA SAHANA W
## REG NO:212223040241
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

# Coding And Output :
```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
x = [1, 2, 3, 4, 5]
y = [3, 6, 2, 7, 1]
plt.plot(x,y,label='line1')
```
![image](https://github.com/user-attachments/assets/82560d38-2529-4143-908d-732d9d755b84)
```
x1 = [1,2,3]
y1 = [2,4,1]
x2 = [1,2,3]
y2 = [4,1,3]
plt.plot(x1,y1,label='line1')
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/77f4f7c3-5f9a-4cd3-bc81-46bc330d470e)
```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
```
![image](https://github.com/user-attachments/assets/09472666-f3c5-4a10-bb4c-ed6b7e41e3e1)
```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![image](https://github.com/user-attachments/assets/028a076b-b792-4f23-847d-effb74430ea5)
```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```
![image](https://github.com/user-attachments/assets/4e02317f-35d4-4243-949a-f435c5ac9113)
```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
```
![image](https://github.com/user-attachments/assets/b1eafcfc-e7b5-4a4e-bb63-10c6117ae993)
```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```
![image](https://github.com/user-attachments/assets/e6d629e2-f307-49aa-889a-809d20a40849)
```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```
![image](https://github.com/user-attachments/assets/9a028d49-4f21-4f41-8615-dc9dd0d7bb61)
```
y
```
![image](https://github.com/user-attachments/assets/cd9cba13-f5b0-4add-ae6d-5e1ff465ad5f)
```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/user-attachments/assets/9d0a3e2d-f947-4cc9-bbc8-1121fc420186)
```
y=x*x
y
```
![image](https://github.com/user-attachments/assets/619bc7cc-e2a8-4f47-85ba-c40eb2e5e13f)
```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);
```
![image](https://github.com/user-attachments/assets/08bde48e-f432-4109-8a86-fcff2f61fb90)
```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![image](https://github.com/user-attachments/assets/d1b2162b-6a7f-4e9b-aa15-3c6775cb18d7)
```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```
![image](https://github.com/user-attachments/assets/84a0b2fc-9668-4c3d-9f2f-589456fa0550)
```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/user-attachments/assets/8e0c72d7-1254-47a7-95f9-0ede15c246a3)
```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```
![image](https://github.com/user-attachments/assets/626f623f-5f95-405c-8779-b3ded444f57a)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/eec6bab0-c59c-4819-ba4f-5edc18e6cea6)
```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```
![image](https://github.com/user-attachments/assets/56a50a98-0f7f-4aa9-913e-8247288ee8a5)
```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![image](https://github.com/user-attachments/assets/483f3a13-6687-44b3-8fd8-6386d5dceaf2)
```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![image](https://github.com/user-attachments/assets/ed6cf6ef-859c-4610-a43f-1a2b3e33be15)
```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/8a57d67b-33e6-45e3-8c60-b82896a6fc1b)
```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![image](https://github.com/user-attachments/assets/d565210f-6d6b-4f3a-98cf-64c5cff502c4)























# Result:
 Include your result here
