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

    import matplotlib.pyplot as plt
    import numpy as np
    import pandas as pd
    
    x=[2018,2019,2020,2021,2022]
    y=[15000,20000,25000,30000,35000]
    plt.plot(x,y,'*',linestyle='dashed',linewidth=2,markersize=8)
    plt.xlabel('x-axis')
    plt.ylabel('y-axis')
    plt.title('2D diagram')
    plt.show()

<img width="696" height="530" alt="image" src="https://github.com/user-attachments/assets/51a2c14f-1cfc-45b7-99ba-cb85ef232a05" />


    plt.subplot(2,2,1)
    plt.plot(x,y,'r--')
    
    plt.subplot(2,2,2)
    plt.plot(x,y,'g--')
    
    plt.subplot(2,2,3)
    plt.plot(x,y,'bo')
    
    plt.subplot(2,2,4)
    plt.plot(x,y,'mo')


<img width="747" height="498" alt="image" src="https://github.com/user-attachments/assets/b77c0616-a0e8-4360-9298-2ae5fc87b749" />

    x=np.arange(0,4*np.pi,0.1)
    y=np.sin(x)
    plt.title('sine')
    plt.plot(x,y)
    plt.show()

<img width="786" height="504" alt="image" src="https://github.com/user-attachments/assets/e4104619-c3ff-4145-851f-1f382d3e14f9" />


    x=[2,4,6]
    y=[3,5,7]
    x1=[8,10,12]
    y1=[9,11,13]
    plt.bar(x,y,color='c')
    plt.bar(x1,y1,color='m')
    plt.show()


<img width="725" height="475" alt="image" src="https://github.com/user-attachments/assets/425f4378-3637-407a-bc4c-beea82323fb6" />






# Result:
Thus all the data visualization techniques of matplotlib has been implemented
