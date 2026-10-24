# Foreign Outflows, Domestic Inflows and the Indian Equity Market

Independent research on whether domestic institutional investors (DII) now absorb selling by foreign portfolio investors (FPI) in Indian equities, and how those flows relate to Nifty 50 returns, SIP growth and macro conditions.

**Period:** January 2017 to September 2026 (117 complete months)
**Status:** Preliminary. See [Limitations](#limitations).

## 1. Research question

Is the Indian equity market becoming less dependent on foreign capital because domestic capital is growing?

The work tests four connected questions:

1. Do DIIs (mutual funds, insurers) buy enough to offset FPI selling?
2. How does the Nifty behave when foreigners are selling?
3. Has the domestic savings base, measured by SIP inflows and mutual fund AUM, grown enough to support this?
4. How do the rupee, inflation and the repo rate relate to flows and returns?

## 2. Data

| Series | Source | Frequency |
| --- | --- | --- |
| FPI net equity flow (Rs crore) | NSDL | Monthly |
| DII net equity flow (Rs crore) | Trendlyne monthly table | Monthly |
| Nifty 50 close | NSE | Daily, aggregated to month-end |
| SIP contributions (Rs crore) | AMFI | Monthly |
| Equity mutual fund AUM (Rs crore) | AMFI | Quarterly |
| USD/INR, repo rate, CPI inflation | RBI, MoSPI | Monthly |

October 2026 is a partial month (to 23 October) and is excluded from all statistics.

## 3. Method

- **Fully offset month:** a month in which FPI net flow is negative and DII net buying is at least equal to the absolute value of that selling.
- **Offset ratio:** DII net buying divided by FPI net selling.
- **Nifty return:** month-end close divided by the previous month-end close, minus one.
- **USD/INR change:** month-end rate divided by the previous month-end rate, minus one. A positive value means rupee depreciation.
- **Tests:** group averages by flow regime, a stress test of the ten largest outflow months, and Pearson and Spearman correlations with robustness checks (trimmed sample, sub-periods).
- Missing data is left blank, never set to zero. All figures in the workbook are calculated by live formulas from the Monthly Data tab.

## 4. Results

### 4.1 Domestic buying usually covers foreign selling

FPI was a net seller in 53 of 117 months. DII buying fully offset the selling in 42 of them, an offset rate of 79%.

| Period | FPI-selling months | Fully offset | Offset rate |
| --- | --- | --- | --- |
| 2017 to 2019 | 13 | 11 | 85% |
| 2020 to 2023 | 21 | 13 | 62% |
| 2024 to Sep 2026 | 19 | 18 | 95% |

The offset rate dipped during 2020 to 2023 and has been highest since 2024.

### 4.2 Offsetting does not mean a rising market

| Flow regime | Months | Average Nifty return | Months with positive return |
| --- | --- | --- | --- |
| FPI net sellers (all) | 53 | -1.08% | 31% |
| of which fully offset by DII | 42 | -1.33% | 27% |
| of which not fully offset | 11 | -0.16% | 45% |
| FPI not selling | 64 | +2.61% | 77% |

Months with full domestic offset still averaged a fall. Domestic buying absorbed the selling but did not prevent weak months.

### 4.3 The largest outflow months are harder to absorb

| Group | Selling months | Fully offset | Offset rate | Average Nifty return |
| --- | --- | --- | --- | --- |
| 10 largest FPI-selling months | 10 | 6 | 60% | -3.95% |
| All other FPI-selling months | 43 | 36 | 84% | -0.39% |

The ten largest outflow months were March 2026, October 2024, January 2025, March 2020, April 2026, June 2022, June 2026, March 2022, May 2022 and January 2026. The group is small, so treat the result as indicative.

### 4.4 Flows and returns move differently

Same-month correlation with the Nifty monthly return:

| Series | Pearson r | Spearman rho |
| --- | --- | --- |
| FPI net flow | +0.53 | +0.50 |
| DII net flow | -0.47 | -0.45 |
| FPI + DII combined | +0.07 | +0.06 |

Foreign flows move with the market. Domestic flows move against it, which is consistent with domestic institutions buying into weakness. This is an interpretation, not a tested result.

### 4.5 The domestic savings base has grown

- Monthly SIP contributions rose from Rs 4,095 crore (Jan 2017) to Rs 32,490 crore (Sep 2026), about 7.9 times.
- Equity mutual fund AUM rose from Rs 5.4 lakh crore (Mar 2017) to Rs 37.9 lakh crore (Jun 2026), about 7 times. AUM growth includes market appreciation, not only new money.
- Across FPI-selling months, SIP level correlates +0.26 with a full offset and -0.04 with the offset ratio. Both series trend upward, so the link is weak.

### 4.6 The rupee is the macro variable most linked to returns

| Indicator vs Nifty return | Months | Pearson r |
| --- | --- | --- |
| USD/INR monthly change | 107 | -0.52 |
| Repo rate | 108 | -0.06 |
| CPI inflation (YoY) | 116 | +0.03 |

The USD/INR relationship holds under robustness checks:

| Test | Months | Pearson r |
| --- | --- | --- |
| All complete months | 107 | -0.52 |
| Excluding outer 2.5% tails | 97 | -0.37 |
| 2017 to 2019 | 26 | -0.39 |
| 2020 to 2023 | 48 | -0.66 |
| 2024 to Sep 2026 | 33 | -0.61 |

Months of larger rupee depreciation tended to be months of weaker equity returns.

## 5. Analysis and conclusion

Domestic institutions have regularly bought more than foreigners sold, and more reliably in recent years, in line with a much larger SIP-funded savings base. But offsetting net flows is not the same as protecting the market: offset months still averaged a fall, and the largest outflow months were both harder to cover and followed by much weaker returns.

My reading is that domestic capital now cushions foreign selling but does not neutralise it. Currency weakness is the macro factor most closely associated with weak equity months.

All results describe association, not cause. Foreign selling, domestic buying and returns can all respond to the same underlying conditions, such as global risk sentiment.

## Limitations

- **Mixed flow sources.** FPI flows are on a depository basis and DII flows are on an exchange basis, so the two series may not be strictly comparable. For July 2026 the FPI figure used here is +Rs 20,200 crore, against about -Rs 5,779 crore in exchange cash-market data. Offset rates and flow correlations are preliminary until both series are rebuilt from the NSE combined FII/FPI and DII cash-market report. The SIP, Nifty and macro results do not depend on this.
- **Small groups.** The ten-month stress test and sub-period correlations rest on few observations.
- **SIP figures** are gross contributions, not net equity purchases.
- **No causal claim** is made.

## Next steps

1. Rebuild FPI and DII monthly flows from one NSE cash-market series and rerun every result.
2. Test lagged relationships between flows and returns.
3. Add global controls such as the US dollar index.
4. Add a daily view of the largest outflow months.

## Repository contents

- `FPI_DII_Flow_Analysis.xlsx`: seven tabs
  - **Summary:** headline figures and charts
  - **Findings:** seven findings with result, reading and limitation
  - **Offset Analysis:** offset rates, regime returns and stress test
  - **Correlations:** flow and macro correlations with robustness checks
  - **Annual Summary:** year-by-year flows, offsets and SIP
  - **Monthly Data:** source data and calculated columns
  - **Method & Sources:** definitions, sources and limitations

## Tools

Excel (formulas and charts), Python (pandas).
