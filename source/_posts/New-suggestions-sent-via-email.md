---
title: New suggestions sent via email
raised: 2000
supporters: 1
date: 'Wed Nov 30 2016 09:55:31 GMT-0500 (EST)'
goal: 2000
short_description: >-
  Allow email alerts to be sent to librarians when new suggestions are created
  by patrons.
tags: koha acquisitions suggestions email
bug: 5770
module: Funded
published: true
originalmodule: acquisitions
---

# Goal
To allow email alerts to be sent to librarians when new suggestions are created by patrons.

# Plan of attack
1. Create new notice for email alert
2. Modify C4::Suggestions::NewSuggestion to send an email to the branch email address or KohaAdminEmailAddress if the branch email does not exist
3. add a system pref for a new email address for this so it would check the pref first, the branch email address second, and the KohaAdminEmailAddress last

# Updates

A member of the Koha community is currently working on this feature. You can follow the status of the work by going to Bug #5770 in Bugzilla.
