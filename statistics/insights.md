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

## Mean

**WHAT IT IS -**  
Average of all values; gives a central number.  
Sensitive to extremes, so one outlier can shift it a lot.  

**FORMULA -**  
Mean = Σx / n  
Add all values and divide by total count.  

**BUSINESS INSIGHT -**  
Mean can hide real segments in skewed data.  
Always ask: “Is this average representing most users or just extremes?”  

**REAL EXAMPLE -**  
Avg spend ₹2000 but most users spend ₹300–₹500.  
Strategy based on mean will fail majority users.  

**WATCH OUT FOR -**  
Misleading when outliers exist.  
Always pair with median or distribution.  


## Weighted Mean

**WHAT IT IS -**  
Average where some values matter more.  
Reflects real contribution instead of equal treatment.  

**FORMULA -**  
Σ(x·w) / Σw  

**BUSINESS INSIGHT -**  
Critical when volumes differ (revenue, traffic).  
Prevents wrong decisions from simple averages.  

**REAL EXAMPLE -**  
100 low-value users vs 1 high-value user.  
Weighted mean reflects true business impact.  

**WATCH OUT FOR -**  
Wrong weights = wrong insights.  


## Trimmed Mean

**WHAT IT IS -**  
Mean after removing extreme values.  
Focuses on core data.  

**FORMULA -**  
Remove top & bottom %, then compute mean.  

**BUSINESS INSIGHT -**  
Useful when outliers are noise.  
But dangerous if outliers are actual business signals.  

**REAL EXAMPLE -**  
Removing rare latency spikes to see normal performance.  

**WATCH OUT FOR -**  
Always ask: “Are outliers noise or signal?”  


## Median

**WHAT IT IS -**  
Middle value in sorted data.  
Represents the typical user.  

**FORMULA -**  
Odd → middle  
Even → average of two middle  

**BUSINESS INSIGHT -**  
Best for skewed data and real user experience.  
More reliable than mean in most real-world cases.  

**REAL EXAMPLE -**  
Median salary shows what most people earn.  

**WATCH OUT FOR -**  
Ignores extreme values completely.  


## Outliers

**WHAT IT IS -**  
Values far from the rest of data.  
Can be errors or key insights.  

**FORMULA -**  
< Q1 − 1.5×IQR or > Q3 + 1.5×IQR  

**BUSINESS INSIGHT -**  
Outliers often contain highest value insights (VIP users, fraud).  
Removing them blindly = losing business intelligence.  

**REAL EXAMPLE -**  
Top 1% users driving huge revenue.  

**WATCH OUT FOR -**  
Always investigate before removing.  


## Robust Estimates

**WHAT IT IS -**  
Metrics not affected much by outliers.  
Examples: median, IQR, MAD.  

**FORMULA -**  
Depends on metric.  

**BUSINESS INSIGHT -**  
Better for messy real-world data.  
Provides stable insights when data is skewed.  

**REAL EXAMPLE -**  
Median income instead of mean income.  

**WATCH OUT FOR -**  
Can hide extreme but important behavior.  


## Variance

**WHAT IT IS -**  
Measures spread using squared differences from mean.  
Captures overall variability.  

**FORMULA -**  
Σ(x − x̄)² / (n−1)  

**BUSINESS INSIGHT -**  
High variance = unpredictability and risk.  
Same average ≠ same stability.  

**REAL EXAMPLE -**  
Two stores same avg sales, one fluctuates heavily.  

**WATCH OUT FOR -**  
Hard to interpret (squared units).  


## Standard Deviation

**WHAT IT IS -**  
Square root of variance; average distance from mean.  
Most practical measure of consistency.  

**FORMULA -**  
SD = √Variance  

**BUSINESS INSIGHT -**  
Tells reliability of a metric.  
Same mean + different SD = different risk levels.  

**REAL EXAMPLE -**  
Delivery time same avg, but one is consistent.  

**WATCH OUT FOR -**  
Sensitive to outliers.  


## Mean Absolute Deviation

**WHAT IT IS -**  
Average of absolute differences from mean.  
Simple and intuitive spread measure.  

**FORMULA -**  
Σ|x − x̄| / n  

**BUSINESS INSIGHT -**  
Easy to explain to stakeholders.  

**REAL EXAMPLE -**  
Avg delivery varies by ~8 mins.  

**WATCH OUT FOR -**  
Less used in advanced modeling.  


## Median Absolute Deviation

**WHAT IT IS -**  
Median of absolute differences from median.  
Robust variability measure.  

**FORMULA -**  
median(|x − median|)  

**BUSINESS INSIGHT -**  
Best for skewed data with outliers.  

**REAL EXAMPLE -**  
Income distribution analysis.  

**WATCH OUT FOR -**  
Less common in dashboards.  


## Range

**WHAT IT IS -**  
Difference between max and min values.  
Simplest spread measure.  

**FORMULA -**  
Max − Min  

**BUSINESS INSIGHT -**  
Shows extreme limits, not typical behavior.  

**REAL EXAMPLE -**  
Delivery: 10 mins to 2 hours.  

**WATCH OUT FOR -**  
Driven entirely by outliers.  


## Percentiles

**WHAT IT IS -**  
Value below which a % of data lies.  
Shows position in distribution.  

**FORMULA -**  
Based on sorted data.  

**BUSINESS INSIGHT -**  
Enables segmentation (top users, bottom users).  
More actionable than averages.  

**REAL EXAMPLE -**  
Top 10% users drive most revenue.  

**WATCH OUT FOR -**  
Different tools compute slightly differently.  


## Interquartile Range (IQR)

**WHAT IT IS -**  
Spread of middle 50% of data.  
Ignores extreme values.  

**FORMULA -**  
IQR = Q3 − Q1  

**BUSINESS INSIGHT -**  
Shows true variability of typical users.  
Very useful for detecting outliers and stable patterns.  

**REAL EXAMPLE -**  
Most users spend ₹500–₹1500 → IQR captures this.  

**WATCH OUT FOR -**  
Ignores extremes completely.  

