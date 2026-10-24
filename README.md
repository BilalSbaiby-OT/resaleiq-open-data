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
| `vinted-fees-by-country-2026-10.csv` | The buyer-side Vinted fee as printed on each of 22 country sites (percentage, fixed part in local currency and EUR, fee on a EUR 20 and a EUR 50 item), with the official sentence, its source page and the read date (`read_on`, 21 Oct 2026) on every row. A fee schedule, so it has no sample size |
| `resale-platform-fees-2026-10.csv` | Seller fee schedules of 25 marketplace variants from 12 platforms applied to a sale of 20, 50 and 100 in each platform's own currency (no conversion, no item cost or shipping), with the source page and the date it was read (`checked`, 4 or 8 Oct 2026) on every row. One variant (eBay AU) has empty fee cells because its fee could not be confirmed on the official page. Published schedules, not Resale IQ observations, so no sample size |
| `vinted-price-tags-2026-10-05.csv` | 5-11 Oct 2026, 1,345 tracked-brand listings that left the feed: share of asking prices that are a multiple of EUR 5 (78.5% overall, 95% CI 76.2-80.6) by market, price band and brand (min 100 per brand), plus the most common exact prices |

Totals: per-market rows do not add up to the `all` row (for example the five markets' departures in `secondhand-price-index-2026-09.csv` sum to more than the `all` departures, and the `market` rows in the price-tag file cover fewer listings than the 1,345 total). Quote a row with its own `n`, and do not add rows across markets.

Every price file carries a sample size (`departures_n` or `n`); every fee file carries the date its source was read.

Live, updated versions and the method: https://resaleiq.dev/data and https://resaleiq.dev/facts

## Use it

Journalists, bloggers, resellers and researchers can quote or chart any of it with the credit line above. If you find an error, tell us: support@resaleiq.dev
