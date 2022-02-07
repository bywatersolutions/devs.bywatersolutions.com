---
bug: 0
raised: 0
goal: 6000
supporters: 0
date: '2022-02-07 08:11 -0600'
published: true
title: Fill Overridden Holds
module: Holds
short_description: Trigger Forced Holds
RT: 83168
---
## Fill Overridden Holds

Koha allows staff to override placing of holds that can not be placed because the circ rules will not allow the hold to be filled.  However, there are times when staff want to place 'unfillable' holds and then have those holds filled.  The following enhancement refines the placing of unfillable holds and then allows Koha to fill the holds.

Step 1:
 - Create a new borrowers permission:  allow_placing_overridden_holds
 - This permission wil only be checked when the system preference AllowHoldPolicyOverride is enabled
 - When the site is updated with this feature, if the syspref is enabled, all borrowers who can place holds for other patrons will receive the new permission initially.

Step 2:
 - Add overridden_hold column to reserves which will indicate if the hold placed was specifically overridden by staff.
 - In filling holds (checkreserves code) Koha will still obey damaged and notfor loan checks
 - Koha will override the Circulation rules checks in last section of checkreserves to force filling overridden holds
