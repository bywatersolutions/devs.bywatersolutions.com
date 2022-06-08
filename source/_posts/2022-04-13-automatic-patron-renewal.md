---
bug: 26888
raised: 0
goal: 3000
supporters: 0
date: '2022-04-13 12:33 -0600'
published: true
title: Automatic Patron Renewal
RT: 84534
module: Patrons
short_description: Auto Renew Patrons
---
##  Automatic Patron Account Renewal

We are proposing an option to make it easy for a patron to have their library membership automatically renew based on their activity at the library. 


When membership renewals come up for a patron, it would be useful for libraries to make a decision about automatic renewals of membership, based on current activity at the library. This would be a benefit/advantage for users who don't come into the physical branch but who do use curbside or electronic services. If Koha could look at borrowers.lastseen - last time a patron has been seen (connected at the OPAC or accessed through the staff interface), this could be used as a way to identify that activity and renew the patron accordingly. 

Use Case: Patron A places holds in the OPAC and requests curbside pickup on a regular basis.  They haven't been inside the library to use self check or checkout at the circ desk in 2 years.  Their account is due expire on 6/1/2022.  When the expiration date draws near, Koha will check the settings for autorenew (autorenew if active within 120 days) and if the patron has logged into the opac in the last 120 days, they are renewed per the patron category rules.

Use Case 2: Patron B only uses ersources at the library.  They have logged into Overdrive in May 2022.  Their account is set to expire May 31, 2022.  The library is set up to autorenew patrons who have been active in the past 60 days.  When Koha checks for expiration, this patron meets the time frame for activity and is renewed per the category rules.


$3000
Work to be done:
- Patron categories will have setting for 'Auto-renew if active within X days'
- A value of 0 (or unset) will disable automatic patron renewal
- Check lastseendate and if within 'active range' renew the patron per rules in the category
- Membership expiry cron should be used to notify patrons of the automatic renewal (and fee if applicable)
