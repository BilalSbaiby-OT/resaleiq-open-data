# Resale IQ open data: Vinted asking prices and listing departures

Independent data from [Resale IQ](https://resaleiq.dev), a price-check and offer-coaching tool for Vinted and eBay resellers. Not affiliated with Vinted or eBay.

Licence: [CC BY 4.0](LICENSE). Credit: "Source: Resale IQ, https://resaleiq.dev/data, September 2026".

## What the numbers are (read this first)

- **Prices are asking prices** that sellers typed on Vinted listings. They are not sold prices. We never call them sales.
- **A "departure"** is a listing that left the public feed during the month (sold, deleted, hidden or expired: we cannot tell which). `departure_share_pct` is a brand's share of all departures in the month, not a sell-through rate.
- Data comes from our own crawl of public Vinted listing pages, repeated passes per market. No user accounts are scraped.
- Medians and quartiles are in euros. Small samples are wide: read `departures_n` / `n` before quoting a row.

## Files

| File | Content |
|---|---|
| `secondhand-price-index-2026-09.csv` | Brand and brand-category rows for September 2026: departures, median / p25 / p75 asking price (EUR), departure share, a demand index (100 = the busiest brand) |
| `vinted-demand-index-2026-10-stats.csv` | Headline counts behind the Vinted demand index page (listings recorded per market, as of 5 Oct 2026) |
| `vinted-price-tags-2026-10-05.csv` | 5-11 Oct 2026, 1,345 tracked-brand listings that left the feed: share of asking prices that are a multiple of EUR 5 (78.5% overall, 95% CI 76.2-80.6) by market, price band and brand (min 100 per brand), plus the most common exact prices |

Live, updated versions and the method: https://resaleiq.dev/data and https://resaleiq.dev/facts

## Use it

Journalists, bloggers, resellers and researchers can quote or chart any of it with the credit line above. If you find an error, tell us: support@resaleiq.dev
