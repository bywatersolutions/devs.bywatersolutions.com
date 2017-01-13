---
title: Removal of shelving location at checkin
raised: 1500
supporters: 2
date: 2016-12-01 06:26:05
goal: 1500
short_description: Shelving locations need to ability to be removed upon checkin.
tags:
bug:
module: Circulation
---

Shelving locations need to ability to be removed upon checkin.

To accomplish this, we will use the same pattern as bug 11629 which updates the not for loan status on checkin.

# Work to be done
* Add new syspref UpdateLocationOnCheckin, the syspref will store a list of location pairs ( from/to where either can also be empty i.e. no location )
* Modify AddReturn so that the location is updated whenever the item is checked in
