# Export & Backup

TallyUp gives you full control over your data. You can export your plan at any time as a file you can keep, share, or restore from.

---

## Exporting a plan

Open the **Plans** screen, find the plan you want to export, and tap the **export icon** (a square with an upward arrow). A prompt asks which data to include.

### Export scopes

**Full Plan**
Everything in your plan: people, assets, transactions, splits, categories, category rules, budgets, funding rules, securities, and any manually-entered security prices. Auto-fetched security prices and FX rates are not included — they are re-fetched automatically after an import.

Use this for a complete backup or to move your plan to another device.

**Setup Data Only**
The plan structure — people, assets, budgets, categories, rules, and settings — but not transactions or market data.

Use this to create a template you can reuse for a new scenario, or to share your setup with someone else.

**Market Data Only**
Securities, price history, and FX rates only. No plan structure or transactions.

Use this to transfer market data to another plan.

---

## File format

Exports are saved as **JSON files**. The file is human-readable and version-stamped, so TallyUp can handle files created by older versions of the app.

Give the file a recognisable name and save it somewhere safe — your Files app, iCloud Drive, or an external location.

---

## Importing a plan

Open the **Plans** screen and tap the **import icon** (a square with a downward arrow). Select a previously exported JSON file.

If a plan with the same name already exists, TallyUp will ask whether to replace it or cancel.

After a full plan import, TallyUp re-fetches auto-priced security prices and FX rates in the background.

---

## iCloud sync

As well as manual exports, TallyUp syncs your plan data across your devices via iCloud automatically. If you sign in to TallyUp on a new device with the same Apple ID, your plans will be available without needing to restore from an export file.

Manual exports are for your own peace of mind and for moving data to locations outside iCloud.

---

## Tips

- Export a full plan backup before making significant changes — deleting assets, reorganising categories, or running a large import.
- Keep at least one recent full export somewhere outside the device (for example, in an email to yourself or on a computer). iCloud sync is not a substitute for a deliberate backup.
- If you are moving to a new Apple ID, export your plans manually first — iCloud sync does not transfer across accounts.
