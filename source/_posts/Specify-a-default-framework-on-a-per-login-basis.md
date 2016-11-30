---
title: Specify a default framework on a per-login basis
raised: 0
supporters: 0
date: 2016-11-30 11:07:52
goal: 3000
short_description: Specify a default framework on a per-login basis
tags: koha marc framework frameworks
bug: 15786
---

![Screenshot](image.png)

# Goal of development
To be able to specify a default framework on a per-login basis

# Work to be done
1. Add new field ‘frameworkcode’ to table ‘borrowers’
2. Revail in the patron editor as “Preferred framework”
3. Make the selected framework the default for new records
4. If editing existing record that does not match preferred framework, pop up confirmation dialog asking/warning to switch to new framework
