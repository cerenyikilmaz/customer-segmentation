# Customer-Segmentation-with-Python
This is my bachelor thesis! I used Python for Customer Segmentation with RFM Analysis. 

-----------------------------------------------------------------------------------------------------------------------------------------------------

This study was created to examine the results to be obtained from the RFM method used in customer segmentation. In this day and age when e-commerce is important, customer loss analysis is one of the sine qua non of this industry. Today's business strategies have prioritized knowing the customer best and determining how to approach the customer. At the same time, data mining, which gives each customer personal access with its features, has become one of the most important tools.
As part of this study, we segmented customers using data from an e-commerce company and analyzed the results.

-----------------------------------------------------------------------------------------------------------------------------------------------------
In our analysis, we used sales data from an e-commerce website for 2021.
We performed our analysis on Jupyter Notebook using Python language. We used the RFM method to segment customers.

-----------------------------------------------------------------------------------------------------------------------------------------------------
We used some libraries in Python to load the dataset, do the analysis and visualize the data. Their names and brief definitions are as follows;

```diff
@@ import pandas @@ 
```
Operations such as reading data, preprocessing, and cleaning are performed with this library.
```diff
@@ import numpy as np @@
```
The Pandas library, which allows us to work with multidimensional arrays and matrices, is also used to perform mathematical operations.
```diff
@@ import datetime as dt @@
```
It's a module that puts at our disposal different functions to work with time, time and date.
```diff
@@ import glob @@
```
It's a module that allows us to list and use specific files in a folder in Python. We used this to import 12 separate CSV files created for 12 months as a single dataframe.
```diff
@@ import os @@
```
It's a module that allows us to work with files and directories with ease.
```diff
@@ from pathlib import Path @@
```
It's a library used to manipulate text files.
```diff
@@ import matplotlib.pyplot as plt @@
```
It's a library that allows us to visualize data through 2 or 3 dimensional drawings.
```diff
@@ import seaborn as sns @@
```
It is a library mainly used for statistical visualizations.
```diff
@@ import squareify @@
```
It is the library that we can use to create treemaps.
```diff
@@ import hashlib @@
```
It is the library used to run various encryption algorithms.
