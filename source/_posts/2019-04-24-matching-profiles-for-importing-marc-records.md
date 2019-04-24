---
bug: 0
raised: 0
goal: 0
supporters: 0
date: '2019-04-24 11:21 -0500'
published: true
title: Matching Profiles for Importing MARC records!!
---
## Do you import records from vendors and find that each vendor requires special handling upon import for things like encoding, matching rule, overwrite actions, etc.?

This development will allow you to have the ability to create "matching profiles" for use on the "Stage MARC Records for Import" screen. This would make it possible to choose a profile rather than manually filling in each of the fields for record type, encoding, record and item matching rules and actions each time a batch of MARC records is imported. 

For example, we might create "matching profiles" for different vendors or formats, and it would save time to select the appropriate profile (maybe from a drop-down list on the page) and have the fields populate automatically.

Specs:
1. Ability to set up profiles and save them while working in the Tools->StageMarcRecords module. 
2. Ability to manage/change profiles in the Admin area (similar to Record->Matching Rules). 
3. Create an API to pull the profile data into Import Tool when selected on the Import Screen.

