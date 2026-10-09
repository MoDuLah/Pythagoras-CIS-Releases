## v3.2.0 - Organized training-order history

- Splits Training Orders into `Orders`, `Add order`, and `Done orders`, keeping running work separate from manual entry and completed history.
- Fetches every available payment-log `4810` and exact training-action `6263` page by following Torn's validated pagination cursor.
- Recognizes the bounded historical `Traine` and `Tains` message variants while leaving no-message transfers for safe manual attribution.
- Editing, completing, or deleting an order updates only the affected table rows instead of redrawing the whole page.
- Adds regression coverage for tab separation, full-history pagination, historical trigger variants, and row-only deletion.
