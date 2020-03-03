---
bug: 0
raised: 0
goal: 2500
supporters: 0
date: '2020-03-03 10:29 -0700'
published: true
title: 'Increase statistics data for Local use report '
module: Statistics
short_description: Increase statistics data for Local use reporting
RT: 36509
---
**Development to refine 'local use' entries in Statistics.**

This development will add information to checkins related to holds and transfers in the statistics table when using RecordLocalUseOnReturn.  We propose adding 'hold' and 'transfer' to the statistics table in the statistics.proccode field when a checkin prompts the user that a hold was found or a transfer requested.  

_**Caveats:**_
- The assumption made is that the user will proceed with 'trapping' the hold and completing the transfer of the item.
- This development will not prevent extra local uses from being recorded when an item is checked in more than once.  (double check-ins) 
- Also, using Koha's statistical patron will also resolve this issue without a development for libraries wishing to use that workflow option.


The cost of this development is $2500