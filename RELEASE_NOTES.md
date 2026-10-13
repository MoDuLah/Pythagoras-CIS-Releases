## v3.3.0 - Reliable staff-history pagination

- Continues valid Torn hire and wage-history pagination when `/v2/user/log` supplies its same-second continuation `nanostamp` in response metadata instead of embedding it in the next link.
- Keeps strict company/account, endpoint, log-selection, malformed-cursor, and repeated-link safeguards so incomplete history is never marked complete.
- Removes the unnecessary gap between completed Sync all steps and the live Sync console.
- Names the actual Torn log IDs in the console: `6242` hire, `6263` training, `6265` wage change, and `6267` role change.
