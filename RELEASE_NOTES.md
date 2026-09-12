## v3.1.6 - Accurate daily records and event timing

- Fixes blank wages and profit after Sync all runs after 18:10 TCT. A wage observation from that same calendar day can recover the closing wage once hire/wage logs cover the observation time.
- Reverses logged wage changes at or after closing before calculating that day's payroll. Missing or contradictory evidence remains unknown, and later calendar dates do not backfill earlier wages.
- Assigns employee-efficiency snapshots observed before 18:10 TCT to the previous company day. Stored rows with a reliable observation timestamp are repaired automatically.
- Replaces company-news observation times in Timeline training entries with the exact Torn user/log 6263 timestamps and retains those exact events across cloud reloads.
- Rebuilds and uploads operating costs, staff history, and daily reports after staff-log sync completes, so saved Balance values use the final wage evidence.
- Adds regression coverage for the company-day cutoff, exact training times, after-closing Sync all, exact-cutoff pay changes, zero wages, missing coverage, and upload failures.
