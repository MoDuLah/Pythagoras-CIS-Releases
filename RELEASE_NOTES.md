## v3.1.5 - Wage history from joining

- Staff cards show a Joined — salary $0 starting entry followed by every recorded salary adjustment with its timestamp. Rehires retain their separate joining records and restart from zero for the new employment.
- Sync all now retrieves all available hire/wage log pages separately from the latest training/role page. Subsequent syncs retrieve new changes with an overlapping timestamp, preserving and deduplicating the full saved history, including events for staff loaded later.
- Balance uses the joining-date zero baseline once available log coverage is established. Recorded wage changes then apply at their dated company-day boundary. Missing, inconsistent, or inaccessible history remains a gap rather than being silently assigned zero or current pay.
- Pagination is restricted to the expected Torn hire/wage endpoint and must advance to older records. Malformed replies, failed requests, and company/account switches do not replace stored history or mark it complete.
- Rebuilds operating costs after the hire/wage import. Revalidates previously reconstructed totals against the joining-aware model without changing current employee pay.
- Run Sync all after updating. Initial backfill can take longer; the sync console shows page progress. Only logs available to the syncing account can be retrieved, so changes made by another director may remain unavailable.
