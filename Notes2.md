# Day6 - Mar 27, 2020

### Measures of Dispersion
#### 2nd moment of Business decisions

disperse means spread
dispersion - measure of dispersion / measure of variations

The mean, median or mode is usually not by itself a sufficient measure to reveal the shape of adistribution of a data set. 
We also need a measure that can provide some information about the variation among data set values.

The measures that help us to know about the spread of a data set are called `measures of` dispersion.

The measures of central tendency and dispersion taken together give a better picture of a data set.

We consider 3 measures of dispersion:
1. Range
2. Variance
3. Standard Deviation

#### 1. Variance - The measure of variation among the datapoints is called as variance.
Example: X1=1, X2=2, X3=3,     Mean=3
| Population Variance formula | Sample Variance formula |
| --- | --- |
| <img src="https://latex.codecogs.com/svg.latex?\sigma^2=\frac{\displaystyle\sum_{i=1}^{N}(x_i-\mu)^2}{N}"/> <br/> N = number of items in the population | <img src="https://latex.codecogs.com/svg.latex?s^2=\frac{\displaystyle\sum_{i=1}^{n-1}(x_i-\overline{x})^2}{n-1}"/>  <br/> n = number of items in the population |
|=((x-2)^2+(2-2)^+(3-2)^2) / 3| --- |
|=((-1)^2+(0)^2+(1)^2) / 3| --- |
|=(1+0+1) / 3| --- |
|=2/3| --- |
| Population Standard Deviation formula | Sample Standard Deviation formula |
| <img src="https://latex.codecogs.com/svg.latex?\sigma=\sqrt{\frac{\displaystyle\sum_{i=1}^{N}(x_i-\mu)^2}{N}}"/>  | <img src="https://latex.codecogs.com/svg.latex?s=\sqrt{\frac{\displaystyle\sum_{i=1}^{n-1}(x_i-\overline{x})^2}{n-1}}"/>   |


Population variation is always denoted by Greek notation - \sigma^2  `sigma square` <br/>
Sample variation is always denoted by English notaton - \s^2 `s square`

Formula for Population variable: 

#### 2. Standard Deviation <br/>

a. Popular Standard deviation (alpha) -> square root  of  variance <br/>
b. Sample standard deviation (s) -> square root of sample variance

#### 3. Range
Difference between maximum number - minimum number <br/>

### Graphical techniques
#### Bar Chart
#### Histogram
A Histogram represents the frequency distribution, i.e. how many observatons take the value within a certain nterval.
Eg. Heights of Black Cherry Trees
#### Pie Chart
2-5 data points
#### Line Chart
50 data points

# Day7 - Mar 28, 2020

### Skewness
#### 3rd moment of Business decisions
Skewness is asymmetry in a statistical distribution, in which the curve appears distrted or skewed eitehr to the left or to the right.
Formula to calculate Manually : <img src="https://latex.codecogs.com/svg.latex?\sum{[(x-\mu/\sigma)]}^3"/>
 
Plotting histogram:
  ```window()```
  ```hist(gmat)```
showing skewness : install moments package
  ```install.library('moments')```
  ```skewness(gmat)```
  ```skewness(workex)```
  
Calculating kurtosis:
  ```kurtosis(gmat)```
  ```kurtosis(workex)```

Plotting barplot
  ```barplot(workex)```
  
Plotting boxplot
  ```boxplot(gmat)```

<strong>How do you calculate outlier in the boxplot?</strong>
 

# Day - Apr 03, 2020
### Python
pandas - for data Manipulation
`import pandas as pd`

numpy - for Numerical operations
`import numpy as np`

matplotlib.pyplot - for Graphs
`import matplotlib.pyplot as plt`

opening file and saving in a variable
`x = pd.read_csv("C:\\New Volume\\Downloads\\mba.csv")

showing records
 ```
 x
 x.head()
 x.head(20)
 x.tail()
 x.tail(20)
 x.columns
 x.describe()
  
 x.gmat.mean()
 x['gmat'].mean()
 
 x.gamt.median()
 x.gmat.mode()
 ```
 mode will show records with index.<br/>
 
 2nd moment of business decision
 ```
 x.gmat.var()
 x.gmat.std()
 range = x.gmat.max() - x.gmat.min()
 range
 x.gmat.skew()
 x.gmat.kurt()
 ```
 Plotting graphs:
 ```
 plt.hist(x.gmat)
 plt.show()             # add this line to ignore junk values

 plt.boxplot
 plt.show()
 ```
 <strong>How to plot the bar graph?</strong>
 Box
 * IQR
 * Lower Outliers = Q1 - (1.5)(IQR)
 * Upper Outliers = Q3 + (1.5)(IQR)
 
 
 
 
 
   

  



