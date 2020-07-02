# R Learning notes:

## Day1 - Mar 19, 2020
Data Science (Business Analytics)
* Business + Statistics (Basic + Advanced) + Technical (last preference i.e. R/Python)
* Statistics (Basic + Advanced)  + ML (Prediction Algorithms) + R & Python
* apart from Communication and Common Sense

Outline & Content Basic Statistics

1. Preliminary Data types

A. Data Types - Continuous, Discrete, 
B. Data Types - Nominal, Ordinal, Interval, Ratio

Continuous - Decimal format with some meaning, eg. height as 6.1 ft., weight 75.3 kg, petrol price 72.15 p/l, temp in bangalore 25.2 degree, 
Descrete - Decimal format that does not have any meaning (decimal numbers not considered) i.e. does not have decimal places, eg. 1.2 laptops, 2.83 bikes does not makes any sense.
     In other words, whole numbers with meaning - 1, 2  or 3 laptops, 2, 3 bikes, 2 or 20 children, 100, 200 employees in office
		   descrete data example:
		   non-numerical data:
			 Collor: (Red, Blue, yellow); gender (M, F, M, F)
## Day2 - Mar 20, 2020
          a: Nominal: labeling variables without any quantitative values: Raj, Delhi, London, New Jersey
          b: Ordinal/direction: measures of non-numeric concepts like satisfaction, happiness, discomfort, etc.: 
                 eg. Raj is a good boy, I don't like Delhi, Tiger is a wild animal.
          c: Interval (score out of whole / range): Conveys relative magnitude with addition to direction: 
                 eg: I rate Delhi 3 and goa 2 on a scale of 5
          d: Ratio: conveys information on exact absolute value/scale, no upper or lower scale: eg: I paid Rs. 25500 for laptop.
     2. Random Variable, Probability, Probability Distribution
     3. Central Tendency, Dispersion, Long Tail & Peakedness
     4. Graphical representation
     5. Hypothesis


## Day3 - Mar 24, 2020
1. Random Variable: In probability adn statistics, a random variable, random quanity, aleatory variable, or stochastic variable whose possible value are outcomes of a random phenomenon

    Variable - It's a symbolic name associated with a value and whose associated value may be changed.
    Random - It is random because there is some chance associated with each possible values. Total should be 100%.
       I can call any student's name out of total 7 students -> 1/7 i.e. 0.14 or 14%
       Toss = head or tail = 1/2 i.e. 0.5 or 50%.
       Dice = 1, 2, 3, 4, 5, 6 = 1/6, i.e. 0.1666 or 16.66%

Probability formula = interested events / total number of events
  P(H) in head or tail = 1/2 i.e. 50%
  P(3) in Dice = 3/6 i.e. 1/6 i.e. 16.66%
  probability of date 1 in a year : 12/365
  probability of date 30 in a year : 11/365
  probability of getting 3 in dice: P(>3) = 4, 5, 6 = 3/6 = 0.5 = 50%

### Probability Distribution:
   always between 0 to 1
   sums up to 100

Random variables plotted on x axis and probability associated with these random variables plotted on y axis is called as probability distribution.

X	P(X)
0	0.20
1	0.30
2	0.25
3	0.20
4	0.05

1. What is the probability of a sale?
2. What is the probability of selling only one product?
3. What is the probability of selling atleast two products?

### Sampling theory
Population vs Random sample data
Population data is always large which is economically costlier to handle.
 eg. survey of all the citizons will require lots of manpower.
In telecom, how many calls are generated, it's a huge data. for anlaysis we will consider some sample data only.

If working on population data, the accuracy should be very much high.

## Day4 - Mar 25, 2020
Measures of Central Tendency: First moment of Business Decisions
Find the center of the numbers: Mean / Median / Mode / Outliers

### Mean/Average

 -> 1, 2, 3, 4, 5 : average=3
 -> 1, 2, 3, 4, 700 : average=142


Omkar		Shiva		Vatsal
(1 YR)		(6 YRS)		(15 YRS)
4 Lacs		8 Lacs		20 Lacs

Avg 20%

80 K		160 K		4 Lacs
				3% = 60K
		7% = 56K
50% = 2 Lacs

50% + 7% + 3% = 60%/3 = 20%

Mean or Average is affected by Outliers.

### Median (data will be sorted before applying)

	1		1
	2     Mean = 3	2
	3     		3
	4     Median = 3	4
	5		700
1, 2, 3, 4, 5
Mean = 3
Median = 3

1, 2, 3, 4, 700
Mean = 142
Median = 3

1, 2, 700, 3, 4
Mean = 142
Median = 3

1, 2, 3, 4, 5, 6
Median = (3+4)/2 = 3.5

### Mode -> most occurence/common/popular value in the dataset
{Grapes, Apple, Orange, Orange}			: Orange
{Grapes, Apple, Apple, Orange, Orange}			: Apple, Orange
{Watermelon, Grapes, Apple, Apple, Orange, Orange, Grapes}	: Grapes, Apple, Orange

1 mode  -> Unimode
2 modes -> Bimode
3 modes -> Multimode

Outlier => much bigger or smaller than the rest of the numbers

Population parameters are denoted by Greek notations	
Sample 	 parameters are denoted by English notatoins 	X bar

Population parameter = (mue)
meu = population mean / population average
N = number of items in the population

Sample parameter = X bar
n = number of items in the sample

### Measures of Dispersion : 2nd moment of business decision
The measures that help us to know about the spread of a data set are called measures of dispersion.

The measures 


# Day5: Mar 26 -> Using Rstudio
Clear Console -> Ctrl + L
packages - same as libraries in other programming languages
Installing packages - Tools -> Install Packages
   1. Enter name of the package to be installed eg. animation
   2. Select "Install dependencies" check box.
To view the installed packages, select packages tab (bottom-right section of the screen)
   enter package name in the search name box. This will show the packages containing given package name.
To use the package in our program select the check mark

Installing Package - Click the install button on the Package tab itself.
   1. Enter name of the package to be installed eg. moments
   2. Select "Install dependencies" check box.

Installing packages from editor window, eg.:<br/>
   ```install.packages('moments')```

if we de-select the check-box, we'll not be able to use it in our program called detaching package.

detaching package from editor window:<br/>
   ```detach("packagae:moments", unload = True)```

help on packages/function name etc.:
   On the Help tab: enter the package  or function name eg. mean in the search box.

Reading csv file:
   On the Environment tab, click import dataset button.
from editor window:<br/>
   ```x <- read.csv("cars.csv'")```

Show the dataset details -> Import Text (base)...<br/>
   ```View(x)```

to check rows and columns in the dataset:<br/>
   ```dim(x)```

to display initial records in the dataset (by default 6 records):<br/>
   ```head(x)```

to display first 3 records:<br/>
  ```head(x, 3)```

to display last records (default 6 records):<br/>
  ```tail(x)```

to display last 3 records:<br/>
  ```tail(x, 6)```

to display all the column names in the dataset<br/>
  ```colnames(x)```

to print average/mean of HP column (column names are case-sensitive):<br/>
  ```mean(x$HP)```

to print median:<br/>
  ``` median(x$HP)```

to avoid using dataset name each time:<br/>
```
attach(x)
mean(HP)
```
to display most occuring value:<br/>
  we need additional library 'LaplacesDemon' to display mode values:<br/>
  ```install.packages('LaplacesDemon')```
  then select the package on the Packages tab.
  ```Mode(HP)```

to display summary of all the column together<br/>
  ```summary(x)```

Create an account on rpubs.com -> whatever you type, you can publish on rpubs.com


  
