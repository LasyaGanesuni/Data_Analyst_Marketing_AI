## Histogram
<img width="922" height="334" alt="image" src="https://github.com/user-attachments/assets/3e357dfe-9fbe-4f8b-b7a2-d56b9ee157f1" />

**WHAT IT IS -**
A chart that groups data into bins 
and shows how many values fall into 
each bin. It reveals the shape of 
your data — not just a single number.

**FORMULA-**
No formula. It is a visual tool.
X axis = value ranges (bins)
Y axis = count or frequency of 
values in each bin.

**BUSINESS INSIGHT-**
A histogram shows me what the 
average hides — whether I have one 
type of customer or five, whether 
the data is normal or skewed, 
whether there is a small group of 
high-value outliers that a single 
number would completely erase.

**REAL EXAMPLE-**
Zalando average order value = £65.
Histogram reveals: 70% of orders 
are £10–£40 (bargain shoppers) and 
5% are £400–£600 (luxury buyers). 
These two groups need completely 
different marketing. The average 
made them invisible.

**WATCH OUT FOR-**
Bin size changes the story. Too 
wide = hides patterns. Too narrow = 
looks like noise. Always try 
multiple bin sizes before concluding 
anything.

[video](https://www.youtube.com/watch?v=qBigTkBLU6g&list=PLblh5JKOoLUK0FLuzwntyYI10UQFUhsY9)

## STATISTICAL DISTRIBUTIONS
<img width="1005" height="365" alt="image" src="https://github.com/user-attachments/assets/b0e6a1e1-aace-45e4-9f5f-346cecd2db98" />

**WHAT IT IS -**
A distribution describes the shape 
of data — where values tend to 
cluster, how spread out they are, 
and how probable each value is. 
Different types of data have 
different natural shapes.

**FORMULA-**
No single formula — depends on 
distribution type.
Normal distribution:
f(x) = (1/σ√2π) × e^(-(x-μ)²/2σ²)
μ = mean, σ = standard deviation.
(You do not need to memorise this —
just know what μ and σ control.)

**BUSINESS INSIGHT-**
Different business metrics have 
different shapes — assuming 
everything is normally distributed 
is how analysts give confident 
answers that are completely wrong.

**REAL EXAMPLE-**
Zalando average order value = £65.
Histogram reveals: 70% of orders 
are £10–£40 (bargain shoppers) and 
5% are £400–£600 (luxury buyers). 
These two groups need completely 
different marketing. The average 
made them invisible.

**WATCH OUT FOR-**
Email open rates are not normally 
distributed — they cluster near 
zero with a long right tail. If you 
run a t-test assuming normality on 
open rate data, your A/B test 
conclusion is wrong. At Booking.com 
running 25,000 tests a year, one 
wrong distributional assumption 
multiplied across thousands of tests 
is a serious problem.

**HISTOGRAM VS DISTRIBUTION CURVE-**
A histogram shows only what 
happened in your actual sample. 
A distribution curve estimates 
the probability of any value — 
including ones never observed — 
by fitting a smooth mathematical 
shape through your data.

**Histogram** = photograph of past data. Can only show values 
that actually occurred. Empty bin = nobody bought that, 
not impossible to buy that.

**Distribution curve** = estimate of probability across ALL 
values including unobserved ones. Fits a mathematical shape 
through your data and fills the gaps the histogram cannot.

**Why it matters**: when predicting future behaviour (churn, 
CLV, next purchase) you need probabilities for values you 
have never seen. The curve gives you that. The histogram 
cannot.

**The catch**: curve is only as good as the shape you assume. 
Wrong shape assumption = wrong probabilities. Always check 
if your data actually fits the distribution you are using.

One looks backward. One looks forward.


[video](https://www.youtube.com/watch?v=oI3hZJqXJuc)

## Population Parameters
<img width="974" height="257" alt="image" src="https://github.com/user-attachments/assets/38734cbb-03ec-459d-a1cb-5cc262336041" />

**WHAT IT IS -**
Population parameters are the true 
values that describe an entire 
population — the real mean, the 
real variance. We can almost never 
measure them directly because we 
never have data on every single 
person. We always estimate them 
from a sample.

**FORMULA-**
Population mean: μ = Σx / N
(sum of all values divided by 
total population size N)

Sample mean: x̄ = Σx / n
(sum of sample values divided 
by sample size n)

The difference: N is everyone.
n is just who you measured.

**BUSINESS INSIGHT-**
Population parameters are the true 
values we can never directly measure 
— every analysis we run is just an 
educated guess about them based on 
the sample we have, and if our 
sample is biased, our guess is wrong.

**REAL EXAMPLE-**
Zalando surveys 50,000 customers 
to understand the average European 
shopper. All 50,000 are loyal 
customers — casual shoppers and 
churned customers never responded. 
The sample mean they calculate 
describes their best customers, 
not the average shopper. Every 
strategy built on this number is 
wrong. They will not know it until 
the strategy fails.

**WATCH OUT FOR-**
Always ask: who is NOT in my 
sample? Biased samples produce 
biased parameters. The analysis 
can be technically perfect and 
still completely wrong because 
of who was excluded.
[video](https://www.youtube.com/watch?v=vikkiwjQqfU)

