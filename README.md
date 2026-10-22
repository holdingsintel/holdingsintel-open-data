# HoldingsIntel Smart Money SEC Filings

What hedge funds, company insiders and activist investors disclosed to the SEC, structured and ready to analyze: 13F holdings and their quarter-over-quarter changes, Form 4 insider trades, and Schedule 13D and 13G stakes above 5%.

Built by [HoldingsIntel](https://www.holdingsintel.com) from SEC EDGAR filings only. Free to use under [CC BY 4.0](./LICENSE).

## What's inside

| Folder | SEC source | One row is | Refreshed |
|---|---|---|---|
| `13f/` | Form 13F-HR and 13F-HR/A | One fund's position in one security for one quarter, with its change from the prior quarter | Four times a year, right after each 13F filing deadline (mid-February, May, August and November) |
| `insider/` | Form 4 | One insider transaction | Weekly |
| `activist/` | Schedules 13D and 13G | One ownership filing | Weekly |

13F coverage: the funds that hold 89% of US 13F-disclosed capital ($70.7T, Q2 2026). Every row carries the SEC accession number of the filing it comes from, so any figure traces back to EDGAR in one step. Each folder's `SCHEMA.md` lists its columns.

Each release is tagged by period and archived on Zenodo with its own DOI. The same files are on [Hugging Face](https://huggingface.co/datasets/holdingsintel/smart-money-sec-filings) and [Kaggle](https://www.kaggle.com/datasets/holdingsintel/smart-money-sec-filings).

## Explore it on HoldingsIntel

See the same funds, stocks and filings with the analysis done, from the Smart Money Verdict to fund ratings: [funds](https://www.holdingsintel.com/filers), [stocks](https://www.holdingsintel.com/stocks), [insider trades](https://www.holdingsintel.com/insiders), [activist filings](https://www.holdingsintel.com/activists). Congressional trades live at [holdingsintel.com/congress](https://www.holdingsintel.com/congress).

## How to cite

Cite the release you used, with its DOI:

> HoldingsIntel (2026). *HoldingsIntel Smart Money SEC Filings* [Data set]. Zenodo. https://doi.org/<DOI of the release>

GitHub's **Cite this repository** button gives the same citation from [`CITATION.cff`](./CITATION.cff).

## License

Data: [CC BY 4.0](./LICENSE). Use it, share it and build on it, commercially too; credit HoldingsIntel and the release you used. The underlying SEC filings are public records. Not investment advice.
