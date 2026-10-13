## v3.3.0 - Reliable staff-history pagination

- Follows Torn's validated hire and wage-history continuation link even when the service uses an opaque cursor instead of exposing the expected timestamp fields.
- Keeps strict company/account, endpoint, log-selection, repeated-page, repeated-link, and maximum-page safeguards so incomplete history is never marked complete.
- Places the Sync console label above its scrolling output and removes the remaining blank strip below completed Sync all steps.
- Uses clear log names in the console: Training, Wage change, Role change, and Hire.
