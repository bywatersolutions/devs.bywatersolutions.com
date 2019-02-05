---
title: Removal of shelving location at checkin
raised: 1500
supporters: 3
date: 'Thu Dec 01 2016 01:26:05 GMT-0500 (Eastern Standard Time)'
goal: 1500
short_description: Shelving locations need to ability to be removed upon checkin.
bug: 0
module: Circulation
published: true
---

Shelving locations need to ability to be removed upon checkin.

To accomplish this, we will use the same pattern as bug 11629 which updates the not for loan status on checkin.

# Work to be done
* Add new syspref UpdateLocationOnCheckin, the syspref will store a list of location pairs ( from/to where either can also be empty i.e. no location )
* Modify AddReturn so that the location is updated whenever the item is checked in
