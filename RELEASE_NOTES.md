## v3.4.3 - Pre-flight training positions and grouped queues

- Groups paid trains by their exact ledger order in the calendar before the queue is locked, so the visible order matches the succession used for execution.
- Checks every paid recipient's first required position when the director locks the queue, before train 1, and keeps the Train `+` disabled until all live Torn positions are confirmed.
- Uses each ledger order's requested position for pre-flight corrections, records temporary changes for one queue-end restoration pass, and retains the immediate safety recheck before every individual train.
- Moves the yellow position safety prompt into an independent floating window instead of expanding or being constrained by the first calendar column.
