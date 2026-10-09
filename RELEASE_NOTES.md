## v3.2.1 - Event-backed training orders

- Uses Torn's top-level payment event ID as the hidden identity for imported training orders and persists it through cloud reloads.
- Keeps the original, lowest-numbered order when a prior sync created duplicate rows, while preserving completion and train-usage state.
- Retains genuinely separate same-day payments when Torn supplies distinct event IDs.
- Marks Add order entries as manual internally so event-ID cleanup never removes them.
- Keeps event IDs and order origins out of the Training Orders and completed-history user interface.
