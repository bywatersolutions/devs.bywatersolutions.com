---
bug: 0
raised: 0
goal: 3000
supporters: 0
date: '2017-11-02 13:56 -0400'
published: true
title: Match on multiple records
short_description: Match on multiple records
Module: Tools
---
This development would allow the system to alert the user about multiple matches when importing records. The user would then be able to select which record, if any, to overlay.

On the stage-marc-import.pl screen, the wording would change from:
[#] records with at least one match in catalog per matching rule "X"
To
[#] records with one match in catalog per matching rule "X"
[#] records with two or more matches in catalog per matching rule "X"

On the manage-marc-import.pl?import_batch_id=#### screen, each record number that is a match would be displayed (multiple matches). The user would then be able to select (checkbox) which record they would like to overlay. Ideally, they would have the option of selecting none, one, or multiple records.
