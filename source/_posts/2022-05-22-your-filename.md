---
bug: 0
raised: 0
goal: 4500
supporters: 0
date: '2022-05-22 14:25 -0600'
published: true
title: SIP self check authentication method
module: Self Check
short_description: 'SIP functionality '
rt: 85736
---

Add the ability for SIP selfcheckin devices to authenticate users based on a repeatable patron attribute. With this development a patron could have multiple of a single attribute (ie. child card) and that attribute would be designated as a method of identifying the parent level account to perform the checkout.

This attribute would also be required to be 'unique'.  That is to say if you have two parents, each with their own individual account, they could not both have the child cards assigned to the accounts.  Only one parent can have the child attribute for child cardnumbers.

Example:
Parent A has 3 children (1,2,3).  Each child has their own account and their own library card and cardnumber.  However the library would prefer that all items be checked out the parent.  Parent A would then have 3 attributes for 'CHILD CARD' each attribute with a child's cardnumber associated.  When the child attempts to login, Koha authenticates that cardnumber as a CHILD CARD belonging to the parent and checks out the item on the parent record.

$4500, sip functionality only not for Koha's Self check module
1 - Add sip config option 'additional_id_attribute'  - only specifiy unique atrtributes
2 - Adjust SIP code to find patron by this id
