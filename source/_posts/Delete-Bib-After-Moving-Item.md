---
title: Delete Bib After Moving Item
raised: 0
supporters: 0
date: 2016-11-30 12:25:04
goal: 2000
short_description: After moving an item to a different bib, have the system prompt you to delete the first bib.
tags: koha delete bib biblio cataloguing record
bug:
---

![Screenshot](image.png)

# Expected outcome of development

1. After item is moved from Record A to Record B, check to see if any items remain on Record A
2. If no items remain on Record A, add a new button to the move item confirmation screen for “Delete record item was moved from”
3. Clicking the button will spawn an ajax process to delete the record
4. The button will be replaced with a confirmation of the success or failure of the record deletion
5. The librarian will then be able to use the “OK” or “Attach another item” buttons as usual.
