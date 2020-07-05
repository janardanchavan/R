

## Apr 27, 2020

## Normal Probability Plot / Normal Distribution plot / Q-Q Plot / Symmetrical Curve

To identify if the data is distributed normally or not.  <br/>
If data points are around in a single diognal line, it means data is following normal distribution.

Plot vs Curve for normal distribution: <br/>
If someone asks to plot a normal distribution curve, draw it like a bell shaped graph. <br/>
If someone asks to plot a normal distribution plot, draw it like a scatter graph with line.

## Sampling variation

* Statistics vary from Sample to Sample due to randomness. <br/>
* A population of 1000,000 people has an average IQ of 100. <br/>
* Suppose if you take sample of 5 people will it be same as 100 or what you will get?

## Confidence Interval

* What is the Probability of a student scoring 65.5% in an Examination?
Probability is '0' (because probability associated with any single value is 0)

What does below line mean? <br/>
I am 95% confident that I will score 75% to 85% in an exam.

Note: <br/>
Z-Score for 95% confidence is 1.96<br/>
Z-Score for 90% confidence is 1.64 (1.64 / 1.65)<br/>
Z-Score for 99% confidence is 2.58 (2.57 / 2.575/ 2.58)<br/>

Case Study with respect to Credit Card: <br/>
* A Bank with 50,000 customers is thinking of offering a <br/>
new credit card to its all customers.

* Profitability of the card depends on the average balance <br/> 
maintained by the card holds.

* A Market research campaign is launched, in which about<br/>
200 customers accept the card in a promotional campaign.

* Average balance maintained by these is $1,650 and the<br/>
standard deviation is $1,987. Assume that the population<br/>
standard deviation is $1,500 from previous launches.

* What we can say about the average balance that will be <br/>
held after a full-fledged market launch?

Population = N = 50,000 <br/>
Sample = n = 200 <br/>
S.Mean = <img src="https://latex.codecogs.com/svg.latex?\overline{X}"/> = 1650 <br/>
S.SD = s = 1987 <br/>
P.SD = <img src="https://latex.codecogs.com/svg.latex?\sigma"/> = 1500 <br/>
what will be population mean? = <img src="https://latex.codecogs.com/svg.latex?\mu"/> = ??? <br/>

### Interval estimates of parameters
  
What do you think will happen if we take another random sample of 200 customers?

Because of this uncertainty, we prefer to provide the estimate as an interval (range) and associate<br/> a level of confidence with it.<br/><br/>
<strong>Interval = Point Estimate +- Margin of Error</strong>

Start by choosing a confidence level (1-\alpha)% (e.g. 95%, 99%, 90%)<br/>
(95% = (100 - 5%). 5% is nothing but alpha. alpha is the % of changes going wrong.<br/>

Then, the population mean will be with in

Xbar +- Z(x-alpha) sigma/sqrt(n) where Z(x-alpha) satisfies p(-Z(x-alpha) < Z <= Z(x-alpha)) = 1-alpha

* Based on the survey and Historical data

- n = 200; σ=$1500; Xbar=$1,650
- σ \base{x} = σ / sqrt(n) = 1,500 / sqrt(200)

* Construct a 95% confidence internval for the mean card balance and interpret it?

($1,442 to $1,858)

### What if we don't know Population Standard Deviation?

* Suppose that the customers of this bank are very different and hence population standard deviation from previous launches can not be used

We replace σ() with our best guess (point dstimate) s(S.SD), which is the standard deviation of the sample:<br/>
(Note that we cannot use Z-distribution, rather we go with T-distribution with n-1 degree of freedom)

<img src="https://latex.codecogs.com/svg.latex?s=\sqrt{\frac{\sum{(x-\overline{X})^2}}{n-1}}"/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="https://latex.codecogs.com/svg.latex?t=\frac{\overline{x}-\mu}{s/\sqrt{n}}"/><br/>

* If the underlying population is normally distributed, T is a random variable distributed<br/>
according to a t-distribution with n-1 degrees of freedom <img src="https://latex.codecogs.com/svg.latex?T_{n-1}"/>

<strong> this is complicated loophole topic in data science or statistical anlaysis.<br/>complicated statistical analysis</strong>

* Research has shown that the t-distribution is fairly robust to deviation of the population of the normal model.

### Student's t-distribution
T-distibution is also called as Student's t-distribution

### Confidence Interval for mean with unknown Sigma

<img src="https://latex.codecogs.com/svg.latex?\overline{X}{\pm}Z_{1-\alpha}\frac{\sigma}{\sqrt{n}},\:where\:z_{1-\alpha}\:satisfies\:P(-z_{1-\alpha}\:\leq\:Z\:\leq\:z_{1-\alpha})\:=\:1-\alpha"/>

changes to  below formula

<img src="https://latex.codecogs.com/svg.latex?\overline{X}{\pm}t_{1-\alpha,n-1}\frac{s}{\sqrt{n}},\:where\:t_{1-\alpha,n-1}\:satisfies\:P(-t_{1-\alpha,n-1}\:\leq\:T_{n-1}\:\leq\:t_{1-\alpha,n-1})\:=\:1-\alpha"/>









