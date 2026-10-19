## v3.3.3 - Safer training ledger corrections

- Corrects Manager purchase instructions to use END as the primary stat and INT as the secondary stat, while configured role requirements use the stronger stat first.
- Adds row-level Edit, Save, and Cancel controls for Primary, Secondary, Comment, and Requested Position without changing payments, train totals, usage, or status.
- Keeps manually corrected instructions authoritative during later order-history synchronization and rejects identical primary and secondary selections.
- Removes the direct `Train N` ledger action so training remains governed by the daily planner, including its 20-train capacity and three-day new-hire hold for paid orders.
- Refreshes training-order purchase history during Daily sync and uploads reconciled ledger values through the normal training-order save path.
