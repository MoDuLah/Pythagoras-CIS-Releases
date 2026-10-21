## v3.3.5 - Complete daily employee history

- Makes Daily sync fetch the current employee roster every time, even while the employee cache is still marked fresh, so each completed Torn day receives an efficiency snapshot.
- Preserves the newly captured employee-efficiency rows through Daily sync's consolidated API upload instead of replacing them with an empty staff-history payload.
- Reports the captured employee-efficiency date in the completed Daily sync message and reuses the snapshot already collected by a stale full-business refresh without making a duplicate Torn request.
