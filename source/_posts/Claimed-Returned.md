---
title: Claimed Returned
raised: 8000
supporters: 3
date: 2016-11-30 12:40:18
goal: 8000
short_description: This feature will add the ability for library staff to mark things as claimed returned when the patron states that he/she returned an item that is still showing as checked out.
tags: koha claims returned
bug: 14697
module: Circulation
---

* mark an item claimed returned via circulation
    * a check box on list of checkouts on patron record and check out screen
* gray out/disable ‘claimed return’ status from lost menu on item detail page – only perform this action from patron/circulation
* sys pref to ask ‘charge’, ‘don’t charge’, or ‘ask for confirmation’ when marking an item claimed returned
* sys pref to say what ‘lost’ status is to be used for ‘claimed returns’ If no value ‘claims returned’ is off
* sys pref to offer an option to block a patron, or alert staff somehow, after a set number of claimed returns
* remove item from patron’s current list of check outs
    * This should stop fines from accruing
* keep basic information about the item on patron’s record so you can track how many times they’ve said ‘i returned that’
    * This should be a tab on the list of checkouts section on patron detail and checkout page all titles they have claimed in the past (even if they have since been returned or deleted)
    * ex. [title 1] / checked out {date} / claimed {date} / not returned / notes
      [title 2] / checked out {date} / claimed {date} / found {date} / notes
* show as missing in the opac and claimed returned in the staff client
* be able to mark item as ‘found’ from claimed tab if item happens to be found
    * Offer options of “returned by patron” or “found in library” in a pull down to the side of every item that has been claimed.
* claimed items should be easily distinguishable on staff side (compared to lost items)
* on patron check out under ‘Attention’ so alert ‘Patron has claimed returns’ that links to the ‘Claimed’ tab below
* next to each claimed item have a ‘notes’ field for anything

Learn more and follow the discussion <a href="http://bugs.koha-community.org/bugzilla3/show_bug.cgi?id=14697">here</a>.
