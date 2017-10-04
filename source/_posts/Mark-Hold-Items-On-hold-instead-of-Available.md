---
title: Mark Hold Items 'On hold' instead of 'Available'
raised: 2500
supporters: 1
date: 'Wed Nov 30 2016 06:43:31 GMT-0500 (EST)'
goal: 2500
short_description: >-
  Make the status of items targeted for holds marked as 'On hold' instead of
  'Available'
tags: koha hold status
bug: 15505
published: true
module: Holds
---

![Mark-Hold-Items-On-hold-instead-of-Available.png]({{site.baseurl}}/source/images/Mark-Hold-Items-On-hold-instead-of-Available.png)

# Work to be done
1. Modify C4::XSLT::buildKohaItemsNamespace to check for proposed holds for each item
2. Modify XSLT if needed
3. Modify item-status.inc to do the same check
