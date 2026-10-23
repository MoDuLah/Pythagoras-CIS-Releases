## v3.4.1 - Incremental sync and daily staff retention

- Checks a small authenticated server revision before downloading a saved workspace; a complete matching local cache is reused without discarding unsaved edits.
- Remembers successful uploads and skips unchanged staff, snapshots, events, stock, settings, ledger and workspace payloads. Concurrent server changes invalidate the cached revision safely.
- Preserves report wage-evidence and invalidation metadata across downloads and upload acknowledgements so old dates do not repeatedly appear corrected.
- Keeps one latest staff snapshot per employee and company day; the separate daily Employee Efficiency history is preserved.
- Defers workspace autosaves until sync completes, reuses prepared operating costs, and calculates historical advertising budgets in one pass.
