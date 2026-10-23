## v3.3.9 - Accurate daily train availability

- Makes Daily sync refresh the live company profile, employees, and stock every time instead of trusting a 24-hour freshness flag for values that reset each company day.
- Rebuilds today's planner and active training queue from Torn's refreshed train count, so a cached zero cannot leave the current day blank after 18:10 TCT.
- Keeps Business Profile, Available train slots, and the consolidated Pythagoras API snapshot on the same current availability.
