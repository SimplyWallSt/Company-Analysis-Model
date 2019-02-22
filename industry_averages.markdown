 Simply Wall St Industry Averages Calculation Methodology
=========================================================

We update our industry averages every 6 hours, for 68 industries, in every country and region we cover. Depending on the metric we use different calculation types, which are detailed below. In some cases we might use multiple calculations on the same metric depending on where it is being used.

In the case of industry groups with less than five companies, we use the regional average for that industry instead. If there are less than five companies in that region then we use the global average. This method allows us to provide more meaningful averages ensuring the data is rich and precise, as well as providing alternatives for small industries of companies with lack of analyst coverage or general macroeconomic variables available for analysis.

We also calculate the averages across the entire market in each country we cover, this allows us to find the median PE Ratio for New Zealand for example.

We include all primary listed companies in each market/ region in our averages, this means for companies with listings in many countries (e.g. Royal Dutch Shell) the country of their primary listing (usually their headquarters) is used. This is to give a better comparison to the rest of the market for investors in each country. Funds and depositary receipts are excluded. 

To give an example of this for NZX:AIA (Auckland International Airport), an infrastructure company based in New Zealand:

#### Industry PE Ratio Example for NZX:AIA (Auckland International Airport)
As there are only 4 infrastructure companies listed in New Zealand (on NXZ: AIA, MMH, SPN & POT) we instead use the Oceania average, which includes Australia and gives us 9 companies in total (add from the ASX: ALX, TCL, SYD, QUB and TTI). 

For PE Ratio we only look at profitable companies and we use the median instead of a weighted average. We use median instead of a weighted average as provides a better comparable (see our [company analysis model](https://github.com/SimplyWallSt/Company-Analysis-Model/blob/master/MODEL.markdown#pe-ratio--how-is-this-calculated)) and doesn't skew the result towards large market caps.

#### Market PE Ratio Example for NZX:AIA (Auckland International Airport)
At the time of writing there are 104 profitable companies listed in New Zealand, which means we can calculate a meaningful median PE Ratio for the market.

(Note the example above are correct at time of writing, June 2018)

## Calculation Methods

Depending on the metric being averaged we use one of the following calculation methods. Some metrics we also define a set of thresholds that restrict meaningless values and anomalies.

* Count (count of the eligible companies)
* Count Positive (count of the eligible companies where the relevant metric is positive)
* Average Weighted Market Cap (where Market Cap is in converted to USD to handle cross listing)
* Average
* Median
* Median Profitable (Median only including profitable companies)
* Median Profitable Analyst Coverage (Median only including profitable companies and those with analyst coverage)
* Xth Percentile

## Market Cap Groupings
We use the following thresholds to define our market cap groups based on the distribution of companies globally. Remember all market caps are converted to USD for consistency:
* Small cap: $0 - $500M (~21,000 companies)
* Mid cap: $500M - $5B (~5000 companies)
* Large cap: >$5B (~2000 companies)

For consistency these are used regardless of country, meaning in some countries many of the companies would be considered small cap on a global scale.

## Metrics List

| **Metric** | **Calculation Type** | **Limits** | **Market Cap Group** |
| --- | --- | --- | --- |
| Eps Growth Annual | Average Weighted Market Cap |  |  |
| Net Income Growth Annual | Average Weighted Market Cap |  |  |
| Cash Ops Growth Annual | Average Weighted Market Cap |  |  |
| Revenue Growth Annual | Average Weighted Market Cap |  |  |
| Total Base Count | Count |  |  |
| Profitable Count | Count Positive |  |  |
| Analyst Coverage Count | Count Positive |  |  |
| Market Cap | Average |  |  |
| Dividend Count | Count Positive |  |  |
| Beta Count | Count | Min:0.2 Max:4 |
| Value Score | Average Weighted Market Cap |  |  |
| Future Score | Average Weighted Market Cap |  |  |
| Past Score | Average Weighted Market Cap |  |  |
| Health Score | Average Weighted Market Cap |  |  |
| Dividend Score | Average Weighted Market Cap |  |  |
| Total Score | Average Weighted Market Cap |  |  |
| Share Price | Average Weighted Market Cap |  |  |
| Analyst Count | Average Weighted Market Cap |  |  |
| Debt Equity | Average Weighted Market Cap |  |  |
| Insider Buying | Average Weighted Market Cap |  |  |
| Levered Beta | Average Weighted Market Cap | Min:0.2 Max:4 |
| Eps | Average Weighted Market Cap | Min:0 |  |
| Intrinsic Discount | Average Weighted Market Cap |  |  |
| Unlevered Beta | Average Weighted Market Cap | Min:0.2 Max:4 |
| Dividend Yield | Average Weighted Market Cap | Min:0 Max:12 |
| Future Dividend Yield | Average Weighted Market Cap | Min:0 Max:12 |
| Levered Beta Median | Median | Min:0.2 Max:4 |
| Pe | Median Profitable |  |  |
| Peg | Median Profitable |  |  |
| Pb | Median |  |  |
| Roe | Median Profitable |  |  |
| Roa | Median Profitable |  |  |
| Growth Past 1Y | Median Profitable |  |  |
| Growth Past 5Y | Median Profitable |  |  |
| Growth Future 1Y | Median Profitable Analyst Coverage |  |  |
| Growth Future 3Y | Median Profitable Analyst Coverage |  |  |
| Price To Sales | Median |  |  |
| Ev To Ebitda | Median | Min:0 |  |
| Ev To Sales | Median |  |  |
| Return 7D | Average Weighted Market Cap |  |  |
| Return 30D | Average Weighted Market Cap |  |  |
| Return 90D | Average Weighted Market Cap |  |  |
| Ebitda 1Y | Median | Min:0 |  |
| Ebitda Growth 1Y | Average Weighted Market Cap |  |  |
| Forward Pe 1Y | Median Profitable Analyst Coverage |  |  |
| Forward Price To Sales 1Y | Median |  |  |
| Forward Ev To Ebitda 1Y | Median Profitable Analyst Coverage |  |  |
| Forward Ev To Sales 1Y | Median |  |  |
| Gross Profit Margin 1Y | Median Profitable |  |  |
| Net Income Margin 1Y | Median Profitable |  |  |
| Ebit Margin | Median | Min:0 |  |
| Ebitda Margin | Median | Min:0 |  |
| Gross Profit Margin | Median Profitable |  |  |
| Capex | Median |  |  |
| Capex Growth 1Y | Average Weighted Market Cap |  |  |
| Capex Growth Annual | Average Weighted Market Cap |  |  |
| Net Debt | Median |  |  |
| Management Rate Return | Average Weighted Market Cap |  |  |
| Dividend Yield Growth Annual | Average Weighted Market Cap |  |  |
| Dividend Yield Future | Average Weighted Market Cap |  |  |
| Ceo Compensation Total | Median |  |  |
| Ceo Compensation Salary | Median |  |  |
| Ceo Salary Growth 1Y | Median |  |  |
| Management Tenure | Median |  |  |
| Board Tenure | Median |  |  |
| Management Age | Median |  |  |
| Board Age | Median |  |  |
| Total Base Count Small | Count |  | Small |
| Total Base Count Medium | Count |  | Medium |
| Total Base Count Large | Count |  | Large |
| Ceo Compensation Total Small | Median |  | Small |
| Ceo Compensation Total Medium | Median |  | Medium |
| Ceo Compensation Total Large | Median |  | Large |
| Ceo Compensation Salary Small | Median |  | Small |
| Ceo Compensation Salary Medium | Median |  | Medium |
| Ceo Compensation Salary Large | Median |  | Large |
| Ceo Salary Growth 1Y Small | Median |  | Small |
| Ceo Salary Growth 1Y Medium | Median |  | Medium |
| Ceo Salary Growth 1Y Large | Median |  | Large |
| Return 30D Small | Median |  | Small |
| Return 30D Medium | Median |  | Medium |
| Return 30D Large | Median |  | Large |
| Capex Small | Median |  | Small |
| Capex Medium | Median |  | Medium |
| Capex Large | Median |  | Large |
| Net Income | Median |  |  |
| Net Income Small | Median |  | Small |
| Net Income Medium | Median |  | Medium |
| Net Income Large | Median |  | Large |
| Revenue | Median |  |  |
| Revenue Small | Median |  |  |
| Revenue Medium | Median |  |  |
| Revenue Large | Median |  |  |
| Profitable Count Small | Count Positive |  | Small |
| Profitable Count Medium | Count Positive |  | Medium |
| Profitable Count Large | Count Positive |  | Large |
| Payout Ratio | Median Profitable |  |  |
| Dividend Yield P10 | 10th Percentile | Min:0 Max:12 |
| Dividend Yield P25 | 25th Percentile | Min:0 Max:12 |
| Dividend Yield P50 | Median | Min:0 Max:12 |
| Dividend Yield P75 | 75th Percentile | Min:0 Max:12 |
| Dividend Yield P90 | 90th Percentile | Min:0 Max:12 |
| Market Cap P25 | 25th Percentile |  |  |
| Market Cap P50 | Median |  |  |
| Market Cap P75 | 75th Percentile |  |  |
| Net Income Growth Annual P25 | 25th Percentile | Min:0 |  |
| Net Income Growth Annual P75 | 75th Percentile | Min:0 |  |
| Roe P25 | 25th Percentile | Min:0 |  |
| Roe P75 | 75th Percentile | Min:0 |  |
| Pe P25 | 25th Percentile | Min:0 |  |
| Pe P75 | 75th Percentile | Min:0 |  |
| Return 30D P10 | 10th Percentile |  |  |
| Return 30D P25 | 25th Percentile |  |  |
| Return 30D P75 | 75th Percentile |  |  |
| Return 30D P90 | 90th Percentile |  |  |
| Ceo Age P25 | 25th Percentile |  |  |
| Ceo Age P75 | 75th Percentile |  |  |
| Year Founded P25 | 25th Percentile |  |  |
| Year Founded P75 | 75th Percentile |  |  |
| Total Employees P25 | 25th Percentile |  |  |
| Total Employees P75 | 75th Percentile |  |  |
