## Feb 2019: Our Automated Intrinsic Value estimates are about to get better

Our automated estimates of intrinsic value provide a quick view of how the company’s financial performance, and analyst estimates, translate to underlying value. Our current calculation works well for stable businesses, but it often doesn’t fully capture the value that fast growing businesses can create. 

So on Monday the 25th of February we’re rolling out a few small, but powerful, changes. 

Our new automated intrinsic value estimate will include three significant changes:

*  Extend the high-growth stage from five years to ten years
*  Use a new ‘growth curve’ to reach the long-run growth rate
*  Use an improved ‘adjusted’ historical free cash flow 

### #1: Extended high-growth stage

The 2-Stage Free Cash Flow Model uses two stages. In the first stage, estimates of levered free cash flow to equity are used, which is sourced from market analyst consensus estimates. If no estimates are available, then the last estimate or reported value is extrapolated using the historical average annual growth rate.

In the second stage, a terminal value is calculated using the Gordon Growth formula, with an assumption that the company will continue to grow its earnings at the 10-year government bond rate, forever. The sum of the cash flow arising from the forecasts are then discounted to today's value using a discount rate, then divided by shares on issue, giving a value per share.

With this update we will increase the high-growth stage from five years to ten years. This will better reflect that growing businesses usually continue to grow at a moderate pace, before eventually slowing to the long-run growth rate.

### #2: Use a new growth curve to reach the long-run growth rate

Wherever possible, we use market analyst consensus estimates as the basis of our free cash flow forecasts. If no estimates are available, then the last estimate or reported value is extrapolated using the historical average annual growth rate. The following years are then forecast to grow, but with the growth rate reducing each year, until it reaches the long-run stable growth rate. 



### #3: Adjusted historical free cash flow

When no analyst forecasts are available we will smooth out the latest historical free cash flow numbers. Free cash flow is calculated as:

    Free Cash Flow = Operating Cash Flow - Capital Investments

Capital investments can be lumpy. In some years a new factory is needed, in others it isn’t. To adjust for this our automated intrinsic value estimate will be based on the growth in an adjusted free cash flow result:

    Adjusted Free Cash Flow = Operating Cash Flow - Three year average rate of Capital Investment

In addition to these improvements, we have also improved our beta estimates, risk free rates, and equity risk premium data points.

### Which companies will be most affected?

##### High Growth

Companies that are growing free cash flow significantly faster than GDP will likely have a higher automated intrinsic value estimate. This is because they will now be forecast to grow for a longer period before reaching the terminal stable growth rate:
![High Growth Company Example](https://simplywall.st/build/images/landing/dcf-high-growth.png "High Growth Company Example")

##### Stable Growth

Companies that are growing free cash flow at around the same pace as GDP will not see a substantial change from the update: 
![Stable Growth Company Example](https://simplywall.st/build/images/landing/dcf-stable-growth.png "Stable Growth Company Example")

##### Declining Growth

Companies with declining free cash flow will likely have a lower automated valuation estimate. This is because the free cash flows will now decline over a longer period before reaching stable growth:
![Declining Growth Company Example](https://simplywall.st/build/images/landing/dcf-decline-growth.png "Declining Growth Company Example")

### Ok, cool. Can you show me a worked example of the new method?

Sure!

Below is an example calculation for Amazon (NASDAQGS:AMZN) from 14/2/2019. Note the details of the calculation can be found for any stock on SWS by clicking Learn More or by clicking the valuation infographic.

**10 year cash flow forecast**

| Year | Levered FCF (USD, Millions) | Source | Present Value Discounted (@ 11.99%) | 
| ---- | ---- | ---- | ---- |
| 2019 | 27,209 | Analyst x12 | 24,296 |
| 2020 | 37,268 | Analyst x9 | 29,716 |
| 2021 | 46,213 | Analyst x4 | 32,903 |
| 2022 | 58,129 | Analyst x3 | 36,956 |
| 2023 | 70,986 | Analyst x3 | 40,298 |
| 2024 | 81,470 | Est @ 14.77% | 41,299 |
| 2025 | 90,560 | Est @ 11.16% | 40,992 |
| 2026 | 98,374 | Est @ 8.63% | 39,762 |
| 2027 | 105,122 | Est @ 6.86% | 37,940 |
| 2028 | 111,030 | Est @ 5.62% | 35,783 |

    Present value of next 10 years cash flows: $359,949

**Terminal Value**

    Terminal Value = FCF2028 × (1 + g) ÷ (Discount Rate – g)
    Terminal Value = $111,030 × (1 + 2.73%) ÷ (11.99% – 2.73%)
    Terminal value based on the Perpetuity Method where growth (g) = 2.73%: 1,231,872

    Present value of terminal value: $397,010

**Equity Value**

    Equity Value (Total value) = Present value of next 10 years cash flows + terminal value ($359,949 + $397,010)
    Value per share = Total value / Shares Outstanding  ($756,960.14 / 488.96)

    ∴ Value per share: $1,548

**New Discount**

New discount = (share price of $1,670.43): -7.9%

### Old Method Worked Example

And here is the same calculation performed using the current valuation method:

| Year | Levered FCF (USD, Millions) | Source | Present Value Discounted (@ 15.58%) | 
| ---- | ---- | ---- | ---- |
| 2019 | 27,209 | Analyst x12 | 24,736 |
| 2020 | 37,268 | Analyst x9 | 30,801 |
| 2021 | 46,213 | Analyst x4 | 34,721 |
| 2022 | 58,129 | Analyst x3 | 39,703 |
| 2023 | 70,986 | Analyst x3 | 44,077 |

    Present value of next 5 years cash flows: $148,361

**Terminal Value**

    Terminal Value = FCF2023 × (1 + g) ÷ (Discount Rate – g)
    Terminal Value = $70,986 × (1 + 2.73%) ÷ (15.58% – 2.73%)
    Terminal value based on the Perpetuity Method where growth (g) = 2.73%: 567,504

    Present value of terminal value: $322,171

**Equity Value**

    Equity Value (Total value) = Present value of next 5 years cash flows + terminal value ($148,361 + $311,171)
    Value = Total value / Shares Outstanding  ($470,532 / 488.96)

    ∴ Value per share: $962

**Old Discount**

Old discount = (share price of $1,670.43): -73.6%



## Further Examples of Model Changes

| Ticker        |  Company  | Old Discount to DCF | New Discount to DCF | Difference |
|---------------|:---------:|--------------------:|---------------------|------------|
| NASDAQGS:AMZN |   Amazon  |              -73.6% | -7.9%               | 65.7%      |
| NASDAQGS:AAPL |   Apple   |              -17.6% | 4.9%                | 22.5%      |
| NASDAQGS:MSFT | Microsoft |              -60.9% | -17.0%              | 43.9%      |
| NYSE:V        | Visa      | -55.6%              | -12.2%              | 43.3%      |
