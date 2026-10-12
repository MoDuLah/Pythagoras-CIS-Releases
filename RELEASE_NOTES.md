## v3.2.4 - Faster cached startup and reliable training orders

- Opens the verified saved company workspace immediately from asynchronous userscript storage while the live Torn identity check continues.
- Keeps a freshly loaded cloud workspace authoritative instead of reapplying an older browser cache that could resurrect deleted orders.
- Uploads only new or changed daily reports after the server workspace is known, avoiding repeated uploads of unchanged report history.
- Restores the lightweight Daily sync action for routine company updates while retaining Sync all as the full history rebuild.
- Remembers deletion of imported refunded orders so the same Torn payment event is not recreated by a later synchronization.
- Preserves empty pending-order replacements, enriches older completed orders with current staff merits, and explains discount savings, credit, and the shortfall to the next full train.
- Gives the Add order staff selector more room, tightens the Paid and Done controls, and confines activity scrolling to the console for startup and synchronization.
