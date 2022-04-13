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


When membership renewals come up for a patron, it would be useful for libraries to make a decision about automatic renewals of membership, based on current activity at the library. This would be a benefit/advantage for users who don't come into the physical branch but who do use curbside or electronic services. If Koha could look at borrowers.lastseen - last time a patron has been seen (connected at the OPAC or staff interface), this could be used as a way to identify that activity and renew the patron accordingly. 


$3000
Work to be done:
- Patron categories will have setting for 'Auto-renew if active within X days'
- 0 or unset will disable patron renewal
- Check lastseendate if within range renew
- Membership expiry cron should be used to notify patrons of the automatic renewal (and fee if applicable)
