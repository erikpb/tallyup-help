# Categories

Categories describe what your transactions mean. They let you group spending and income into named buckets — Groceries, Salary, Utilities — so Tally Up can show you patterns and measure your budget performance.

---

## How categories work

Categories are **global** — they are shared across all your plans, not tied to a specific plan. Any category you create is available everywhere in the app.

Categories are **hierarchical**. You can create parent categories with child categories underneath them. For example:

```
Living Costs
  ├── Groceries
  ├── Utilities
  └── Transport
```

A category at any level can be applied to a transaction. Parent and child categories are independent — you can budget at whichever level makes sense for you.

Every category has a **type**: either Income or Expense. The type determines how Tally Up treats the category in budget reporting.

---

## Managing categories

Go to **Settings → Categories** to view, create, edit, and delete categories.

### Creating a category

Tap **Add** and fill in:

- **Name** — the display name (e.g. `Groceries`)
- **Type** — Income or Expense
- **Parent** — optional; choose a parent to nest this category under another

### Editing a category

Tap any category to edit its name, type, or parent. Changes apply immediately across all transactions that use it.

### Deleting a category

Swipe to delete. Transactions that used the deleted category become uncategorised.

---

## Automatic categories

When you [import transactions](Transactions.md#importing-transactions), Tally Up reads the category labels in the file and creates matching categories automatically. This saves manual setup if you are migrating from another finance app.

Tally Up's auto-categorisation engine also assigns categories to new transactions based on your Category Rules. See [Category Rules](Category%20Rules.md) for details.

---

## Tips

- Keep your top-level categories broad and use children for detail. Deep trees are harder to maintain.
- The type (Income vs Expense) matters for budgeting — make sure it matches how you use the category.
- Categories created during QIF import default to Expense if the type cannot be inferred from the file.
