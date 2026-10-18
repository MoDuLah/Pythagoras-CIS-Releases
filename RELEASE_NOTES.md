## v3.3.2 - Fair bought-train allocation

- Adds a Bought-train allocation dropdown in Training setup with FIFO, equal Split, and every oldest/next-buyer combination for the daily paid cap.
- Splits eight bought trains as four per buyer when two buyers are waiting, treating multiple open orders from the same player as one buyer.
- Leaves any capacity beyond the paid cap in sponsored/free rotation and safely falls through when a buyer cannot use their full daily quota.
