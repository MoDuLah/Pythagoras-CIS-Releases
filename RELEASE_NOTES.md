## v3.3.6 - Stable report identity and lighter styling

- Preserves Torn's source event ID from company news through daily-report storage and comparison, with a one-time backfill for legacy date-only rows.
- Lets explicit wage-history invalidations replace stale server values so Daily sync converges instead of repeatedly uploading the same corrected reports.
- Loads the versioned CIS stylesheet from GitHub Pages with a pinned integrity hash and userscript, TornPDA, browser-fetch, and stylesheet-link fallbacks.
- Limits automatic userscript execution to Torn company pages instead of also matching the Jobs and Messages routes.
