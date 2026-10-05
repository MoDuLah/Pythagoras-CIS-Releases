## v3.1.8 - Automatic company workspace handover

- Verifies the saved Torn account and current company before startup workspace loading and before every company sync.
- Detects company or account changes automatically, preserves the historical cloud workspace, and opens a pristine workspace for the verified company without carrying staff, news, stock, wage, ledger, planner, or company settings across.
- Keeps only portable browser preferences and the remembered API identity during handover, clears unscoped company caches, and explains the switch in the interface.
- Historical workspace shortcuts can only open when the Torn account is currently attached to that company; manual switching can no longer save or merge an old company into the new one.
- Rejects business data if Torn returns another company or identifies another director before any current workspace data is mutated.
- Requires the live backend to verify the current director from Torn's company profile, revoke stale company access, and deny ordinary staff accounts instead of recording them as directors.
- Adds regression coverage for company moves, leaving a company, pristine-state boundaries, strict bootstrap failures, staff rejection, authoritative director verification, and stale-access revocation.
