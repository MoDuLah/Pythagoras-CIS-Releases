## v3.1.10 - Training ledger reconciliation

- Recognizes Torn company-news wording such as `Apprentice Technician Racehorce received 10 trains by the director` and records the recipient, position, and exact train count.
- Import from log now reclassifies stored training history and immediately reconciles given trains into matching ledger orders.
- Existing payment rows can be safely imported again: the duplicate payment remains skipped while previously missed training history repairs the order.
- Adds focused regression coverage for both newly imported and already-existing orders.
