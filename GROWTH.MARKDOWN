There are three main ways of estimating growth rates:

1. **Based on historical rates**: A strong indicator of long term trend is the past performance. Although, the past isn’t always indicative of the future, it is a good starting point for growth estimation.

2. **Based on analysts’ estimates**: Analysts generally have a good understanding of the companies they follow, and their estimates tend to be reflective of upcoming events impacting companies’ cash flows.

3. **Based on fundamentals**:  Ultimately, all earnings growth can be traced back to how much the firm is reinvesting (i.e. retention ratio) and what return it yields (i.e. ROE).

**Growth Based on Historical Rates**

If a company has no analyst estimates, but it has a sufficient track record, we use its historical growth to project future figures. Past line items, such as earnings, are plotted as below with a line of best-fit running through each equally-weighted point, with a minimum of 3 years. The slope, or gradient, of this line is divided by the average of the absolute values to compute the annual growth rate for earnings. Absolute values allow us to calculate a growth rate even when earnings are negative or are expected to become positive.

For example, Apple’s past earnings annual growth rate is 17.13% year-on-year, which is calculated by:

```
Annual past earnings growth rate = Line of Best Fit Slope / Average of Absolute Earnings (2011-2018)
				   = 7.44 / 43.43B
			     	   = 17.13%  
```


**Growth Based on Analyst Estimates**

If a company has analyst coverage, we use the consensus of their estimates to calculate its future growth rate. Similar to the calculation above, we plot the line of best-fit through each earnings estimate to determine the slope, and therefore the growth rate. However, instead of using equal-weighting for each data point, the years with more analyst coverage have higher weighting, which means we place more importance on estimates with 20 analysts’ forecasts compared to ones with only a few. The first data point is taken from the most recent earnings release and given a weight of one.

For example, Apple’s future earnings annual growth rate is 4.4% year-on-year, which is calculated by:

```
Annual future earnings growth rate = Line of Best Fit Slope / Average of Absolute Earnings (2018-2023)
				   = 2.66 / 60.56B
			     	   = 4.40%  
```
|Year              |Mar-18|Sep-18|Sep-19|Sep-20|Sep-21|Sep-22|
|------------------|------|------|------|------|------|------|
|Earnings (US$, B) |53.32 |57.75 |61.84 |63.58 |62.01 |64.85 |
|Analysts          |Actual|  35  |  38  |  14  |   2  |   2  |

***Note on negative earnings***: when the first period of earnings is negative, the growth rate cannot be estimated. To overcome this, we use the absolute value of earnings to calculate the growth rate. For annualized growth rates (i.e. on average, how much will Apple growth year-on-year over the next few years?) we will still show this rate, but the subject company will not be able to pass some of the growth checks if earnings are negative. For single point-in-time growth rates (i.e. how much will Apple grow in the upcoming year?), we will not compute the growth rate at all is earnings start off as negative.

**Growth Based on Fundamentals**

For companies with no analyst forecast and insufficient historical track record, we use the fundamental Return on Equity (ROE) method to calculate future earnings growth rates. Damodaran states that all earnings growth can be traced back to how much the firm is reinvesting (i.e. retention ratio) and what returns it yield (i.e. ROE).

We linearly interpolated the subject company’s current ROE towards its industry median ROE over a 5-year period, with the underlying assumption that companies’ returns will, on average, converge to the industry level over time. High-returning companies should attract competition, which will reduce their returns. Low-returning companies should become more efficient in order to survive.

We apply this method to currently profitable companies as we do not want to impose the assumption that all loss-makers will become profitable over the next 5 years. We also focus on companies that reinvest (i.e. 0% <= payout ratio < 90%) and have positive shareholders’ equity. We determine the growth rate exactly the same way as the method above.
For example, HemaCare has a current ROE of 30.2% but its industry median ROE is 13.8%, so its ROE will incrementally fall towards the industry median. With a retention ratio of 100%, HemaCare retains all of its earnings which adds to its Equity position over time. Each year, earnings is calculated by rearranging the Return on Equity formula:

```
Return on Equity = Earnings / Equity → Earnings = Return on Equity * Equity
```
|Year                   | 2017 | 2018 | 2019 | 2020 | 2021 | 2022 |
|-----------------------|------|------|------|------|------|------|
|Return on Equity       |30.2% |26.9% |23.6% |20.3% |17.1% |13.8% |
|Equity (start of year) |10.27 |14.70 |18.65 |23.05 |27.74 |32.47 |
|Earnings               |4.43  |3.95  |4.40  |4.69  |4.73  |4.48  |
|Retained Earnings      |4.43  |3.95  |4.40  |4.69  |4.73  |4.48  |
|Equity (end of year)   |14.70 |18.65 |23.05 |27.74 |32.47 |36.95 |

A line of best-fit plotted through above earnings results in a slope of 0.0821, which divided by the average of earnings (US$4.45m) leads to an earnings growth rate of 1.85%.

|           Data point            |                          Notes                       |
|---------------------------------|------------------------------------------------------|
|Current Return on Equity         |Last reported value                                   |
|Industry Median Return on Equity |Median ROE of the industry within the listing country |
|Payout Ratio                     |Median payout of previous 3 years to avoid volatility |
|Total Equity                     |Last reported value                                   |


