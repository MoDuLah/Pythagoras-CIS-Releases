## v3.2.3 - Independent training batches

- Allocates exact training actions chronologically and only to orders that already existed when each action occurred.
- Rebuilds synchronized usage for event-backed orders, clearing stale trains that had carried into a later purchase.
- Keeps Racehorce's 10-train and 21-train purchases independent: the first 10 fill only the first batch, while later actions can fill the second batch to a total of 31.
- Preserves manually entered usage on manual orders that have no Torn payment event ID.
