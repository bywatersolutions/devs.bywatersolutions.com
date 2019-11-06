---
title: Balancing high demand holds
raised: 2500
supporters: 1
date: 'Wed Nov 30 2016 23:30:47 GMT-0700 (Mountain Standard Time)'
goal: 2500
short_description: >-
  Add options to the decreaseLoanHighHolds preferences so that users have the
  ability to choose A) based on the number of holds, as Koha currently does, or
  have the ability to B) set a number of holds past the number of holdable items
  in that record
bug: 0
module: Funded
published: true
originalmodule: Holds
---

This development will add an option to the decreaseLoanHighHolds preferences so that users have the ability to choose A) based on the number of holds, as Koha currently does, or have the ability to B) set a number of holds past the number of holdable items in that record.

Work to be done:

1. Add new system preferences
    * decreaseLoanHighHoldsOffset
    * decreaseLoanHighHoldsIgnoreDamaged
    * decreaseLoanHighHoldsIgnoreLost
    * decreaseLoanHighHoldsIgnoreWithdrawn
    * decreaseLoanHighHoldsIgnoreNotForLoan
    * Implement logic for new system preferences
2. Add unit tests.

We can use the multi-select enhancement for system preferences from bug 9043 to avoid having 4 prefs.
