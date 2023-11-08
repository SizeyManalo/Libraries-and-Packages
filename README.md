# Libraries-and-Packages
This code snippet demonstrates the use of Python libraries for data visualization and analysis, including Matplotlib, NumPy, and Pandas. The code begins by importing these essential libraries and packages. It then constructs a sample data frame from a dictionary containing information about individuals' names, ages, math marks, physics marks, and chemistry marks. With this data frame, the code showcases various plotting techniques, including bar plots, scatter plots, pie charts, and line plots, to visualize the physics marks of the individuals. It provides a practical illustration of how to utilize these libraries for data analysis and visualization, making it a useful reference for those working with Python in data-related tasks.

[ ]
#Library - matplotlib - pie chart, bar chart
#numpy - mathematicial operations
#pandas - analysis, manipulate data
#scipy - scientific computations
#seaborn - stats for visualization, based on matplotlib
[ ]
#import libraries and packages
import pandas as pd
import numpy as np
[ ]
import matplotlib.pyplot as plt

[ ]
# Dictionary - name,age,math_marks,physics_marks,chem_marks
data_dict = {"name":["Mikko","Steve","Mary"],
             "age":[32,23,24],
             "math_marks":[100,94,96],
             "physics_marks":[100,90,94],
             "chem_marks":[90,100,100]}
print(data_dict)
#Creating a data frame object (2D table)
df = pd.DataFrame(data_dict)
df.head()
account_circle

[ ]
#Bar Plot
df.plot(kind='bar',x='name',y='physics_marks',color='yellow')
plt.title('Barplot')
plt.show()
account_circle

[ ]
#Bar Plot
df.plot(kind='scatter',x='name',y='physics_marks',color='red')
plt.title('Scatterplot')
plt.show()
account_circle

[ ]
#Bar Plot
df.plot(kind='pie',x='name',y='physics_marks')
plt.title('Piechart')
plt.show()
account_circle

[ ]
df.plot(kind='line',x='name',y='physics_marks',color='red')
plt.title('lineplot')
plt.show()
account_circle

[ ]
