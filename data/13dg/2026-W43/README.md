# 13D and 13G edition 2026-W43

205 beneficial-ownership filings made with the SEC from October 19, 2026 to October 25, 2026: 58 Schedule 13D (an investor free to push for change) and 147 Schedule 13G (a passive stake).

Follow activist stakes as they are filed at [holdingsintel.com/activists](https://www.holdingsintel.com/activists).

## Files

### filings.csv (205 rows)

One row per filing, newest first.

| Column | Meaning |
| --- | --- |
| `week` | ISO week of the filing date, e.g. 2026-W42. |
| `filing_date` | Date the schedule was filed. |
| `event_date` | Date of the event that required the filing. |
| `form_type` | SCHEDULE 13D, 13D/A, 13G or 13G/A. |
| `filer` | Filing investor, as filed. |
| `filer_cik` | Filing investor's SEC CIK. |
| `subject_company` | Company whose shares are reported. |
| `subject_cik` | Subject company's SEC CIK. |
| `ticker` | Subject company ticker, where known. |
| `cusip` | CUSIP of the reported class, as filed. |
| `ownership_pct` | Percent of the class reported as beneficially owned. |
| `prev_ownership_pct` | The same filer's previously reported percent, where one exists. |
| `accession_number` | SEC accession number of the filing. |
| `sec_filing_url` | The filing on SEC EDGAR. |
| `holdingsintel_url` | The stock's page on HoldingsIntel, where one exists. |

## Method

- Schedules 13D and 13G and their amendments, as filed. Structural filings are excluded: any filing on an ETF or open-end fund, a sponsor reporting on its own fund, or a record holder reporting 90% or more of a class.
- Up to 300 filings per week, newest first.
- The week runs Monday to Sunday by filing date.

## Cite

HoldingsIntel (2026). *HoldingsIntel Smart Money Open Data*, edition 13dg-2026-W43. https://github.com/holdingsintel/holdingsintel-open-data. https://doi.org/10.5281/zenodo.23606240. CC BY 4.0.
