---
title: Limit Item Types by Branch
raised: 1000
supporters: 1
date: 2016-11-30 12:36:29
goal: 3500
short_description: This feature will allow the creation of branch specific item types.
tags: koha itemtype library
bug: 
---

![Screenshot](image.png)

# Work to be done
1. Create new table itemtype_branches similar to authorised_values_branches
2. Add branch selector to itemtypes editor similar to branch limiter for authorised values
3. Create subroutine to return only itemtypes for logged in branch
4. Replace itemtype select in additem.pl with call to aforementioned subroutine
