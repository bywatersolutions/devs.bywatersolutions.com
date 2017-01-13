---
title: Disable the ability to suspend holds related to certain itemtypes
raised: 1500
supporters: 1
date: 2016-11-30 15:00:14
goal: 4500
short_description: Disallow "suspend hold" on certain item types.
tags: koha hold holds suspend
bug:
module: Holds
---

For example: If an item is an “ILL” the ability to suspend the hold should not be an option.

# Work to be done
1. Add new field suspend_hold_allowed to the itemtypes table, default of 1
2. Reveal this field though the itemtypes editor
3. Create a subroutine that will look up the field value for a given itemtype
4. Create a subroutine that accepts a reserve and calls the previous sub to find the value for this reserve ( based on itype/itemtype )
5. Add a test before suspending for each hold suspension request
6. Add a new TT plugin that uses this subroutine to disable suspend buttons in the opac
7. Add ability to suspend individual holds in the staff intranet
8. Add ability to disable suspending of individual holds in the staff intranet

The last two steps give librarians not only more flexibility for suspending holds, but give a visual indicator that a hold is not suspend-able.
