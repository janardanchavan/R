# Scatter Plot
1. Scatter diagrams or plots  provide a graphical representation of the relationship of two continuous variables.
2. <strong>Be Careful - </strong>Correlation is not cause and effect relationship.(\sum{xy})
3. Judge strength of relationship by width and tightness of scatter.

### Positive Correlation
If x increases y also increases, it is called as positive correlation.
1. Strong Positive Correlation - If dots are tightly bounded to the straight line.
2. Moderate Positive Correlation - Data points are slightly loosly scattered.
3. Poor Positive Correlation - Data is still slightly loosly scattered.

### Negative Correlation
If x increases y reduces, it is called as negative correlation.
1. Strong Negative Correlation - If dots are tightly bounded to the straight line.
2. Moderate Negative Correlation - Data points are slightly loosly scattered.
3. Poor Negative Correlation - Data is still slightly loosly scattered.

### No Correlation
If x and y are highly scattered, it is called as no correlation.

# Correlation Analysis
Correlation Analysis measures the  degree of linear relationship between two variables.<br/>
It is denoted by small 'r' and called as `correlation coefficient`<br/>
* Range of correlation coefficient (-1 to 1)
* Perfect positive relationship (+1)
* Perfect negative relationship (-1)
* No Linear relationship (0)

If the absolute value of the correlation coefficient is greater than 0.85, then we say there is a good relationship.<br/>
If the r value is > +0.85, it is called as strong positive relationship<br/>
If the r value is > -0.85, it is called as strong negative relationship
* Example: r = 0.87, r = -0.9, r-0.9, r=0.9, r=-0.87 describe good relationship

If the r value is between 0.65 to 0.85, it is called as Moderate Positive correlation or Average Positive correlation.
If the r value is between -0.65 to -0.85, it is called as Moderate Negative correlation or Average Negative correlation.

If  the r value is less than 0.65, then it is called as Poor Positive correlation.
If  the r value is less than -0.65, then it is called as Poor Negative Correlation.
* Example: r = 0.5, r = -0.5, r = 0.28 describe poor relationship

<img src="https://latex.codecogs.com/svg.latex?r=\frac{n(\sum{xy})-(\sum{x})(\sum{y})}{\sqrt{[n\sum{x}^2-(\sum{x})^2][n\sum{y}^2-(\sum{y})^2]}}"/>
|X|Y|
|---|---|
|1|2|
|2|3|
|3|4|

Points to remember:
- n = number of records
- sum(x*y) - (sum(x)*sum(y)) i.e. 3(20) - (6)(9)
- x square and x whole square

# Linear Regression Model - first prediction algorithm
<b>Linear regression Model is the equation that represent how an independent variable is related to a dependent variable.</b>

equation of straight line = y=mx+c
m=slope
c=interception / constant
x=independent variable

Equation of regression: y = ß0 + ß1x + ε <br/>
<img src="https://latex.codecogs.com/svg.latex?y=\beta_0\:+\:\beta_1{x}+\varepsilon"/>
Beta not, Beta1 and epsilon/small e
independent variable x is related to dependent variable y.

<b>Error term is a regression model.</b><br/>
ε(epsilon) = an error.
ß0(beta 1) = Intercept
ß1(beta 1) = slope
x = input / independent variable
ß0 and ß1 together are called as <b>parameters of the model</b> or <b>coefficients of the model</b> or <b>estimates of the model</b>. 

ε is a random variable called error = actual value - predicted value.

What is regression equation?<br/>
Regression equation and Linear regression equation both are same.

<img src="https://latex.codecogs.com/svg.latex?\beta_0=\frac{(\sum{y})(\sum{x^2})-(\sum{x})(\sum{xy})}{n(\sum{x^2})-(\sum{x})^2}"/>

<img src="https://latex.codecogs.com/svg.latex?\beta_1=\frac{n(\sum{xy})-(\sum{x})(\sum{y})}{n(\sum{x^2})-(\sum{x})^2}"/>






