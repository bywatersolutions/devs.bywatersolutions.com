---
title: Clearing Z39.50 search fields
goal: 1000
raised: 1000
supporters: 1
date: 'Wed Nov 30 2016 23:42:53 GMT-0700 (Mountain Standard Time)'
short_description: >-
  Add a button on the Z39.50 search form that will reset all the fields to
  blank.
in_koha_release: 3.2
bug: 0
module: Funded
published: true
originalmodule: cataloging
---

When doing multiple z39.50 searches one after another, it would be helpful if there was a way to clear all the entries in the z39.50 in one fell swoop instead of having to remove each field individually. This development will add a button on the Z39.50 search form that will reset all the fields to blank.

# Work to be done
* Add “clear form” button to the search form
* Add javascript to clear all form fields when clicked

# Updates
A member of the Koha community has already submitted a patch for this same functionality.  Their patch has passed QA and is well on it's way to a release.  To read more on the patch, please go to http://bugs.koha-community.org/bugzilla3/show_bug.cgi?id=7741
