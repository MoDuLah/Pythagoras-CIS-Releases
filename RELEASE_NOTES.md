## v3.4.0 - Background sync and visible verification

- Replaces chained page-timer yields during startup history processing with message tasks and uses dedicated-worker timers for sync request pacing, with a fallback where workers are unavailable.
- Shows sync progress immediately, including current Torn account verification and company workspace loading, while retaining the single-sync guard.
- Makes Up to date a clickable button that checks GreasyFork again with a fresh request.
- Bounds browser-fetch requests through response-body completion so an unresponsive request cannot hold the sync queue indefinitely.
