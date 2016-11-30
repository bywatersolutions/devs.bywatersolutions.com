---
title: Make Longoverdue/Lost items not renewable
raised: 0
supporters: 1
date: 2016-11-30 14:53:02
goal: 1500
short_description: Prevent renewals based on item table values.
tags: koha renew renewal renewals
bug: 15494
---

This development would allow a library to prevent the renewal of items based on the values of any field in the items table including but not limited to any itemlost value.

# Work to be done
1. Add new system preference ItemsDeniedRenewal patterned after OpacHiddenItems
2. Modify C4::Circulation::CanBookBeRenewed to check this system preference
