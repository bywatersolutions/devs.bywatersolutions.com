---
title: Show item count on Z39.50 results
raised: 500
supporters: 1
date: 2016-11-30 11:59:38
goal: 2500
short_description: Show holding counts when searching Z39.50 targets
tags: koha holds z39.50
bug: 15499
module: Cataloging
---

![Screenshot](image.png)

# Work to be done
1. In the z39.50 search targets editor, add a field for “item tag”. In the case of searching a Koha target, it would be 952. We’ll have to find out what the item tag is for other ILS’s. It seems 852 and 949 are common.
2. Modify the code to count the number of instances of the given tag for the given server
3. Show this number as the “holdings” for the given search result.
