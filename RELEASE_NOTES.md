## v3.1.3 - Faster startup, authoritative sync, and role-aware wages

- Timeline and report-section settings now persist correctly. Timeline loading can be disabled completely, and disabled timelines are omitted from the server bootstrap for faster startup.
- Routine refreshes are consolidated into one Sync all action covering business details, the authoritative employee roster, stock and services, latest news and reports, exact training actions, wage and role history, advertising changes, and restocking costs.
- Fresh Torn employee data is authoritative: missing current staff move to Past Staff, rehires return to Current Staff, and local contracts/history are retained.
- Suggested wages use only each position's primary and secondary working stats. Mechanic Shop Technician/Apprentice/Cleaner use MAN + END; Manager/Receptionist/Trainer use INT + END.
- Every wage-model value and role requirement accepts decimal input and retains decimal precision until the final suggested wage is rounded.
- Retains the recruitment-mail hand-off and all behavior present in the previous PE userscript; no old-only methods were removed during reconciliation.
