---
title: Show number of holds on the staff side next to 'holds' link
raised: 0
supporters: 0
date: 2016-11-30 11:18:09
goal: 3000
short_description: Show number of holds on the staff side on the search results parenthetical next to 'holds' link
tags: koha holds
bug: 14876
---

![Screenshot](image.png)

# Work to be done
1. Create new module Koha::Template::Plugin::Holds with subroutine count( $biblionumber )
2. Modify koha-tmpl/intranet-tmpl/prog/en/modules/catalogue/results.tt to call this plugin to display the count of holds per record
