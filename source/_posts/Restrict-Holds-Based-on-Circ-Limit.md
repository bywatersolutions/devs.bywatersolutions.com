---
title: Restrict Holds Based on Circ Limit
raised: 0
supporters: 1
date: 2016-12-01 06:18:08
goal: 2000
short_description: Add a way to restrict holds for patrons who are at or over their circulation limit.
tags: koha circulation debar debarment restriction restrictions
bug:
module: Circulation
---

This development will add a way to restrict holds for patrons who are at or over their circulation limit by:
* Creating a new system preference “IncludeCheckoutsInHoldsAllowedCount” ( or something similar )
* When enabled, Koha will add a patron’s count of current checkouts to the count of current holds to determine if the patron has exceeded the maximum number of holds allowed as defined by the “Holds allowed ( count )” field in the issuing rule for that library/patron/itemtype combination.
