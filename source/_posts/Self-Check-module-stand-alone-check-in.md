---
title: Self-Check module stand alone check-in
raised: 2000
supporters: 1
date: 'Wed Nov 30 2016 08:58:23 GMT-0600 (Central Standard Time)'
goal: 2000
short_description: >-
  Add a check-in button to the main self-check screen to allow check-in of
  multiple items.
tags: koha sco self-check selfcheck
bug: 15492
module: Funded
published: true
originalmodule: Self-check
---

This would work very similarly to the current check-in module on the staff client, except that patron information won’t be displayed. Once all books are scanned in for check-in, a “Finish” button can be clicked in order to return to the main shelf-checkout screen to login with ID and checkout books as normal.

# Work to be done
1. Create new sco-checkin.pl script
2. Create new sco-checkin.tt template
3. Make sco-checkin.pl accept barcodes and mark items as returned
4. If item cannot be returned ( i.e. AddReturn returns 0 ) request that the item be taken to a library for returning.
