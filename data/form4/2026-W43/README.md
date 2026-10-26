# Form 4 edition 2026-W43

Open-market stock purchases and sales that company insiders filed with the SEC from October 19, 2026 to October 25, 2026.

- 85 purchase filings, $34.4M at reported prices
- The 250 largest of 321 sale filings, $2.6B at reported prices

See every insider trade as it is filed at [holdingsintel.com/insiders](https://www.holdingsintel.com/insiders).

## Files

### open_market_filings.csv (335 rows)

One row per Form 4 filing and direction, purchases first, each largest value first.

| Column | Meaning |
| --- | --- |
| `week` | ISO week of the filing date, e.g. 2026-W42. |
| `filing_date` | Date the Form 4 was filed. |
| `first_transaction_date` | Earliest transaction date in the filing for this direction. |
| `last_transaction_date` | Latest transaction date in the filing for this direction. |
| `insider` | Reporting person, as filed. |
| `insider_cik` | Reporting person's SEC CIK. |
| `relationship` | Relationship to the issuer: Director, Officer, 10% Owner or Other. |
| `title` | Officer title, where filed. |
| `issuer` | Company whose shares were traded. |
| `issuer_cik` | Issuer's SEC CIK. |
| `ticker` | Issuer ticker, as filed. |
| `direction` | purchase (code P) or sale (code S), open market only. |
| `transactions` | Transaction lines summed into this row. |
| `shares` | Total shares traded. |
| `value_usd` | Total value at the reported prices, in US dollars; blank when a line has no price. |
| `avg_price_usd` | Share-weighted average price. |
| `accession_number` | SEC accession number of the Form 4. |
| `sec_filing_url` | The filing on SEC EDGAR. |
| `holdingsintel_url` | The stock's page on HoldingsIntel, where one exists. |

## Method

- Open-market purchases (transaction code P) and sales (code S) of common stock, filed by individual insiders. Grants, option exercises, gifts, private placements and filings by entities are excluded.
- A filing's transaction lines in the same direction are summed into one row.
- Up to 250 filings per direction, by value. Filings with an implausible line (over $10B, or over $100,000 a share) are left out whole.
- The week runs Monday to Sunday by filing date.

## Cite

HoldingsIntel (2026). *HoldingsIntel Smart Money Open Data*, edition form4-2026-W43. https://github.com/holdingsintel/holdingsintel-open-data. https://doi.org/10.5281/zenodo.23606240. CC BY 4.0.
