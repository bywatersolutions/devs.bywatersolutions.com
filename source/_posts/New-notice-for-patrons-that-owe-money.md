---
title: New notice for patrons that owe money
raised: 0
supporters: 0
date: 2016-11-30 11:46:07
goal: 2000
short_description: The goal of this development is to be able to send a notice to patrons that owe money on a monthly basis
tags: koha notices notice fine fines fee fees
bug: 15507
module: Accounting
---

![Screenshot](image.png)

# Work to be done
1. Write a script that will
    1. Accept a report number as a parameter
        1. The only required parameter would be ‘template_borrowernumber’ and maybe ‘template_branch’ so each library could have a separate template
    1. Accept a notice module/code as a parameter

All the columns output by the report would be available to the template via the script. The script would generate a notice and queue it for sending for each result row in the query.
