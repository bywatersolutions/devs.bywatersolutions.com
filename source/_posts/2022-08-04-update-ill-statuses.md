---
bug: 0
raised: 0
goal: 4000
supporters: 0
date: '2022-08-04 10:26 -0600'
published: true
title: Update ILL statuses
module: Circulation
short_description: ILL Status Updates
RT: 100008
---

When updating ILL statuses in Koha, the user must access the "Manage Request" page to do so.  This enhancment provides an easier way to access that page (fewer clicks) from the View ILL requests screen (see below).

The proposed solution:
-Adjust API to allow for update of requests
-Add 'Edit request' button to ILL requests table
-Add a modal display of request
-Add JavaScript to update the request when modal form is submitted



![ILL-module-item-statuses.png]({{site.baseurl}}/source/images/ILL-module-item-statuses.png)