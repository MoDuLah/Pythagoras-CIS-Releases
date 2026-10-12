## v3.2.6 - Explicit training instructions

- Honors explicit train counts in automatic payment comments across accepted singular and plural trigger variants, so `!train 10` remains 10 even when the discounted payment alone would estimate 9.
- Repairs an existing event-backed order on the next history sync when its prior payment-only estimate disagrees with the explicit count.
- Retains and displays sender comments plus sortable Primary and Secondary stat columns.
- Parses labelled stats and shorthand such as `!train 10 Int & End`; position requests such as `!train 10 Trainer` are stored and derive the role's two working stats when known.
- Lets manual Add order entries store the same comment, stat, and requested-position details.
- Persists the new instruction fields through the company cloud workspace and includes them in receipts and exported reports.
