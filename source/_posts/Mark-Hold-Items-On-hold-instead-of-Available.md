---
title: Mark Hold Items 'On hold' instead of 'Available'
raised: 1500
supporters: 1
date: 2016-11-30 11:43:31
goal: 2500
short_description: Make the status of items targeted for holds marked as 'On hold' instead of 'Available'
tags: koha hold status
bug: 15505
---

![Screenshot](image.png)

# Work to be done
1. Modify C4::XSLT::buildKohaItemsNamespace to check for proposed holds for each item
2. Modify XSLT if needed
3. Modify item-status.inc to do the same check
