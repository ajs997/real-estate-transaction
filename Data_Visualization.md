# -*- coding: utf-8 -*-
"""
Created on Mon Feb  4 11:38:26 2019

@author: aj-nok

about: Data Visualization using pandas,numpy,matplotlib

dataset: realesatatetransactions.csv
"""

CODE:
import pandas as pd
import numpy as np
import matplotlib.pyplot as mplt
import seaborn as sns

data=pd.read_csv("realestatetransactions.csv")
print(" BAR Graph between cities and their counts: ")
city_count=data['city'].value_counts()
city_count.plot(kind='bar')

OUTPUT:
BAR Graph between cities and their counts: 
![](city_vs_city_count.png)