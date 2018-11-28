---
title: Limit Item Types by Branch
raised: 3500
supporters: 3
date: 'Wed Nov 30 2016 07:36:29 GMT-0500 (EST)'
goal: 3500
short_description: This feature will allow the creation of branch specific item types.
tags: koha itemtype library
bug: 0
published: true
module: Cataloging
---
![Limit-Item-Types-by-Branch.png]({{site.baseurl}}/source/images/Limit-Item-Types-by-Branch.png)

# Work to be done
1. Create new table itemtype_branches similar to authorised_values_branches
2. Add branch selector to itemtypes editor similar to branch limiter for authorised values
3. Create subroutine to return only itemtypes for logged in branch
4. Replace itemtype select in additem.pl with call to aforementioned subroutine
