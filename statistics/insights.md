## Histogram
<img width="922" height="334" alt="image" src="https://github.com/user-attachments/assets/3e357dfe-9fbe-4f8b-b7a2-d56b9ee157f1" />

A histogram shows me what the average hides — whether I have one type of customer or five, whether the data is normal or skewed, whether there is a small group of high-value outliers that a single number would completely erase.
[video](https://www.youtube.com/watch?v=qBigTkBLU6g&list=PLblh5JKOoLUK0FLuzwntyYI10UQFUhsY9)

## Histogram vs Distribution curve
<img width="1005" height="365" alt="image" src="https://github.com/user-attachments/assets/b0e6a1e1-aace-45e4-9f5f-346cecd2db98" />

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

The parameters that determine how a distribution fits the population data are called population parameters.
We never measure the full population — we always work 
with a sample. Population parameters (true mean, true 
variance) are what we are trying to estimate.

The dangerous assumption: that our sample looks like 
the full population. If the sample is biased — only 
loyal customers, only desktop users, only one country 
— every parameter we calculate is wrong, and every 
decision built on it is wrong too.

Real risk: Zalando surveying only loyal customers and 
treating the results as representative of all European 
shoppers. The sample does not represent the population. 
The strategy built on it will fail.
Always ask: who is NOT in my sample?
[video](https://www.youtube.com/watch?v=vikkiwjQqfU)

