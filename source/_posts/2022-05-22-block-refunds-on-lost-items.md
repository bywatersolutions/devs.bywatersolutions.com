---
bug: 0
raised: 0
goal: 5000
supporters: 0
date: '2022-05-22 14:11 -0600'
published: true
title: Block refunds on Lost items
module: Circulation
short_description: Lost Item Refunds
rt: 82715
---
Often lost items should not generate refunds to patrons even when that lost item is found and returned to the library.  This development will create a system preference that allows the library to specify the age of a paid lost item that cannot be refunded.  

"User Story": Patron lost a book and is charged the lost fee at 30 days overdue.  The patron pays the lost fee at 50 days past the lost date in order to continue to be able to circulate items at the library.  Patron eventually finds the book at home and brings it back to the library 93 days after it was marked lost.  The library has the system preference set to 90 days (allowing refunds up to 90 days for lost items). When the item is checked in, NO refund is issued to the patron and the item is checked in and marked as 'not lost'.


This work is estimated at $5000.  The work to be done:

1 - Add a syspref 'Dont refund items paid off more than X days ago'
2 - Add code to determine age of most recent lost refund
3 - Add a check at Circulation to see if a refund should be created according to pref and check in
