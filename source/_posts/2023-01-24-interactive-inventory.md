---
bug: 0
raised: 0
goal: 12000
supporters: 0
date: '2023-01-24 14:57 -0700'
published: true
title: Interactive Inventory
module: Tools
RT: 80182
---
Libraries that are engaged in active weeding are scanning shelves on a regular basis want to ensure that the collection is as accurate as possible for their patrons.  We propose enhancing the inventory module so that it can provide a more interactive experience for librarians and help streamline the inventory process.  

Currently, staff scan a number of item's barcode on a shelf, in a collection and upload that file of scanned barcodes into Koha.  Koha comes back with info about items with non-standard statuses, and missing/lost statuses, etc.  We propose that the item data be presented to staff as they scan the barcodes, right there at the shelf!!!  (For example, staff conducts the inventory with a laptop plus scanner on a cart).


Work to be done:
- Develop a new interface for 'Interactive inventory'
- To begin, the library will scan a book and this item's callnumber will be considered the 'starting' place.
- An option would be created to allow users to provide a manual starting callnumber.  
- Staff could also select options to use Collection code or shelving location to determine upcoming/expected next books
- Koha would display a preview upcoming books to allow librarian to visually scan shelf for next item if out of order
- The above work will require an API route to fetch books in shelf order given configuration settings (collection/location)

As the librarian scans items on the shelf, 
	1. Automatically mark an expected book(s) as 'Missing' when it is not scanned in the planned order
    2. Unmark missing a book that is found out of order on the shelf, and provide feedback to the user that it should be reshelved
