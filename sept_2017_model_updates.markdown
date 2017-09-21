Important Updates to the Simply Wall St Company Analysis Model
==============================================================

This documents changes to the Simply Wall St Company Analysis model made in September 2017.

## Key Change #1: Company Valuation Models

### What&#39;s changed?

Simply Wall St now has four different company valuation models, building on from our two existing methodologies, which are automatically selected to best fit the characteristics of a particular stock, such as its industry and data availability.

### Why is this important?

Understanding the intrinsic value of a company is a crucial part of any investment decision and we want to ensure that our analysis fully utilizes our exclusive access to S&amp;P Capital IQ&#39;s premium quality data, in order to more accurately determine the true value of each stock.

### What are the details?

Our two previous method of valuing companies are: **2-Stage Discounted Cash Flow Model** and **Dividend Discount Model (DDM)**. The 2-stage model incorporates the fact that companies do not necessarily grow at a constant rate over time. Generally, they tend to be high-growth, and then become stable after a couple of years. The DDM is accurate for companies that consistently pays out a meaningful portion of their earnings. These models work relatively well for non-financial companies, and those that pay high dividends.

The problem is that financial companies are different, and their cash flows should be treated and valued differently. We&#39;ve overcome this problem by implementing two new valuation models: **Excess Returns Model** and **Adjusted-Funds-From-Operations (AFFO) Discounted Cash Flow Model**. If data is unavailable, we fall back to using the DDM, given that most financial firms do payout dividends.

Below is a flow chart which illustrates how we choose our valuation model for each stock:

![Simply Wall St Discounted Cash Flow Model Selection Proces](https://simplywall.st/build/images/landing/sws_model_selection_process.png "Simply Wall St Discounted Cash Flow Model Selection Process")

## Banks &amp; Insurance: Excess Returns Model

Since banks and insurance companies generally do not have a significant proportion of physical assets, and face different regulatory requirements for cash holdings, the **Excess Returns** method is better suited to calculate the intrinsic value of these companies than the traditional discounted cash flows model.

The key assumption for this model is that equity value is how much the firm can earn, over and above its cost of equity, given the level of equity it has in the company at the moment. The returns above the cost of equity is known as excess returns:

**Excess Return = (Return on Equity – Cost Of Equity) (Book Value Of Equity)**

We use this value to calculate the terminal value of the company, which is how much we expect the company to continue to earn every year, forever. This is a common component of discounted cash flow models:

**Terminal Value = Excess Return / (Cost of Equity – Expected Growth Rate)**

Putting this all together, we get the value of the company:

**Company Valuation = Book Value of Equity + Present Value of Terminal Value**

**Value Per Share = (Book Value of Equity + Present Value of Terminal Value) / Shares
                                  Outstanding**

Note that the component Book Value of Equity (BVE) represents the equity capital that has been invested in the company plus retained earnings. For each year going forward, BVE is estimated in order to reflect the growing nature of the company. Below is the source of our inputs above:

| Input | Source |
| --- | --- |
| Book Value of Equity | Most recent quarterly announcement |
| Future Book Value of Equity | Weighted average of analyst consensus estimates, if not available then the past median value is used |
| Stable Future Return on Equity | Weighted average of analyst consensus estimates, if not available then the past median value is used |
| Stable Future Earnings per Share | Weighted average of analyst consensus estimates if at least 5 analysts cover the stock, if not available then a multiplication of Stable Book Value and Stable Return on Equity is used. |

## Real Estate Investment Trusts (REITs): Adjusted Funds from Operations Discounted Cash Flows Model

This model is the same as the 2-Stage Discounted Cash Flows Model, except for one key difference – instead of discounting the company&#39;s free cash flows, we use its **Adjusted Funds from Operations (AFFO)** instead. AFFO better reflects the operational cash flows of REITs as opposed to the commonly used free cash flows.

**Funds from Operations (FFO)** is the company&#39;s earnings, with depreciation and amortization added back on, and removal of capital gains from property sales. AFFO has other adjustments the FFO number to make it even more accurate, by subtracting off capital expenditure and maintenance costs of the property, and adding rental increases. These factors are very specific to property and REITs, making it a far superior measure of value for these types of stocks.

Below is the source of our inputs above:

| Input | Source |
| --- | --- |
| Future AFFO | Weighted average of analyst consensus estimates, if less than 3 analysts have submitted estimates then FFO is used.|

## Key Change #2: Future Growth Rates and Checks

### What&#39;s changed?

Our new method for measuring future earnings growth rates will substantially improve the quality of our Future Performance Score and reduce a number of anomalies. We are achieving this by using weighted linear regression of forecast data from consensus of up to 50 analysts per stock, looking forward five years, as opposed to our old method of interpolation.

### Why is this important?

Understanding the growth potential of a company is key to any investment decision. Whilst this does mean we lose the granularity of seeing 1-year and 3-year growth expectations, it lowers the number of astronomical growth rates arising for companies growing off a low base. Furthermore, the new rate allows us to handle negative earnings, as well as give our users a much better idea of the likely future growth trend.

### What are the details?

Our old method took the last reported earnings, cash flow and revenue data and compared it to the consensus estimates in the future. Typically, analyst future estimates are done annually. This means we have one data point each year of the consensus level for each line item, from which we perform a simple growth rate calculation relative to the most recent financial year data. If one analyst is extremely bullish for the next three years ahead, and the stock only has two analyst coverage, our growth rate will be skewed upwards by one source of data.

To overcome this problem, we&#39;ve applied a weighted linear regression model, which generates a line of best-fit between the isolated annual data points, and calculated the growth rate based off this slope. We&#39;ve weighted data points with more analyst coverage to give them higher importance, as opposed to equally weighing growth rates for a year with 30-analyst coverage, and another year with a single extremely bullish analyst. This means our growth rates are more representative of the belief of the market, and within the range which should be more appropriate for the company.

Note that this future growth rate will also be used in our Price-To-Earnings (PEG) ratio, which previously used the +1-year growth rate, and therefore will not make this ratio directly comparable to those found on other websites. However, we believe our ratio will more meaningful and superior for investors who want dynamic data, rather than static. In addition to future growth rates, we&#39;ve also implemented the linear regression method to annual past earnings growth and the average annual dividend growth over 10 years.

## New versus Old Future Performance Checks

As a result of improving how we measure future growth, we&#39;ve also revised the Future Performance Score checks, which is part of the Snowflake.

|   | New Future Performance Checks | Previous Future Performance Checks |
| --- | --- | --- |
| 1 | Net income annual growth rate greater than the low risk savings rate | Earnings growth in 1 year greater than the low risk savings rate  |
| 2 | Net income growth rate greater than market average | Earnings growth in 3 years greater than the low risk savings rate  |
| 3 | Revenue annual growth rate greater than the market average  | Revenue growth in 2 years greater than 50%  |
| 4 | Net income annual growth rate greater than 20%  | Operating cash flows growth in 2 years greater than 50%  |
| 5 | Revenue annual growth rate greater than 20% | Earnings growth in 2 years greater than 50%  |
| 6 | Return on equity in 3 years greater than 20% | Return on equity in 3 years greater than 20%  |

## Key Change #3: Updates to the Industry Average Calculations

### What&#39;s changed?

Depending on the metric we are now using median or market cap-weighted average with boundaries to exclude significant outliers. We are also further refining the classification of industries, from a more generic primary level of 24 industries such as Capital Goods, to a more specific secondary level of 68 industries such as Electrical Equipment.

### Why is this important?

Comparing your stock to its peers is an important concept of investing. As Simply Wall St begins to cover every stock market in the world, we need to further refine which peer group is relevant to each stock, in order to provide useful relative valuation. An example would be the average PE ratio for mining stocks in Brazil.

### What are the details?

The new system updates the various averages every 6 hours, for 68 industries, in every country we cover. In the case of industry groups with less than five companies, we use the global average for that industry instead. This method allows us to provide more meaningful averages when the data is rich and precise, as well as providing alternatives for small industries of companies with lack of analyst coverage or general macroeconomic variables available for analysis.

Read more about how we calculate industry averages [here](https://github.com/SimplyWallSt/Company-Analysis-Model/blob/master/industry_averages.markdown).
