# taller3.graficoBigotes
import numpy as np
import matplotlib.pyplot as plt 
import pandas as pd 


data = [np.random.normal(0, std, 200) for std in range(1, 4)]
data1 = [np.random.normal(1, std, 100) for std in range(2, 4)]
data2 = [np.random.normal(2, std, 100) for std in range(3, 4)]
data3 = [np.random.normal(3, std, 200) for std in range(0, 4)]
data4 = [np.random.normal(4, std, 100) for std in range(2, 7)]
data5 = [np.random.normal(5, std, 100) for std in range(0, 10)]
# boxplot rectangular 

plt.boxplot(data,vert=True,patch_artist=True);

fig, ax = plt.subplots(5, 2, sharey = True)

ax[0, 0].boxplot(data,vert=True,patch_artist=True)
ax[1, 0].boxplot(data1,vert=True,patch_artist=True)
ax[2, 0].boxplot(data2,vert=True,patch_artist=True)
ax[3, 0].boxplot(data3,vert=True,patch_artist=True)
ax[4, 0].boxplot(data4,vert=True,patch_artist=True)
ax[1, 1].boxplot(data5,vert=True,patch_artist=True)
ax[0, 1].boxplot(data1,vert=True,patch_artist=True)
ax[2, 1].boxplot(data3,vert=True,patch_artist=True)
ax[3, 1].boxplot(data4,vert=True,patch_artist=True)
ax[4, 1].boxplot(data5,vert=True,patch_artist=True)
