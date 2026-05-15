# FX Rates

If you hold assets in more than one currency, Tally Up uses exchange rates to convert balances and transaction amounts into your base currency for reporting. FX rates are fetched automatically and require no manual setup in most cases.

---

## Base currency

Your base currency is the currency used for all consolidated reports — net worth, performance, forecasts, and budgets. All other currencies are converted to it.

Set your base currency in **Settings → Base Currency**. Choose the currency that matches your primary financial life.

You can change your base currency at any time. Historical reports will recalculate using the appropriate historical rates.

---

## How rates are obtained

Tally Up fetches exchange rates automatically in the background for all currency pairs relevant to your assets. For example, if you have assets in GBP and USD and your base currency is EUR, Tally Up will maintain GBP/EUR and USD/EUR rate histories.

Rates cover both current and historical dates, so valuations and reports remain accurate across your full transaction history.

---

## Viewing rates

Go to **Settings → FX Rates** to browse stored exchange rates. You can filter by currency pair to inspect the data for a specific combination.

FX rates are read-only in this view — they are managed automatically by Tally Up.

---

## Data Feed settings

Go to **Settings → Data Feed** to configure how Tally Up fetches market data, including FX rates:

- **Automatic refresh** — enable to let Tally Up update rates in the background on a schedule
- **Refresh interval** — how frequently automatic updates run

---

## Sync and storage

Exchange rates are stored on your device only — they are not synced via iCloud. Each of your devices fetches rate history independently. This keeps your iCloud sync small, since rate history across all currency pairs can grow large over time.

---

## Tips

- Make sure your base currency is set correctly before adding assets in other currencies. Changing it later is safe, but worth getting right early.
- If a rate is missing for a specific date, Tally Up uses the nearest available rate as a fallback.
- FX rates are not included in plan exports — they are re-fetched automatically after an import completes.
