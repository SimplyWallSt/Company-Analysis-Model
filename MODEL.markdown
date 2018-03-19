![Simply Wall St Logo](https://simplywall.st/images/simplywallst384.png "Simply Wall St Logo")
 
 Simply Wall St Company Analysis Model
======================================



## Contents
* [Overview of the model](#overview-of-the-model)
* [The Snowflake](#the-snowflake)
* [Value Analysis](#value)
* [Future Performance analysis](#future-performance)
* [Past Performance analysis](#past-performance)
* [Financial Health analysis](#health)
* [Dividends analysis](#income-dividends)
* [Management analysis](#management)

Overview of the model
---------------------

The [Simply Wall Street](https://simplywall.st/) (SWS) app is designed to help make you a better
investor by allowing you to make non-emotional long term investment
decisions.

The SWS app is not intended to provide investment advice or
recommendations. Rather the SWS app is an analysis platform which
provides information and analytics allowing investors to identify and
assess stocks which meet their investment parameters and objectives -
for example high quality consistent performers, income oriented stocks
or growth oriented stocks. The results are presented in an easy to
understand infographic form with the aim of making the underlying data
more understandable to users.

To assess stocks, the SWS app performs a number of quantitative "checks"
across a range of assessment criteria and provides the results in a
visually intuitive Snowflake (see below).

The checks performed are based on widely accepted and tested investment
criteria, and used by demonstrably successful investors and investment
firms.

Our checks are divided into 5 assessment criteria:



  Area                   | Assessment Criteria
  -----------------------| ---------------------------------------------------------------------------------------------------------------------------------------
  Value                  | The fair value of the company's shares, and how that value compares with the current share price, other companies and the stockmarket
  Future performance     | Anticipated future financial performance based on analyst forecasts
  Past performance       | The historical financial performance of the company
  Health                 | The financial strength of the company's balance sheet
  Dividends		 | The dividend being paid, and the sustainability of the dividend

The assessment criteria and individual checks performed are explained in
this document.

**The Snowflake**
-----------------

The results of the checks in each of the 5 assessment criteria are
presented visually in our Snowflake. The snowflake has been designed to
present the results for a company as a visually intuitive summary in
order to allow:

-   a quick "eyeball" scan of a particular stock, a group of stocks or
    the stockmarket as a whole;

-   visual comparisons of the results of our stock filters;

-   visual side by side comparisons of selected stocks using our
    "compare" feature;

-   consolidated view using our "portfolio" feature.

#### Example Snowflake
![Example Snowflake Tile](https://simplywall.st/build/images/landing/NYSE-WALT250.PNG "Example Snowflake Tile" )

#### Methodology behind generating the Snowflake  
The snowflake is constructed as follows:

1.  for each assessment criteria, there are 6 individual checks
    performed (giving a total of 30 checks for each stock);

2.  if a check is successful, it is assigned a score of "1";

3.  the total successful checks are added to give an overall score for
    each assessment criteria - for example a stock may receive 4
    successful check scores for "Health", giving a total Health score of
    4 (from a possible 6);

4.  the total score for each of the assessment criteria is shown on the
    relevant axis of the snowflake.

The total scores for each assessment criteria are then used to generate
the shape and colour of the snowflake. The greater the total number of
successful checks the larger the snowflake.

In addition the snowflake is colour coded - the greater the number of
successful checks the more "green" the snowflake - the fewer the more
"red" the snowflake will appear.

### Notes on shape and colour

While the size and colour of the snowflake broadly indicates the
"quality" of the company, a low score in a particular assessment
criteria should not necessarily exclude a stock from investment
consideration. The snowflake simply summarises visually relevant
characteristics of a stock.

For example, a low "Dividends" score simply indicates that from an Dividend
point of view, the company may be paying a low dividend, however it may
also be experiencing high growth and reinvesting cash in growth
initiatives. In this example, investors seeking high growth
opportunities may still consider the stock as an investment candidate.

Investors should therefore consider each of the assessment criteria in
terms of their own investment objectives and orientation.

### Changes in shape and colour/ Snowflake Sensitivities

The size and colour of a company snowflake will change over time as data
is updated - in particular for updated earnings results and changes in
share price.

The Snowflake is specifically designed to help investors become less
emotional by ignoring minor share price fluctuations and focusing on the
fundamentals. Four out of five axis only change when new company or
analyst level data is available.

The sensitivity of the axis:

  Area                   | Main sensitivity
  -----------------------| ------------------------------------------------------------------------------------------------------------------------------------
  Value                 |  Sensitive to changes share price however the change must be significant to breach the various thresholds detailed in this document
  Future performance    |  Expected growth rates of earnings per share, revenue, cash flow and net income
  Past performance      |  Historical earnings per share performance
  Health                |  Balance sheet and ability to service debt
  Dividends		|  The reliability and sustainability of the dividend

### Summary of the Snowflake

The graphic below summarises the checks used to generate the Snowflake. The remainder of this document explains each in detail and the analysis used in the Management screen.

A PDF of this graphic is available [here](https://simplywall.st/documents/Simply-Wall-St-The-Snowflake-explained.pdf).

![Snowflake Summary](https://simplywall.st/documents/Simply-Wall-St-The-Snowflake-explained-700.png "Snowflake Summary" )

**Value**
---------

While the stock market sets a &quot;price&quot; for a company, this price will often be affected by a wide range of factors, some of which may not impact the true worth, or fair value, of the company. By comparing the market price to the fair value of a company, or a set of companies or indices, investors can determine whether a company&#39;s shares are potentially over- or undervalued.

There are many methods which can be used to determine the fair value of a company. The SWS app uses two approaches: discounted cash flows and relative valuation.

### Discounted Cash Flows (DCF)

DCF is the most widely-accepted method to calculate the fair value of a company. It is based on the premise that the fair value of a company is the total value of its incoming cash flow less its expenses, technically called Free Cash Flows (FCF), discounted to today&#39;s value.

The SWS app uses four variations of DCF depending on the characteristics of a particular stock, such as industry and data availability.

- **2-Stage Discounted Cash Flow Model:** suitable for companies that do not necessarily grow at a constant rate over time. They tend to be high-growth initially, and become stable after a couple of years.
- **Dividend Discount Model (DDM):** accurate for companies that consistently pays out a meaningful portion of their earnings as dividends.
- **Excess Returns Model:** used for financial companies such as banks and insurance, generally do not have a significant proportion of physical assets, and face different regulatory requirements for cash holdings.
- **Adjusted-Funds-From-Operations (AFFO) 2-Stage Discounted Cash Flow Model:** used for Real Estate Investment Trusts (REITs), as they incur capital gains and other real estate-specific factors which impacts their free cash flows.

![Simply Wall St Discounted Cash Flow Model Selection Proces](https://simplywall.st/build/images/landing/sws_model_selection_process.png "Simply Wall St Discounted Cash Flow Model Selection Process")

#### 2-Stage Free Cash Flow Model – How Is This Calculated?

Two calculations are performed: high-growth stage and stable-growth stage. In **high-growth** , estimates over the next five years of levered free cash flow to equity are used, which is sourced from market analyst consensus estimates. If no estimates are available, then the last estimate or reported value is extrapolated using historical average annual growth rate, capped within a reasonable range of 20% in the first year declining by 1% per year.

In **stable-growth** , a terminal value is calculated using the Gordon Growth formula, with an assumption that the company will continue to grow its earnings at the 10-year government bond rate, forever. The sum of the cash flow arising from the forecasts are then discounted to today&#39;s value using a discount rate, then divided by shares on issue, giving a value per share.

#### Dividend Discount Model – How Is This Calculated?

Since dividends are a form of cash flows which are directly returned to shareholders, it can be used to determine how much a share value is worth to a shareholder who will reap the benefit of these future **dividend payments**. The Gordon Growth model is used to discount a company&#39;s dividend payments over time, with the assumption that dividends will continue to grow at a certain rate forever.

Using the expected dividend per share, the value of a stock is found by:

    Value = Expected dividends per share / (Discount Rate - Perpetual growth rate)

#### Excess Returns Model – How Is This Calculated?

**Excess Returns** method is better suited to calculate the intrinsic value of financial companies than the traditional discounted cash flows model. The key assumption for this model is that equity value is how much the firm can earn, over and above its cost of equity, given the level of equity it has in the company at the moment. The returns above the cost of equity is known as excess returns:

    Excess Return = (Return on Equity – Cost Of Equity) (Book Value Of Equity)

We use this value to calculate the terminal value of the company, which is how much we expect the company to continue to earn every year, forever. This is a common component of discounted cash flow models:

    Terminal Value = Excess Return / (Cost of Equity – Expected Growth Rate)

Putting this all together, we get the value of the company:

    Company Valuation = Book Value of Equity + Present Value of Terminal Value

    Value Per Share = (Book Value of Equity + Present Value of Terminal Value) / Shares Outstanding

Note that the component Book Value of Equity (BVE) represents the equity capital that has been invested in the company plus retained earnings. For each year going forward, BVE is estimated in order to reflect the growing nature of the company.

#### Adjusted Funds from Operations Discounted Cash Flows Model – How Is This Calculated?

This model is the same as the 2-Stage Discounted Cash Flows Model, except for one key difference – instead of discounting the company&#39;s free cash flows, we use its **Adjusted Funds from Operations (AFFO)** instead. AFFO better reflects the operational cash flows of REITs as opposed to the commonly used free cash flows.

**Funds from Operations (FFO)** is the company&#39;s earnings, with depreciation and amortization added back on, and removal of capital gains from property sales. AFFO has other adjustments the FFO number to make it even more accurate, by subtracting off capital expenditure and maintenance costs of the property, and adding rental increases. These factors are very specific to property and REITs, making it a far superior measure of value for these types of stocks.

If AFFO estimates is unavailable, we fall back to using FFO. However, if both are unavailable, we use another REIT-specific measure called **Net Asset Value (NAV).** NAV is basically the total market value of the REIT&#39;s investments and other assets, less its short-term and long-term liabilities – essentially, it&#39;s equity value!

#### How Is The Discount Rate Determined For All DCF Methods?

The discount rate is calculated based on the following equation:

    Discount rate = Cost of Equity = Risk Free Rate + (Levered Beta \* Equity Risk Premium)

The risk-free rate is the 10-year government bond rate and the equity risk premium is 10% less the risk-free rate. Beta is a measure of volatility, or risk, in comparison to the market as a whole.

A bottom-up beta is calculated for each company by using it&#39;s industry unlevered beta (removes the effect of debt and varying capital structure) and levering it up using the company&#39;s own debt level to take into account its own capital structure. The bottom-up beta cannot be lower than 0.8 (this is the lowest practical beta for a stable firm, according to Damodaran) or greater than 2.

Levered beta is used in the case of financial firms, and is not re-adjusted to account for varying capital structure. Therefore, the average levered beta of comparable companies is used as the bottom-up beta for financial firms.

#### What Are The Advantages And Disadvantages of The DCF Model?

The advantages of DCF are:

- DCF value is not affected by emotional or unquantifiable factors (which often affect stock market prices);
- DCF uses objective, measurable data and inputs to calculate a fair value;
- DCF allows investors to determine whether the share price of a company is potentially over- or undervalued.

The drawbacks of DCF are:

- DCF calculation is sensitive to its key inputs - the growth rate and the discount rate. Relatively small changes in these inputs affect the final value significantly;
- DCF is a highly quantitative technique which may not fully reflect changes in non-financial information;
- DCF is not applicable to companies which does not generate positive free cash flow (for example high-growth technology companies which are not yet profitable);
- Estimating free cash flow for financial institutions can be difficult.

#### What Does A Typical DCF Calculation Look Like?

Below is an example calculation for [Walt Disney
(NYSE:DIS)](https://simplywall.st/NYSE:DIS/walt-disney#value) from 22/09/2015. Note the details of the calculation can be found for any stock on SWS by clicking **Learn More** or by clicking the valuation infographic.


    **5 year cash flow forecast**
    				2015        	2016		2017		2018		2019
    Levered FCF (USD, Millions)	$6,563  	$8,491		$9,704		$11,063		$12,434
    Source				Analyst x16 	Analyst x16 	Analyst x10 	Analyst x8  	Analyst x5
    Present Value
    Discounted (@ 8.4%)		$6,053      	$7,223		$7,613		$8,006		$8,299
    
    Present value of next 5 years cash flows:
    $37,195
    
    **Terminal Value**
    Terminal Value = FCF2019 × (1 + g) ÷ (Discount Rate – g)
    Terminal Value = $12,434 × (1 + 2.1%) ÷ (8.42% – 2.1%)
    Terminal value based on the Perpetuity Method where growth (g) = 2.1%:
    $201,152
    Present value of terminal value:
    $134,257
    
    **Equity Value**
    Equity Value (Total value) = Present value of next 5 years cash flows + terminal value
    Value = Total value / Shares Outstanding ($171,452 / 1,688)
    Value per share: 
    $101.58

    ----------------------------------------------
	Current discount (share price of $103.41): -2%
	----------------------------------------------
    
    
    **Estimate of Discount Rate**
    The discount rate, or required rate of return, is estimated by calculating the Cost of Equity.
    Discount rate = Cost of Equity = Risk Free Rate + (Levered Beta * Equity Risk Premium)
    Discount rate = 8.42% = 2.11% + (0.8 * 7.89%)
    
    
    **Estimate of Bottom Up Beta**
    The Levered Beta is the Unlevered Beta adjusted for financial leverage. It is limited to 0.8 (lowest range for a stable firm).
    Levered Beta = Unlevered beta (1 + (1- tax rate) (Debt/Equity))
    0.569 = 0.536 (1 + (1- 30%) (8.75%))
    Levered Beta used in calculation = 0.8

Data points used in 2-Stage Free Cash Flow Model

| **Data point** | **Notes** |
| --- | --- |
| Levered Free Cash Flow estimates +1 to +5 years | Annual |
| Levered Free Cash Flow actual last reported | Annual |
| Revenue (LTM to -5 years) | Annual |
| Debt to equity ratio | Annual, last reported |
| Dividend per share | Annual, last reported |
| Return on equity (ROE) | Last reported |

Data points used in Excess Returns Model

| **Data point** | **Notes** |
| --- | --- |
| Estimates of Return on Equity | Annual |
| Estimates of Book Value of Equity | Annual |
| Book Value of Equity | Last reported |
| Return on equity (ROE) | Last reported |

Data points used in Adjusted Funds from Operations 2-Stage Model

| **Data point** | **Notes** |
| --- | --- |
| Estimates of Adjusted Funds from Operations | Annual |
| Estimates of Funds from Operations | Annual |
| Adjusted Funds from Operations | Annual, last reported |
| Funds from Operations | Last reported |

Data points used in Dividend Discount Model

| **Data point** | **Notes** |
| --- | --- |
| Estimates of Dividends per Share | Annual |
| Dividends per Share | Last reported |

**Where Can I Go To Learn More About DCF?**

- http://www.streetofwalls.com/finance-training-courses/investment-banking-technical-training/discounted-cash-flow-analysis/
- http://people.stern.nyu.edu/adamodar/pdfiles/ovhds/dam2ed/dcfveg.pdf
- http://pages.stern.nyu.edu/~adamodar/pdfiles/valn2ed/ch13.pdf


### Relative Valuation

Relative valuation is another method to calculate a company&#39;s fair value. The key difference between this method and discounted cash flows, is that we use the value of the company&#39;s industry peers as a benchmark for whether the company is over- or undervalued, rather than directly assessing the company&#39;s cash flows.

The SWS app calculates three types of relative valuation.

- **Price-to-Earnings (PE) ratio:** useful for profitable companies generating consistent net income over time.
- **Price-to-Earnings Growth (PEG) ratio:** suitable for profitable companies with projected growth in the bottom-line in the future.
- **Price-to-Book (PB) ratio:** appropriate for companies with high levels of physical assets, or loss-making.

#### PE Ratio – How Is This Calculated?

The PE ratio is used to give an indication of the value of the share price as a function of the company&#39;s net income per share. As a market-based ratio, it provides a shorthand indication of the relative valuation of a company and allows a comparison of the valuation between companies, against an industry sector or the stock market as a whole.

The higher the PE ratio, the more &quot;expensive&quot; the stock is considered to be. For example, a company with a PE ratio of 25 times would be considered more &quot;expensive&quot; than a company with a PE ratio of 15 times, or the whole market average PE of 18.

The PE ratio is calculated as:

    PE ratio = Current share price / Earnings per share

| **Data point** | **Notes** |
| --- | --- |
| GAAP Earnings per Share | (Annual, last reported),converted to the currency of the listing if different. |
| Share price | End of day in the currency of the listing |

#### PEG Ratio – How Is This Calculated?

The PEG ratio is used to give an indication of the value of the share price as a function of the growth in a company&#39;s net income per share. Similar to PE, as a market-based method, it allows us to compare a company&#39;s growth and earnings level to its industry sector or the wider stock market.

The higher the PEG ratio, the more &quot;expensive&quot; the stock is considered to be taking account the company&#39;s rate of earnings growth. For example, a company with a PEG ratio of 1.2 would be considered more &quot;expensive&quot; than a company with a PEG ratio of 1.0. Stocks are considered to have a &quot;fair&quot; PEG ratio of between 0.8 and 1.0.

The PEG ratio is not usually compared to a market average due to the diversity and differing nature of companies across the market. Note that the PEG ratio depends highly on the PE ratio and growth rate used. Other websites may quote different PEG ratios depending on which time period EPS growth is calculated.

The PEG ratio is calculated as:

    PEG ratio = PE ratio / Annual net income growth rate (%)

| **Data point** | **Notes** |
| --- | --- |
| PE Ratio | As above |
| Annual net income growth rate | The same annual net income growth rate calculated in the  [Future Performance analysis](https://github.com/SimplyWallSt/Company-Analysis-Model/blob/master/MODEL.markdown#minimum-earnings-growth) |

#### PB Ratio – How Is This Calculated?

The PB ratio is used to give an indication of the value of the share price as a function of the &quot;book value&quot; of a company. The book value is calculated as assets less intangible assets less liabilities per share - in the other words the net tangible assets held by the company.

The PB ratio allows a comparison of the valuation between companies, against an industry sector or the stock market as a whole.

The higher the PB ratio, the more &quot;expensive&quot; the stock is considered based on the company&#39;s net tangible assets. For example, a company with a PB ratio of 4.0 would be considered more &quot;expensive&quot; than a company with a PB ratio of 3.0.

The PB ratio is most commonly compared to the relevant industry average as companies within an industry average will usually have common asset characteristics - for example airlines are capital-intensive businesses, usually with high asset holdings.

The PB ratio is calculated as:

    PB ratio = Stock Price / Book Value per Share

| **Data point** | **Notes** |
| --- | --- |
| Book value per share | Annual, last reported |
| Share price | End of day in the currency of the listing |


### The SWS Snowflake checks regarding value

The SWS performs 6 checks regarding "value".

##### CHECK #1: Is the discounted cash flow value less than 20% of the share price?

The SWS app compares the fair value (ie the calculated DCF value) to the current share price.

If the share price is =&gt; 20% below the fair value, it is considered to be moderately undervalued and is scored one point.

##### CHECK #2: Is the discounted cash flow value less than 40% of the share price?

The fair value of a stock, calculated using DCF model, is compared to its current market share price.

If the share price is below the fair value by 40% or more, then it is considered substantially undervalued and is scored one point.

##### CHECK #3: Is the PE ratio less than the market average but still greater than 0?

The PE ratio is compared to the whole market PE ratio for the country of listing.

If the PE ratio is less than the market average PE ratio, then the stock is scored one point.

##### CHECK #4: Is the PE ratio less than the industry average but still greater than 0?

The PE ratio is compared to the industry average PE ratio for its industry classification.

If the PE ratio is less than the industry average PE ratio, then the stock is scored one point.

##### CHECK #5: Is the PEG ratio within a reasonable range (0 to 1)?

The PEG ratio is compared to the range of 0 to 1.

If the PEG ratio falls within this range, then the stock is scored one point.

##### CHECK #6: Is the PB ratio within a reasonable range (0 to 1)?

The PB ratio is compared to the relevant industry average.

If the PB ratio is greater than zero, but below the industry average, then the stock is scored one point.


**Future Performance**
----------------------

The SWS app examines professional analyst estimates of company future expectations for revenue, cash flow, net income and return on equity, which in turn are used to calculate growth for the respective line items. Historically, it has been demonstrated that analyst estimates, on average, are relatively accurate over the short term.

#### How does SWS calculate growth rates

Annual growth rates for each line item are calculated using weighted linear regression which plots a line of best-fit through the time series data point. The year with more analyst coverage has higher weighting, which means we place more importance on estimates with twenty analysts&#39; forecasts compared to ones with only a few. The first data point is taken from the most recent earnings release and given a weight of one.

The slope, or gradient, of this line is then divided by the average of the absolute values to compute the annual growth rate. Using absolute values allow us to calculate a growth rate even when a line item, such as earnings, is negative, or is expected to become positive.

#### Data points used to perform these checks

| **Data point** | **Notes** |
| --- | --- |
| Annual Earnings Growth Rate | Annual growth rate of GAAP net income excluding extraordinary items over the next 3-5 years based on analyst&#39;s estimates |
| Annual Revenue Growth Rate | Annual growth rate of revenue over the next 3-5 years based on analyst&#39;s estimates |
| Low risk savings rate | Readily available consumer savings account interest rate of the listing country |
| Inflation (CPI) | CPI of the region of the listing country |
| Market Average Annual Net Income Growth Rate | Weighted average annual net income growth rate of the listing country.See industry averages methodology for how this is calculated. |
| Market Average Annual Revenue Growth Rate | Weighted average annual revenue growth rate of the listing country.See industry averages methodology for how this is calculated. |

#### Return on Equity (ROE)

Return on Equity (or Return on Shareholders Funds) measures
profitability in terms of a company's shareholders funds, so provides an
indication of the profitability and efficiency of the usage of the
company's own funds to generate profits.

Return on Equity is calculated as:

    Return on Equity = Net Income / Average Equity (Shareholders Funds)

  **Data point**                         | **Notes**
  ---------------------------------------| --------------------------------------
  Current Return on Equity              |  Last reported
  Estimated Return on Equity in 3 years |  Based on consensus analyst estimates

The main advantage of ROE is that it takes into account movements in
equity issued by the company which may distort other measures of
profitability. The main disadvantage is that ROE is not affected by the
level of debt (or additional debt) held by a company.

The higher the ROE, the higher the return generated by the company, and
vice versa.

An ROE of 20% or greater is considered to be indicative of a company
which is highly profitable / efficient.

### The SWS Snowflake checks regarding Future Performance

##### CHECK #1: Is the annual growth rate in earnings expected to exceed the low risk savings rate, plus a premium to keep pace with inflation?

This check measures whether the expected net income/ earnings growth of a stock at least matches the low-risk savings rate plus a premium to keep pace with inflation. If not, it may be more rational to invest in a low-risk savings product rather than the stock being reviewed, which carries a higher level of risk.

If the average annual growth rate of earnings is greater than the low risk savings rate plus inflation, then the stock is scored one point.

If the company is expected to become profitable in the next 5 years, then the stock is also scored one point.

##### CHECK #2: Is the annual growth rate in earnings expected to exceed the market average in the country of listing?

This check measures whether the company is expected to grow net income/ earnings by more than the average stock in market in which it is listed.

If the average annual growth rate of net income is greater than the weighted average earnings growth for stocks listed in the same country, then the stock is scored one point.

##### CHECK #3: Is the annual growth rate in revenue expected to exceed the market average in the country of listing?

This check measures whether the company is expected to grow revenue by more than the average stock in market in which it is listed.

If the average annual growth rate of revenue is greater than the weighted average revenue growth for stocks listed in the same country, then the stock is scored one point.

##### CHECK #4: Is the annual growth rate in earnings above 20%?

This check is used to identify high-growth companies by looking at the annual growth rate of its earnings. Earnings growth indicates whether the company is able to grow its profitability, which fundamentally impacts the valuation of the company.

If the average annual growth rate of net income/ earnings is greater than 20%, then the stock is scored one point.

##### CHECK #5: Is the annual growth rate in revenue above 20%?

This check is used to identify high-growth companies by looking at the annual growth rate of its revenues. Revenue growth is a pure measure of growth, as the number is more difficult to manipulate. It usually sheds light on how the company&#39;s operations are doing and how they are growing, whether it is increasing prices, expanding market share or introducing new products.

If the average annual growth rate revenue is greater than 20%, then the stock is scored one point.

##### CHECK \#6: Is the Return on Equity (ROE) in 3 years expected to be over 20%?

The Return on Equity (ROE) in 3 years' time is calculated based on the
average analyst estimates of earnings.

If the ROE in 3 years’ time is estimated to be \> 20% the stock is
scored one point.

**Past Performance**
--------------------

The Past Performance section of the SWS app provides an analysis of a
company's historical performance over the past 5 financial years.

### The SWS Snowflake checks regarding Past Performance

### Historical Earnings per Share (EPS) growth

Earnings per Share (EPS) measures company earnings expressed on a per
share basis.

EPS is calculated as:

    EPS = Net Profit / Average number of shares on issue during the year

The EPS figure is widely used to measure the absolute profit that a
company earns on a per share basis. As it uses a common base, EPS can be
used to compare different companies and industries. For that reason it
is used in the calculation of the Price to Earnings (PE) Ratio, which
gives an indication of the relative price of different companies' stock
prices.

An important advantage of EPS is that distortions which may arise from
changes in the number of company shares issued (eg arising from an
equity capital raising) are accounted for. An important disadvantage of
EPS is that it does not consider the shareholder's funds employed or the
level of debt held by a company.

Data points used in the Earnings per Share checks:

  **Data point**                                                      | **Notes**
  --------------------------------------------------------------------| -----------------------------------------
  Historical GAAP Earnings per Share (LTM to -5 years)  | Annual, last reported quarterly results

#### How is the 5 year annual average calculated?

To calculate the 5 year annual average growth a linear regression trend
line is fitted to the historical quarterly LTM EPS data and the gradient
(M coefficient) divided by the average earnings over the same period.
This not only produces the best overall growth trend but also handles
some negative earnings.

#### How is growth from negative earnings handled?

Calculating a growth rate when the earnings in the starting period are
negative is difficult and sometimes meaningless, for this reason no
‘growth’ ratio is used rather SWS informs the user this is the case and
awards scores accordingly.

##### CHECK \#1: Is Has Earnings Per Share (EPS) growth exceeded that of the company's industry average over the past year?

If the EPS growth of the company is \> the EPS growth of its relevant
industry average the stock is scored one point.

This check measures the performance of the company against its peer
group average.

##### CHECK \#2: Is Have Earnings Per Share (EPS) increased in past 5 years?

If the EPS for the current year is \> the EPS from 5 years ago the stock
is scored one point.

##### CHECK \#3: Is the current EPS growth higher than the average annual growth over the past 5 years? 

If current year growth in EPS is \> the average annual growth in EPS
over the past 5 years the stock is scored one point.

### Return on Equity (ROE)

See earlier section for full detail on Return on Equity.

  **Data point**            | **Notes**
  --------------------------| ---------------
  Current Return on Equity  | Last reported

##### CHECK \#4: Is the Return on Equity (ROE) higher than 20%?

If the ROE for the company for the current year is \> 20% the stock is
scored one point.

### Return on Capital Employed (ROCE)

Return on Capital Employed (ROCE) measures the profitability of a
company in terms of the total capital employed by the company, both
equity (or shareholders funds) and long term liabilities (which are
often primarily made up of debt).

ROCE is calculated as:

    Return on Capital Employed (ROCE) = Net Income / Long Term Liabilities

ROCE measures the efficiency of the usage of the company's total
available capital, and is often used in conjunction with ROE to provide
a more comprehensive measure of profitability. In particular ROCE takes
into account debt (and increased debt) utilised by a company to generate
returns.

The higher the ROCE, the higher the profitability of the company, and
vice versa.

  **Data point**                          | **Notes**
  ----------------------------------------| -----------
  Net income (LTM & -3 years)             | Annual
  Long term liabilities (LTM & -3 years)  | Annual

##### CHECK \#5: Has the Return on Capital Employed (ROCE) increased from 3 years ago?

If the current year ROCE is \> the ROCE from 3 years ago the stock is
scored one point.

### Return on Assets (ROA)

Return on Assets (ROA) calculates the profitability of a company in
terms of the total Assets held by the company. It is a broad measure of
the efficiency of asset usage by the company and is often used to
compare the returns of companies in capital intensive industries such as
manufacturing or raw materials production.

ROA is calculated as;

    Return on Assets (ROA) = Net Income /Total Assets

  **Data point**            | **Notes**
  --------------------------| ---------------
  Current Return on Assets  | Last reported

##### CHECK \#6: Is the Return on Assets (ROA) above industry average?

If the current year ROA is \> the relevant industry average the stock is
scored one point.

**Health**
----------

The Health section of the SWS app provides an analysis of a company's
financial position, primarily in terms of the company's Balance Sheet,
and in particular the amount of debt held by the company.

#### Point to note regarding Health metrics

Financial Institutions (Banks, Financial Service companies, REIT’s and
Insurance firms) by their nature borrow the majority of their funding
(or liabilities), and as a result conventional measures of debt levels
are not generally applicable. For that reason the SWS app uses a
separate series of Health checks specifically applicable to Financial
Institutions.

### Non-financial institutions analysis

The analysis performed for non-financial institutions uses the following
data points as input:

  **Data point**                               | **Notes**
  ---------------------------------------------| -----------------------
  Short term Assets                           |  Last reported
  Long term Assets                            |  Last reported
  Short term liabilities                      |  Last reported
  Long term liabilities                       |  Last reported
  Total debt (LTM to -5 years)                |  Last reported
  Total shareholders equity (LTM to -5 years) |  Last reported
  Operating cash flow                         |  Annual, last reported
  Net interest expense                        |  Annual, last reported
  Net income                                  |  Annual, last reported

Full balance sheet data is visualized in the infographic.

#### Balance sheet checks

##### CHECK \#1: Are short term assets greater than short term liabilities?

This check measures whether, on a short term basis (\< 12 months), the
company has a net positive financial position. In the event of financial
stress, this check indicates whether the company could liquidate short
term assets to meet its short term liabilities.

If the company's short term assets are \> short term liabilities the
stock is scored one point.

##### CHECK \#2: Are short term assets greater than long term liabilities?

This check measures whether the company holds short term assets which
are greater than its long term (\>12 months) liabilities. In the event
of financial stress, this check indicates whether the company could
realise short term assets to meet its long term liabilities.

If the company's short term assets are \> long term liabilities the
stock is scored one point.

#### Debt to Equity Ratio

The Debt to Equity ratio measures a company's total debt relative to its
total book value of shareholders' equity (i.e. net worth or shareholders' funds). 
This ratio illustrates the level of leverage a company has. If the ratio is high, 
this indicates that the company is holding a high level of debt compared to 
its net worth, and in the event of financial stress, may experience difficulty 
meeting debt or interest obligations.

A ratio of 40% or less is considered acceptable.

The Debt to Equity ratio is calculated as;

    Debt to Equity ratio = Total Debt / Total Book Value of Shareholders Equity

##### CHECK \#3: Has the debt to equity ratio increased in the past 5 years?

The Debt to Equity ratio for the current year is compared to the debt to
equity ratio 5 years ago. If the ratio has not increased, or has fallen,
the stock is scored one point.

##### CHECK \#4: Is the debt to equity ratio over 40%?

If Debt to Equity ratio is \< 40% the stock is scored one point.

##### CHECK \#5: Is debt covered by operating cash flows?

This check indicates whether, in the event of financial stress, the
company is able to meet its debt obligations using purely its cash flow 
for the year from its operational activities.

Debt held the company is compared to Operating Cash Flows. If Operating 
Cash Flows are \> Total Debt the stock is scored one point.

##### CHECK \#6: Are earnings greater than 5x the interest on debt (if company pays interest at all)?

This check indicates whether the company's interest obligations are met
through earnings before interest and tax (EBIT). A ratio of 5 times earnings 
indicates a strong level of coverage.

If EBIT is \> 5 x interest on debt the stock is scored one point.

### Cash Runway Analysis

Placeholder

### Financial Institutions

This analysis is used in the case of Banks, Financial Service companies,
REIT’s and Insurance firms.

The following data points are used in addition to the previous for this
analysis:

  **Data point**                      | **Notes**
  ------------------------------------| ---------------------------------------------------------------
  Total deposits                      | Last reported
  Total loans                         | Last reported
  Total non-performing loans          | Last reported
  Allowance for non-performing loans  | Last reported
  General/ Specific allowance         | Last reported (Represents reserves created for problem loans)
  Net charge offs                     | Last reported

##### CHECK \#1: Is Leverage (Assets to Equity) \> 20x?

Leverage (or gearing) refers to the amount of assets held in a business
when compared to the company's own resources (shareholders funds or
equity).

While Financial Institutions will always have an elevated level of
leverage, if the level becomes too high the institution may come under
stress in the event of adverse circumstances. A leverage ratio of 20
times or less is considered acceptable.

Total Assets are compared to Shareholders Equity. If Total Assets are \<
20 times Shareholders Equity the stock is scored one point.

##### CHECK \#2: Coverage of bad loans (Bad Loan Coverage) \> 100%?

Bad loans are loans made by Financial Institutions which are considered
to be unrecoverable. Bad loan coverage refers to provisions set aside
against potential bad loans. A provision of this nature is offset
against profits.

Bad loan provisions held are compared to the level of Bad loans actually
written off. If the Bad Loan provisions are \> actual Bad Debts written
off the stock is scored one point.

##### CHECK \#3: Proportion of lower risk deposits compared to total funding (Deposits to Liabilities) \< 50%? 

Financial Institutions borrow money (to lend) in many different forms.
Deposits from customers generally bear the lowest risk as they are less
volatile than other forms of borrowing in terms of both the amount
available (which does not usually change quickly) and interest rate paid
(the rates paid are set by the Financial Institution itself).

Broadly the higher the level of Deposits held the less risky the
Financial Institution is considered to be.

Total Deposits held are compared to Total Liabilities. If Total Deposits
are \> 50% of Total Liabilities the stock is scored one point.

##### CHECK \#4: Proportion of higher risk assets compared to total assets (Loans to Assets \> 110%)?

The Loans to Assets ratio measures the net loans outstanding as a
percentage of total assets. The higher this ratio indicates a bank has a
high level of loans and therefore its liquidity is low. The higher the
ratio, the more risky a bank may be to higher defaults.

Financial firms such as Banks with high Loans to Assets ratios rely on
interest income from loans and other securities for a high portion of
their total revenue. Those with lower ratios have more diversified
sources of revenue, for example from investment banking and asset
management.

If Net Loans are \< 110% of Total Assets the stock is scored one point.

##### CHECK \#5: Total loans compared to deposit funding (Loans to Deposits \> 125%)?

The Loans to Deposits (LTD) ratio measures the liquidity of a Financial
Institution. Liquidity refers to the funds available to a Financial
Institution to repay liabilities, in particular Deposits (recognising
that Deposits must generally be repaid on demand, or at short notice).
Loan assets on the other hand generally have a fixed term, and often
cannot be readily realised.

If the LTD ratio is too high, the Financial Institution may experience
difficulty repaying Deposits if unusual circumstances arise. The
observed LTD range is 50% (very liquid) to 175% (illiquid).

Total Loans held are compared to Deposits held. If Total Loans are \<
125% of Deposits held the stock is scored one point.

##### CHECK \#6: Level of bad loans (Net Charge Off Ratio \> 3%)?

The level of Bad Loans incurred by a Financial Institution is a key
indicator of the quality of loans made. A high level of Bad Loans may
indicate that the Financial Institution is engaged in overly risky
lending practices.

If Bad Loans written off is \< 3% of Total Loans held the stock is
scored one point.



**Income (Dividends)**
----------------------

The Income section of the SWS app provides an analysis of a company's
dividend (income) payments to its shareholders.

The app analyses the dividend payment in terms of its absolute level and
against other dividend payers. In addition the app analyses the
volatility and sustainability of the dividend.

Note that if a company pays a dividend of less than 0.5%, or no
dividend, no further Income checks are undertaken.

### Dividend Yield %

The Dividend Yield % is the annualised dividend paid expressed as a
function of the company's share price:

    Dividend Yield = Annualised Dividend paid ($) / Share Price

Note that the Dividend Yield % will change as the share price changes.

Data points used to in the Income analysis:

  **Data point**                             | **Notes**
  -------------------------------------------| ------------------------------------------
  Dividend yield (End of day to -10 years)   |  Annual
  Dividend per share (LTM to -10 years)      |  Annual, last reported
  Payout ratio                              |  Last reported
  Estimate of Dividend per Share (+3 years) |  Annual, from analyst consensus estimates
  Estimate of GAAP Earnings per Share (+3 years) |  Annual, from analyst consensus estimates
  
  Note: For an [American Depository Receipt (ADR)](https://en.wikipedia.org/wiki/American_depositary_receipt) or equivalent the dividend yield is derived from the the primary listing of the stock, not the ADR. 
  
##### CHECK \#1: Is the current dividend yield higher than the cash savings rate?

If the Dividend Yield is \> the cash savings rate (for the relevant
geography) the stock is scored one point.

##### CHECK \#2: Is the current dividend yield in the top 25% of dividend paying stocks?

If the Dividend Yield is within the top 25% of dividend paying stocks
(for the relevant geography) the stock is scored one point.

##### CHECK \#3: Has the dividend been volatile in the past 10 years?

To check for volatility SWS looks at the historical dividend per share
payments, if at any point in the last 10 years a drop of greater than 10%
has occurred the dividend is considered volatile. Note this check is
based on the per share dividend amounts paid, not the yield.

One point is scored if there have been no annual drops in DPS of more
than 10% in the past 10 years. This check also fails by default if the stock has been paying a dividend for less than 10 years.

##### CHECK \#4: Has the dividend increased in the past 10 years?

The current annualised dividend amount paid is compared to the
annualised dividend amount paid 10 years ago. This check also fails by default if the stock has been paying a dividend for less than 10 years.

If the current annualised dividend amount is \> the annual dividend
amount 10 years ago the stock is scored one point.

##### CHECK \#5: Are dividends paid well covered by Net Profit (or Net Income)?

The payout ratio (as defined below) is used to check if the dividend is
affordable by the company.

    Payout ratio = Dividends per share / Earnings per share

If the payout ratio is greater than 0% and less than 90% the stock is
scored one point, in the case of REITs this threshold is 100%.

##### CHECK \#6: Are future expected dividends paid well covered by Net Profit (or Net Income)?

To check for future dividend coverage the payout ratio in 3 years’ time
is estimated. This is done using consensus analyst estimates for
Dividend per share payments and Earnings per share.

If the estimated payout ratio in 3 years is greater than 0% and less
than 90% the stock is scored one point, in the case of REITs this threshold is 100%.

**Management**
--------------

Metrics related to company management are not incorporated in the
Snowflake, however are included within the app as additional information
to assist with investment decision making.

The Management checks are designed to highlight whether CEO compensation
is reasonable and consistent with company performance. If CEO
compensation is out of step with company performance or the marketplace,
this may indicate that management's interests are not well aligned with
the company or shareholders.

In addition we provide an analysis of management tenure as an indicator
of stability and alignment with the company and shareholders. If
management or Board tenure is relatively short, this may indicate
instability or uncertainty within the company.

We finally analyse recent (up to 12 months) "insider" (ie The Board and
Management) share purchases and sales in the company. If company
insiders are net sellers of shares this may indicate a lack of
confidence in the future prospects for the company.

The following data is used in the SWS management analysis:

  **Data point**                                           | **Notes**
  ---------------------------------------------------------| ----------------------------------------------------------------------------
  Historical CEO total compensation (LTM to -5 years)     |  Annual, last reported
  GAAP Earnings per Share (LTM to -5 years) |  Annual, last reported
  Management team average tenure                          |  Calculated by averaging the tenure of the top 10 ranked ‘Professionals’
  Board of directors average tenure                       |  Calculated by averaging the tenure of the top 10 ranked Board of directors
  Number of shares sold by insiders                       |  Last reported, includes options exercised
  Number of shares bought by insiders                     |  Last reported, includes options exercised

##### CHECK \#1: Is the CEO's compensation unreasonable compared to market cap and earnings?

Whilst extensive analysis on CEO compensation exists there is no
industry standard metric or ratio to check for unreasonable levels
compared to company performance. We based our check on an excellent
article from
[Fool.com](http://www.fool.com/investing/general/2014/07/19/are-ceos-worth-the-millions-of-dollars-theyre-paid.aspx)
in 2014.

(From the Fool.com)

In 2013, the average S&P 500 CEO earned $10.5 million, a new record.
Total profits of S&P 500 companies were about $1 trillion, or $2
billion on average, meaning the average CEO's compensation was about
0.5% of the company's profit, or 0.03% of market cap, which is about
$35 billion on average. Since executive pay seems like it should be
tied to company profits and market value, perhaps we should use that as
a starting point.

Therefore this check is flagged if the following occurs:

    CEO Comp > (0.5% * Net Income + 0.03% * Market Cap)

##### CHECK \#2: Has the CEO's compensation increased more than 20% whilst the EPS is down more than 20%?

The increase in CEO compensation over the most recent financial period
is compared to the movement in company earnings per share (EPS) over the
most recent financial period.

If CEO compensation has increased more than 20%, and the company's EPS
has fallen more than 20%, this check is flagged.

##### CHECK \#3: Is the average tenure of the management team less than 2 years?

If the average tenure of the management team on average is \< 2 years
this check is flagged.

##### CHECK \#4: Is the average tenure of the Board of Directors team less than 3 years?

If the average tenure of the Board of Directors is \< 3 years this check
is flagged.

##### CHECK \#5: Are company "insiders" net buyers or sellers of the company's shares?

If company "insider" share sales is greater than the number of share
purchases this check is flagged. Insider trading activity is defined as a transaction from an internal stakeholder with an interest in the companies’ stock performance. Insiders can be individuals or corporates.

##### What transactions are included in this check?
The following transactions are included in the Insider Trading check:
* Open Market Acquisition (Buy)
* Open Market Disposition (Sell)

Equivalent to transaction type P/S on an SEC [Form 4](https://www.sec.gov/about/forms/form4data.pdf) filing.

Industry Averages
-----------------

Industry averages are calculated by region on a weekly basis. The
calculation for each data point is weighted by market cap.

Currency
--------

Any currency conversions are undertaken using end of day conversion
rates.
