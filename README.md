# Bitcoin Historical Prices and Returns by Month and Year (Maketo)

Bitcoin daily prices since July 2010 and returns by month and year, from Maketo's daily price record.

**This copy ends on 31 Oct 2026.** Today's price and this month's return are on the live page:
**[Bitcoin Historical Returns by Month and Year](https://maketo.com/bitcoin/historical-returns)** at maketo.com, updated every day.

## Files

| File | Rows | What each row is |
|---|---|---|
| `bitcoin_daily_prices.csv` | 5,951 | One UTC day: open, high, low and close in US dollars, and the change from the day before. |
| `bitcoin_monthly_returns.csv` | 196 | One calendar month: open, high, low, close and the month's return. |
| `bitcoin_yearly_returns.csv` | 17 | One calendar year: first open, last close and the year's return. |

Every row has a `source_url`: the Maketo page that shows the same numbers, with the latest days added.

## Columns

- `date`: the UTC day, as YYYY-MM-DD.
- `open_usd`, `high_usd`, `low_usd`, `close_usd`: Bitcoin's price in US dollars. A day runs from 00:00 to 24:00 UTC.
- `change_pct`: the close against the day before's close, in percent. Empty on the first day.
- `return_pct`: in the monthly file, the month's first open to its last close, in percent. In the yearly file, the year's first open to its last close, in percent. A year's return is not the sum of its monthly returns.
- `full_year`: `no` for the year that is still running; its return covers only the months in this copy.

## How it is made

The prices come from Maketo's daily price record, which starts on 17 Jul 2010.
Maketo lists the markets behind the record at [maketo.com/sources](https://maketo.com/sources) and explains its method at
[maketo.com/methodology](https://maketo.com/methodology). Before each copy is published, every monthly and yearly return is
checked against the numbers on the live page.

## Licence and credit

CC BY 4.0 ([https://creativecommons.org/licenses/by/4.0/](https://creativecommons.org/licenses/by/4.0/)). You may copy, share and build on this data, including for commercial use,
as long as you credit Maketo with a link. Suggested credit:

> Source: Maketo, Bitcoin Historical Returns by Month and Year, https://maketo.com/bitcoin/historical-returns

## Updates

A new copy is published at the start of each month, ending on the last day of the month before.
The same data is on GitHub ([Maketocom/bitcoin-historical-returns](https://github.com/Maketocom/bitcoin-historical-returns)),
Hugging Face ([Maketocom/bitcoin-historical-returns](https://huggingface.co/datasets/Maketocom/bitcoin-historical-returns))
and Kaggle ([maketocom/bitcoin-historical-returns](https://www.kaggle.com/datasets/maketocom/bitcoin-historical-returns)).


## Permanent copy (DOI)

Every three months a copy is archived at Zenodo, under one permanent DOI: [10.5281/zenodo.24523486](https://doi.org/10.5281/zenodo.24523486). Researchers can cite that DOI; it always leads to the latest version.

This data is for learning and research. It is not financial advice.
