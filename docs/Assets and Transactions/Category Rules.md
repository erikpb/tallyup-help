# Category Rules

Category Rules tell TallyUp how to automatically assign a category to a transaction when it arrives. Once set up, new transactions are categorised without any manual effort.

---

## How rules work

When a transaction is imported or synced, TallyUp looks at the merchant or payee name and tries to match it against your rules. If a match is found, the category from that rule is applied automatically.

Rules are matched in priority order. The first rule that matches wins.

---

## Viewing and managing rules

Go to **Settings → Category Rules** to see all your rules.

The list shows each rule's:

- **Pattern** — the merchant or text being matched
- **Match count** — how many transactions this rule has categorised
- **Confidence** — how reliably the rule matches (higher is more specific)
- **Priority** — the order in which rules are evaluated

You can sort the list by Match Count, Priority, Confidence, or Name.

---

## Creating a rule manually

Tap **Add** to create a rule. You can specify:

- **Pattern** — the text to match against the transaction description or payee. Supports plain text, wildcards (`*`), and regular expressions.
- **Category** — the category to assign when the rule matches
- **Amount constraints** — optionally restrict the rule to transactions of an exact amount, or within a range
- **Priority** — lower numbers are evaluated first

Rules based on recognised merchants are the most reliable. When TallyUp identifies a known merchant in the transaction description, it uses that merchant as the match key — making the rule stable even if the raw bank description varies slightly between transactions.

---

## Inferring rules from history

Rather than creating rules one by one, TallyUp can learn from your existing categorised transactions and generate rules automatically.

Tap the **wand icon** in the Category Rules screen and choose how many months of history to scan (the default is 24 months). TallyUp reviews your categorised transactions and creates rules for patterns it finds consistently.

The summary shows how many rules were created, reused, or skipped.

This is a good starting point when you first set up TallyUp, or after importing a large batch of transactions.

---

## Multiple Categories

If two rules match the same merchant but assign different categories, TallyUp marks the transaction as **Multiple Categories** rather than guessing. You can then open the transaction and choose the correct category.

This prevents silent miscategorisation when a merchant (such as Amazon) is used for several different purposes.

---

## Tips

- Run inference from history before creating rules manually — it often covers the most common merchants immediately.
- Use amount constraints to distinguish regular monthly bills from one-off purchases at the same merchant.
- Delete rules that consistently produce wrong results — TallyUp will leave those transactions uncategorised for you to handle manually.
