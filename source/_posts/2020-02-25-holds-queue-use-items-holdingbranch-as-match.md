---
bug: 0
raised: 0
goal: 6000
supporters: 0
date: '2020-02-25 12:43 -0700'
published: true
title: Holds Queue - Use items holdingbranch as match
module: Holds
short_description: Selecting items for the Holds Queue
RT: 54076
---
Development to make the Holds Queue algorithm match the "Current Location" (holding branch) against the patron's pick-up branch, rather than the "Permanent Location" (homebranch)?  

If the "Current Location" is where the item is presently and the "Permanent Location" is simply the branch where the item was first introduced matching on where the item is may be a better match to get holds to patrons quicker.
