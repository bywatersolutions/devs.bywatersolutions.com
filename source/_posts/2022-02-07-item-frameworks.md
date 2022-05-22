---
bug: 24606
raised: 8000
goal: 8000
supporters: 2
date: '2022-02-07 07:51 -0600'
published: true
title: Item Frameworks
module: Funded
short_description: Item Frameworks
RT: 63095
RT2: 95849
Sponsor1: Monterey County
Sponsor2: Aspencat (Clic)
sponsor: Monterey County
---
## Ability to create and use 'frameworks' when adding item records

This development would create a way to make different templates for item records, (ex: Adult Fiction, Adult Non Fiction, etc) that libraries would be able to apply when creating an item record.  

For example: Cataloger is adding Adult Fiction items, they would create (or select the existing framework) from the item add screen.  The item fields configured (location, itype, callnumber prefix, etc) in the framework would autopopulate and reduce the need for repetitive data entry.  

https://bugs.koha-community.org/bugzilla3/show_bug.cgi?id=24606

Worked required to complete this feature:
-Add an API route. 
-Three buttons:
  1. Save this template
  2. Use one of my templates
  3. Use my template for my entire session (as long as I am logged in)
-The templates are stored in the db by user
