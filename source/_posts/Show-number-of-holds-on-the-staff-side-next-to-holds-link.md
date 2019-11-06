---
title: Show number of holds on the staff side next to 'holds' link
raised: 3000
supporters: 1
date: 'Wed Nov 30 2016 06:18:09 GMT-0500 (EST)'
goal: 3000
short_description: >-
  Show number of holds on the staff side on the search results parenthetical
  next to 'holds' link
tags: koha holds
bug: 14876
module: Funded
published: true
originalmodule: holds
---

![Screenshot](image.png)

# Work to be done
1. Create new module Koha::Template::Plugin::Holds with subroutine count( $biblionumber )
2. Modify koha-tmpl/intranet-tmpl/prog/en/modules/catalogue/results.tt to call this plugin to display the count of holds per record
