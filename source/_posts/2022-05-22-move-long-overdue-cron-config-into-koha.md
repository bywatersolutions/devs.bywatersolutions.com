---
bug: 0
raised: 10000
goal: 10000
supporters: 1
date: '2022-05-22 14:19 -0600'
published: true
title: Move long overdue cron config into Koha
module: Cron
short_description: move long overdue cron config into Koha
rt: 106319
sponsor: Rapid City Public Library
---
This enhancement request will move all the configuration options for the Long Overdue Cron into the staff side of Koha so that libraries can manage these settings on their own instead of needing someone to adjust them at the command line on the server.

The development will create a new configuration page in the Administration area of Koha to allow libraries to set their configurations per branch for the long overdue process.  New API routes will need to be created to allow Koha to get and set the rules.  The rules will be set at the branch level, group level, or system level.

The current cron will still function with the runtime options however it will warn that the switches are to be deprecated and the new interface should be used.

We estimate this at $10,000, work to be done:
1 - Add a new config page to the administration section
2 - Add API routes for getting/setting rules
3 - Utilize datatables API for displaying/editing rules
4 - Allow for defining rules at the system, group, or library level
5 - The cron switches will take precedence if set, but will warn of deprecation
