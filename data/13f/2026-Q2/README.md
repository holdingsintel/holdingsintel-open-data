# Q2 2026 13F edition

What 546 funds reported holding at the end of Q2 2026 (June 30, 2026), from their SEC 13F filings.

- 546 funds reporting $65T in US-listed equities
- The 1,000 largest stocks by reported value, 90.2% of the funds' reported value
- Each fund's 10 largest holdings

Read the [Q2 2026 Smart Money Report](https://www.holdingsintel.com/reports/2026-Q2) for the quarter's biggest moves.

## Files

### stocks.csv (1,000 rows)

One row per stock, largest reported value first.

| Column | Meaning |
| --- | --- |
| `quarter` | Calendar quarter of the 13F filings, e.g. 2026-Q2. |
| `period_end` | Quarter-end date the holdings are reported as of. |
| `cusip` | CUSIP of the security, as filed. |
| `ticker` | Ticker, where one is known. |
| `issuer` | Issuer name. |
| `funds_holding` | Tracked funds reporting the stock at quarter end. |
| `funds_opened` | Funds reporting a position they did not report the quarter before. |
| `funds_added` | Funds that reported more shares than the quarter before. |
| `funds_trimmed` | Funds that reported fewer shares than the quarter before. |
| `funds_exited` | Funds that reported the stock the quarter before and not this quarter. |
| `flows_withheld` | split or cusip_change when a stock split or CUSIP change in the quarter makes share counts incomparable; the four flow columns are then blank. |
| `reported_value_usd` | Sum of the tracked funds' reported values, in US dollars. |
| `holdingsintel_url` | The stock's page on HoldingsIntel. |

### funds.csv (546 rows)

One row per fund, largest reported value first.

| Column | Meaning |
| --- | --- |
| `quarter` | Calendar quarter of the 13F filing. |
| `period_end` | Quarter-end date the holdings are reported as of. |
| `cik` | The fund's SEC Central Index Key. |
| `fund` | Fund name as filed with the SEC. |
| `reported_value_usd` | Reported value of the fund's US equity holdings (options excluded), in US dollars. |
| `positions` | Number of equity positions reported. |
| `filed_date` | Date the 13F filing used here was filed. |
| `accession_number` | SEC accession number of that filing. |
| `sec_filing_url` | The filing on SEC EDGAR. |
| `holdingsintel_url` | The fund's page on HoldingsIntel. |

### fund_top_holdings.csv (5,383 rows)

Each fund's 10 largest holdings, as its HoldingsIntel page shows them.

| Column | Meaning |
| --- | --- |
| `quarter` | Calendar quarter of the 13F filing. |
| `period_end` | Quarter-end date the holding is reported as of. |
| `cik` | The fund's SEC Central Index Key. |
| `fund` | Fund name as filed with the SEC. |
| `rank` | 1 is the fund's largest holding by reported value. |
| `cusip` | CUSIP of the security, as filed. |
| `ticker` | Ticker, where one is known. |
| `issuer` | Issuer name. |
| `reported_value_usd` | Reported value of the holding, in US dollars. |
| `portfolio_weight_pct` | Share of the fund's reported equity value, in percent. |
| `sec_filing_url` | The fund's 13F filing on SEC EDGAR. |
| `holdingsintel_url` | The stock's page on HoldingsIntel. |

## Method

- Holdings and values are as each fund reported them to the SEC, in US dollars. Equity positions only: put and call options are excluded.
- `stocks.csv` lists shares and ETFs: bonds, convertible notes, warrants, rights and options are left out.
- Each fund's latest filing for the quarter is the one linked, amendments included.
- Flow counts compare each fund's reported shares with its own previous quarter.
- A stock split or a CUSIP change resets share counts, so for those stocks the flow columns are blank and `flows_withheld` names the event (13 stocks this quarter). Holders and reported value stay exact.

## Cite

HoldingsIntel (2026). *HoldingsIntel Smart Money Open Data*, edition 13f-2026-Q2. https://github.com/holdingsintel/holdingsintel-open-data. CC BY 4.0.

Explore every fund and stock at [holdingsintel.com](https://www.holdingsintel.com).
