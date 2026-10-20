## v3.3.4 - Reliable PDA reports and Jobs loading

- Stops unchanged historical daily reports being re-uploaded when Torn's event time and the reconstructed report timestamp differ, while keeping genuine corrections uploadable.
- Labels the Daily sync comparison as stored report history so its totals are not mistaken for reports created today.
- Loads CIS on Torn PDA's Jobs route and avoids the smart-apostrophe normalization that caused `Unexpected identifier 's'` during script parsing.
- Moves the large disposable startup cache to Torn PDA's native asynchronous storage, verifies legacy-cache migration before removing localStorage data, and retries quota-blocked replacements safely.
- Preserves the newest daily report dates through the PDA cache round-trip and continues in memory if the device cannot persist the refreshed cache.
