## v3.1.4 - Historical Balance wages

- Current employee wages are no longer copied into older Balance dates. Wage totals require dated staff wage-change logs or API observations, and explicitly recorded zero wages stay zero.
- Wage-change logs preserve exact timestamps and use the existing 18:10 TCT company-day boundary, so late-night changes apply to the next closing date. Re-sync upgrades legacy date-only entries; ambiguous change dates stay unknown until their timing is recovered.
- Ignores unverified wage totals backfilled by older versions while retaining advertising history. Newly reconstructed totals carry evidence metadata, and dated logs can correct previously saved totals.
- Unknown historical wages and their profit remain blank in Balance and exported reports. Daily and weekly graphs leave gaps instead of plotting unknown costs as zero; company goals disclose missing wage coverage.
- Loading older individual staff logs no longer overwrites current pay. Fresh staff-card history takes precedence over stale profile copies.
- Use Sync all and, where necessary, older staff-log pages to recover wage history. Rebuild balance refreshes the displayed calculations; missing historical evidence is not replaced with suggested pay.
