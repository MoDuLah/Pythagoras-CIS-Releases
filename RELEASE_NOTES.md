## v3.2.5 - Faster verified startup and timed sync activity

- Uses Torn's readable numeric `uid` cookie as the early account identity hint, allowing a matching cached workspace to open before Torn's page globals or navigation links render.
- Keeps the live Torn API response authoritative for authentication, company membership, and workspace access; sensitive authentication-token cookies are never read.
- Shows individual elapsed times for completed initialization, Daily sync, Sync all, and nested synchronization steps while retaining the overall duration on the final line.
- Pauses the activity toast's remaining auto-close countdown while the pointer is over it and resumes the same countdown when the pointer leaves.
- Checks the stock-purchase log from the newest saved purchase timestamp instead of rereading older entries during routine checks.
- Removes the automatic restock child-sync log and stops repeating the same restock result in the final Daily sync summary.
