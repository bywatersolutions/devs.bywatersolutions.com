---
bug: 0
raised: 0
goal: 4000
supporters: 0
date: '2022-08-04 10:16 -0600'
published: true
title: Streamline the editing of ILL statuses
module: Circulation
short_description: Update ILL Statuses
RT: 100008
---
## Updating statuses in the Koha ILL module

Currently in the ILL module, statuses are updated through the Manage Request page.  This requires clicking a few times into the request to update the status.  This enhancement simplifies the process to update ILL statuses.  


The development provides a way to access the 'manage request' page easily (fewer clicks) from the View ILL request page.  Changes can be done quicker and easier which will streamline the process of keeping your ILl requests up to date.

The technical details are as follows:

-Adjust API to allow for update of requests
-Add 'Edit request' button to ILL requests table
-Add a modal display of request
-Add JavaScript to update the request when modal form is submitted
