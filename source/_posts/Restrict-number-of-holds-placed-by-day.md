---
title: Restrict number of holds placed by day
raised: 500
supporters: 1
date: 2016-12-01 06:12:23
goal: 4000
short_description: Add the ability to restrict the number of holds placed per day up to the maximum number of holds in circ/hold rules.
tags: koha hold limit restrict limits daily day
bug:
---

# Example
A patron is allowed to place 5 holds (or other variable number set by the library) per day but can not exceed 30 holds (set by circ rules).

# Work to be done
1. Add new database column reservesallowed_daily to the table issuingrules
2. Add new database column “created_on” to the table reserves
3. Modify C4::Reserves::AddReserve to populate “created_on” with the current timestamp
4. Add new column “Holds allowed (daily)” to the circulation and fine rules.
5. Modify “Holds allowed (count)” to “Holds allowed (total)” for clarity
6. Modify CanItemBeReserved to check if max daily holds has been exceeded If so, it must return new error code ‘TooManyReservesToday’
7. Modify all code calling CanItemBeReserved to handle this new error code
8. Add unit tests for new CanItemBeReserved behavior
