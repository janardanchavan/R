# Day - Apr 04, 2020
#### Normal Distribution
Normal distribution is  also called as symmetrical distribution.
* Bell shaped curve
* 50% data lies at the left of virticle line i.e. Mean and 50% data lies at the right of virticle line
* any normal distribution/random variable value takes values between -infinity to +infinity <br/>
   i.e. anything that occurs naturally on this plannet would be always between -infinity to +infinity
* the probability that a normal random variable X <strong>equals</strong> any particular value is 0
* The total area under the normal curve is equal to 1

Probability formula: P() = I.E. / Total Events

The probability associated with any single random variable is always 0, because we are interested in only one random event.
Ex. What is the probability of the climate of being 25.6 degree => 0%.

Standard Normal Distribution:
* A Normal Distribution with a mean of 0 and a standard deviation of 1 is called as Standard Normal Distribution.
* Any x value can be transformed into  a z-score by using the formula `Z = (Value - Mean) / (Standard Deviation) = (x-µ) / σ

Example data:


| | Emp No | Salary | Work Exp. |
| --- | --- | --- | --- |
| | 123 | 450000 | 2 |
| | 314 | 650000 | 3.5 |
| | 423 | 850000 | 5.3 |
| Mean | | | |
| Standard Deviation | | | |

Why Standard distribution?
* to make the data unitless
* to resolve scalling issue

The process of converting normal distributed data to standard distributed data is called as `Standardization` or `Normalization`.

#### Calculating Probability from Z distribution
Lifespan of a person can be reasonably modelled using a normal distribution
Ex. What is the probability of a person leaving greater than 75 years provided average year is 72 years.
- µ = 72 years and σ = 6 years

What is P(x >= 75)

Step 1: Calculate Z score corresponding to 75
- Z = (75 - 72) / 6 = 0.5

Step 2: Calculate the probabilities using Z-Table (use z-table.com site)
- P(Z <= 0.5) = 0.6915

```
We know that the probability P(X > 75) is equal  to 1-P(X<=75), so we can use a table to find (P(X<=75). This result is equal to P(Z<=0.5) (where Z is the standardized random variable). The table state that P(Z<=0.5)=0.6915
```

Now we can calculate P(X > 75):
```
= P(X>75)
= 1-P(X<=0.75)
= 1-P(X<=0.5)
= 1-0.6915
= 0.3085
```

Assignments - Probability Distribution

Q1. The final exam scores in a statistics class were normally distributed  with a mean of 58 and a standard deviation of 4. Find the probability that a randomly selected student scored more than 62 in the class.

Q2. The final exam scores in a statistics class were  normally distributed with a mean of 58 and a standard deviation of 4. Find the probability that a randomly selected student scored less than 62 in the exam.

Q3. A normally distibuted random variable X has a mean of 20 and a standard deviation of 4. Determine the probability that a randomly selected x-value is between 15 and 22.







<hr/>
```js
  import { Component } from '@angular/core';
  import { MovieService } from './services/movie.service';

  @Component({
    selector: 'app-root',
    templateUrl: './app.component.html',
    styleUrls: ['./app.component.css'],
    providers: [ MovieService ]
  })
  export class AppComponent {
    title = 'app works!';
  }
```
