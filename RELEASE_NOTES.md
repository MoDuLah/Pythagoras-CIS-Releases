## v3.1.9 - Reliable launcher, training, and daily records

- Repairs the minimized footer launcher when Torn redraws its button or removes the emblem. Empty wrappers collapse, surviving wrappers are reused, and the floating launcher returns whenever the footer control is unhealthy.
- Auto mode treats enabled addiction and inactivity thresholds as hard exclusions for sponsored/free trains. Paid FIFO orders remain eligible, and sponsored/free capacity rotates across every eligible member before assigning an extra train to the lowest-stat member.
- Advertising-budget observations now use the 18:10 TCT company-day boundary. Exact budget changes override stale daily snapshots so Balance does not apply a post-closing budget to the day that already closed.
- Recovers one isolated closing wage when complete wage logs contain an exact post-closing departure and no later roster snapshot can exist. Incomplete or inferred departures remain unknown.
- Adds adaptive contrasting outlines to progress-bar and graph text across light, dark, built-in, and custom themes.
- Adds focused regression coverage for launcher recovery, Auto threshold exclusions, paid-order immunity, advertising-budget dates, exact departures, and text contrast.
