---
bug: 0
raised: 0
goal: 15000
supporters: 0
date: '2019-07-31 09:49 -0600'
published: true
title: Select Multiple Funds for a Single Order
module: Acquisitions
short_description: Multiple Funds per Order
tags: 'acquisitions, funds'
---
Currently in Acquisitions orders placed are tied to a single fund.  Sometimes, libraries need to split the cost across two or more funds.  For example:

- The Sociology department and Psychology department pool their respective funds to to split the cost of a subscription needed for both deparments.

- Or maybe it's the end of the fiscal year and there is $20.00 left in YA fund and $15.00 left in the Adult materials fund.  Acquisitions staff would like to cobble those two funds together to purchase an item at $35.00


**We are proposing the following development to allow users to select multiple funds for a single order:**
1. Create a new database table to contain an order and associated fund/amount data.
2. The acquisitions Order table would show either a single fund or the word "multi". 
3. If multi is selected the user then selects all the funds desired.
4. The new orderfunds table would have as many lines as needed to make up the price of the item ordered (funds selected above).  fund A at $70 and fund B at 30$ for a total price of $100.  Each fund could have a unique dollar amount taken from it.
