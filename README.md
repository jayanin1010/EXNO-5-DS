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


    x=[1,2,3]
    y=[4,5,6]
    plt.plot(x,y,color='y')
    plt.title('line')
    plt.show()


<img width="632" height="490" alt="image" src="https://github.com/user-attachments/assets/a2655c53-c99c-4426-8f29-6f3e04dc950d" />



    x1=[1,2,3]
    y1=[4,5,6]
    plt.plot(x1,y1)
    x2=[1,2,3]
    y2=[7,8,9]
    plt.plot(x2,y2)
    plt.title('multi-line')
    plt.show()



<img width="651" height="506" alt="image" src="https://github.com/user-attachments/assets/074e554d-d63b-4f85-b21c-85b348770951" />

    x=[1,2,3,4,5,6]
    y=[2,4,6,8,10,12]
    plt.plot(x,y,color='y',linestyle='dotted',marker='o',markerfacecolor='r',markersize=10)
    plt.xlabel('x-axis')
    plt.ylabel('y-axis')
    plt.title('line')
    plt.show()


<img width="659" height="510" alt="image" src="https://github.com/user-attachments/assets/b253cae0-a3e3-474e-9e09-b0647d218d9e" />


    o=[2,4,6,7,9,35,37]
    a=[2,4,6,8,19,32,41]
    y=[2019,2020,2021,2022,2023,2024,2025]
    plt.plot(y,a,marker='o')
    plt.plot(y,o,marker='*')
    plt.title('crop yield')
    plt.xlabel('year')
    plt.ylabel('yield')
    plt.legend(['apples','oranges'])
    plt.show()


<img width="738" height="539" alt="image" src="https://github.com/user-attachments/assets/4daf248a-9aab-41fb-a199-f0242ae36b2d" />


    o=[2,4,6,7,9,35,37]
    a=[2,4,6,8,19,32,41]
    y=[2019,2020,2021,2022,2023,2024,2025]
    plt.bar(o,a)
    plt.plot(y,a,marker='o')
    plt.plot(y,o,marker='*')
    
    plt.legend(['apples','oranges'])
    plt.show()


<img width="701" height="482" alt="image" src="https://github.com/user-attachments/assets/342992b9-3bad-4a26-baae-d61cf69c11bd" />

    plt.figure(figsize=(10,4))
    plt.plot(y,o,marker='o',label='oranges')
    plt.title('oranges yield')
    plt.legend()
    plt.show()

<img width="1024" height="431" alt="image" src="https://github.com/user-attachments/assets/f1467a19-5467-408a-837f-d80bd8aefaea" />


    x=[1,2,3,4]
    y=[2,3,5,7]
    plt.scatter(x,y,label='star',color='r',marker='*',s=30)
    plt.title('scatter')
    plt.legend()
    plt.show()

<img width="690" height="516" alt="image" src="https://github.com/user-attachments/assets/8f0ae65f-725e-4aef-b2d8-048f3c79489e" />


    
    x=[1,2,3,4,5]
    y1=[10,12,14,16,18]
    y2=[5,7,9,11,13]
    y3=[2,4,6,8,10]
    plt.fill_between (x,y1, color='y', label='y1')
    plt.fill_between (x,y2, color='m', label='y2')
    plt.fill_between (x,y3, color='c', label='y3')
    plt.title("fill between")
    plt.legend()
    plt.show()


<img width="899" height="501" alt="image" src="https://github.com/user-attachments/assets/c67b63b3-cafb-43c8-9c1e-17ab76549978" />

    plt.stackplot(x,y1,y2,y3,colors=['c','m','y'])
    plt.legend(['y1','y2','y3'])
    plt.title('stackplot')
    plt.show()


<img width="747" height="504" alt="image" src="https://github.com/user-attachments/assets/38101be8-d6be-4e62-bd5e-4bc5223f6088" />

    from scipy.interpolate import make_interp_spline
    x=np.array ([1,2,3,4,5,6,7,8,9,10])
    y=np.array([2,4,5,7,8,9,10,11,12,13])
    spl=make_interp_spline(x,y)
    x_smooth=np.linspace (x.min(),x.max(),100)
    y_smooth=spl(x_smooth)
    plt.plot(x,y, 'o', label='data')
    plt.plot(x_smooth, y_smooth, '-', label='spline')
    plt.title('Spline interpolation')
    plt.legend()
    plt.show()


<img width="766" height="521" alt="image" src="https://github.com/user-attachments/assets/091433df-8ad5-4f63-b4a8-24b11f452b56" />

    vals=[1,3,5,6,7]
    lab=['a','b','c','d','e']
    plt.bar(lab,vals,color='b')
    plt.show()


<img width="854" height="491" alt="image" src="https://github.com/user-attachments/assets/cf1d684e-4908-4f73-beb8-9e13cb0100a4" />

    ages=[2,5,70,40,45,50,43,40,44,60,7,13,57,18,90, 77, 32,21,20,40]
    range1=(0,100)
    bins=10
    plt.hist (ages, bins, range1, color='y', histtype='bar', rwidth=0.8)
    plt.xlabel('ages')
    plt.ylabel('no.of people')
    plt.title('my histogram')
    plt.show()


<img width="1597" height="574" alt="image" src="https://github.com/user-attachments/assets/d4965973-6003-4848-98bc-2b543cade9a8" />

    x=[2,1,5,6,3,4,8,9,3,2,3,5]
    plt.hist(x,bins=6,alpha=0.5)
    plt.show()

<img width="823" height="476" alt="image" src="https://github.com/user-attachments/assets/ec9b43d8-9d08-4d7c-89ed-1091890c777b" />


    np.random.seed(0)
    data=np.random.normal(loc=0,scale=1,size=10)
    data


<img width="731" height="58" alt="image" src="https://github.com/user-attachments/assets/c7332f8c-f5fc-476f-8420-78eba7a32d4c" />

    fig,ax=plt.subplots()
    ax.boxplot(data)
    ax.set_xlabel('x-axis')
    ax.set_ylabel('y-axis')
    ax.set_title('boxplot')
    plt.show()


<img width="898" height="534" alt="image" src="https://github.com/user-attachments/assets/0791b894-8b96-4bd1-8c3c-269be3a21a1a" />


    activities=['eat', 'sleep', 'work', 'play']
    slices=[3,7,8,6]
    colors=['orange', 'y','m', 'c']
    plt.pie(slices, labels=activities, colors=colors, startangle=90, shadow=True, explode=(0,0,0.1,0), radius=1.2, autopct="X1.1")
    plt.legend()
    plt.show()


<img width="706" height="474" alt="image" src="https://github.com/user-attachments/assets/d2bd8a9c-1017-43d1-8638-79fcc70148f1" />


    labels='python', 'C+', 'ruby', 'java'
    sizes=[215,130,245,210]
    colors=['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
    explode=(0,0.4,0,0.5)
    plt.pie(sizes, explode=explode, colors=colors, labels=labels, autopct='% 1.1f%%', shadow=True)
    plt.axis('equal')
    plt.show()


<img width="789" height="467" alt="image" src="https://github.com/user-attachments/assets/522261c3-132d-4779-bbcf-1850182da2c4" />



# Result:
Thus all the data visualization techniques of matplotlib has been implemented
