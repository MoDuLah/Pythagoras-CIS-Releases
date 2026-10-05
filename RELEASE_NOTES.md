## v3.1.7 - More reliable train payments and closing wages

- Training Ledger payment imports accept `!train` or `!trains` at the start of the money-transfer message when extra instructions follow.
- Message text also tolerates `train` or `trains` without the exclamation mark, while exact trigger fields remain strict and unrelated words such as `training` or `restrains` are rejected.
- Balance can recover one isolated missing closing-wage day when the immediately adjacent verified company days have matching wage evidence. Wider or contradictory gaps remain unknown.
- Adds regression coverage for supported train-message forms, false positives, exact trigger fields, and the single-day wage recovery boundary.
