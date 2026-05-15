# Securities

Securities represent the individual stocks, ETFs, funds, bonds, and other instruments that your investment assets hold. Tally Up tracks prices for each security so your portfolio value stays current.

---

## Managing securities

Go to **Settings → Securities** to view, add, edit, and delete securities.

### Adding a security

Tap **Add** and fill in:

| Field | Description |
|---|---|
| Symbol | Ticker symbol (e.g. `AAPL`, `VWRL`) |
| Name | A descriptive name |
| Currency | The currency the security trades in |
| Market | Optional exchange identifier (e.g. `NYSE`, `LSE`) |
| Type | Stock, ETF, Mutual Fund, Bond, Crypto, Stock Option, or Other |

### Editing or deleting a security

Tap any security to edit its details. Deleting a security removes its price history but does not affect any transactions that reference it.

---

## Pricing

### Automatic pricing

Tally Up retrieves prices from market data providers in the background. Prices update automatically — no action is required.

If automatic pricing encounters an error (for example, an unrecognised symbol or a provider outage), the date and reason are shown on the security's detail screen.

### Manual pricing

You can enter prices manually for any security. Open the security → tap **Prices** → tap **Add** to enter a price for a specific date.

Manual prices are useful for:

- Securities traded on exchanges not covered by automatic providers
- Historical prices you want to lock in from a specific source
- Private securities with no market price feed

---

## How securities are linked to transactions

When you record a buy or sell transaction on an investment asset, you can link it to a security. Tally Up uses those links — along with the security's price history — to calculate your portfolio value and performance over time.

Securities can also be created automatically during QIF import if the file includes investment transactions with symbol information.

---

## Sync and storage

Automatically fetched prices are stored on your device only — they are not synced via iCloud. Each of your devices fetches price history independently. This keeps your iCloud sync small, since price history across many securities can be large.

Manual prices you enter are synced via iCloud along with the rest of your plan data, so they remain available on all your devices without needing to be re-entered.

---

## Tips

- Use the exact ticker symbol as it appears on the exchange where the security trades — this is what the automatic pricing provider uses to look up prices.
- If you hold the same security in multiple assets (for example, the same ETF in two ISAs), you only need to add it once. The same security record is shared across all assets.
