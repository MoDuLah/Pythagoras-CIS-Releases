## v3.3.8 - Reliable training queues

- Reopens the requested-position prompt when Torn returns an employee to the original role between paid trains, without sending the blocked train.
- Defers every temporary planner position restoration until the whole queue is complete, then restores all changed employees in one submitted update.
- Refreshes only the training session, current queue controls, and active row during each training phase instead of rebuilding the full CIS interface.
- Adds Build from today so a saved past or future planner date cannot hide the current day's calendar when the director needs it.
