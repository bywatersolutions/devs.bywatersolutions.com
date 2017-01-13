---
title: Search serials by barcode
raised: 1000
supporters: 1
date: 2016-11-30 11:24:34
goal: 1000
short_description: Allow serials to be searched by barcode from the top search bar and the advanced searched
tags: koha serials
bug: 14875
module: Serials
---

![Screenshot](image.png)

# Work to be done
1. Modify quick search to add barcode field ( may need to make it hidden by default ala the patron quick search
2. Modify the advanced search to add barcode field
3. Modify serials-search.pl to accept barcode as a parameter
4. Modify SearchSubscriptions to accept barcode as a parameter
