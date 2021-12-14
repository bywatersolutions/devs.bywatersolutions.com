---
bug: 0
raised: 0
goal: 10000
supporters: 0
date: '2021-12-14 10:28 -0600'
published: true
title: Auto Update Guarantor and Guarantees
RT: 51030
module: Patrons
short_description: Auto Update Guarantors and Guarantees
---
## Improve the process for updating guarantees or guarantors

When editing a patron's record show 'update linked accounts' checkbox.

When this box is checked, and the record is saved, show the user a list of all other linked accounts and choose which accounts to update with information from the record you just edited.

The fields listed in PrefillGuaranteeField system preference will be used to indicate the fields that will be updated for linked (and selected) accounts.

Additionally add 'Update linked accounts' button on patron menu that leads to same screen as above.  In this case and the linked accounts will be displayed and allow user to select accounts to update based on the data in the originating record.

**Use Case:** Guarantor updates mailing address with circ staff in the library.  The circ rep updates the record and checks the box to update linked accounts.  They can update all accounts, or select only certain guarantee accounts to update with guarantor mailing address.  

**Use Case:** Patron submits updates to their account through opac.  This change is reviewed and accepted by library staff.  Once the update is accepted, staff can then click the button to Update linked accounts.  They will be presented with the linked accounts and then select only the accounts they wish to update.
