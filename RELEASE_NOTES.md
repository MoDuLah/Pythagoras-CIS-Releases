## v3.3.7 - Merit-aware sponsored training

- Adds a sponsored/free risk policy inside Notification rules: reuse the enabled fixed thresholds or evaluate each employee dynamically from Merits + Addiction + Inactivity.
- Treats a positive merit balance as eligible, blocks zero or negative balances, and fails closed when the effectiveness breakdown needed for the decision is missing.
- Explains eligible, risk-blocked, and three-day-held candidates while preserving a ninth sponsored slot after eight paid trains whenever someone qualifies.
- Keeps paid ledger slots independent from sponsored-risk filtering, uses each order's requested position, verifies or restores that position before training, and never bypasses the three-day new-hire hold.
- Uses the upcoming daily training supply for pre-reset planning instead of the already-spent live balance.
