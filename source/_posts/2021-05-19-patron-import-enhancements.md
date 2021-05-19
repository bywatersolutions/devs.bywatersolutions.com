---
bug: 0
raised: 5000
goal: 10000
supporters: 1
date: '2021-05-19 11:20 -0600'
published: true
title: Patron Import Enhancements
module: Tools
short_description: Patron Imports
rt: 80501
sponsor1: bws for 50%
---
### Patron import enhancement

## Proposed behavior

1. Staff using the patron import tool is presented the usual form, with a new checkbox: Review before commit.
2. Once the file is uploaded, and the checkbox checked, the patron is presented some potential import results, as with biblios: summary, and a link to a new page for staged patron imports
3. The staged patron's page shows a list of patrons, if matched, the diff, potentially rendering the unblessed representation as well.

Caveats:
* This doesn't include any feature to reverse imports once they are done.
* It is designed to use existing APIs.

## Work to be completed

1. Add routes for adding new tasks to the queue
2. Add tables:
    - import_patrons table
    - import_patrons_matches
3. Add a page for displaying staged patron imports
4. Add classes for handling patron imports in the task queue

## Potential Future follow-ups (would require additional funding)

I would love to see a feature added for staged files, that detects unknown columns, and allows mapping them (e.g. some unnamed columns or with unknown names, could be mapped into extended attributes, or even core fields)

## Funding

ByWater Solutions is proposing a 50% subsidy to the core development.  The cost of the entire development is $10,000USD of which ByWater will cover $5,000.  Any monies raised in excess of the quoted amount will be put towards the devlopments covered under 'future followups'.
