---
title: Override fix loan period
raised: 1500
supporters: 1
date: 'Wed Nov 30 2016 23:27:33 GMT-0700 (Mountain Standard Time)'
goal: 1500
short_description: >-
  When checking out to someone that is homebound or in a limited access area
  (such as a bookmobile that comes through once a month), it is necessary to set
  a fixed loan period. There needs to be a way to override this feature on the
  fly.
bug: 0
module: Funded
published: true
originalmodule: circulation
---

When checking out to someone that is homebound or in a limited access area (such as a bookmobile that comes through once a month), it is necessary to set a fixed loan period. There needs to be a way to override this feature on the fly. This development will make it so that there is an option next to the Specify Due Date field on check out to force the due date to remain regardless of other settings.

# Work to be done
* Add a checkbox to circulation.pl for “Don’t decrease loan length based on holds” which would cause Koha to ignore the decreaseLoanHighHolds system preference as long as the checkbox is checked.
* Add an option for the system to remember if it’s checked or not to keep it checked as well.
* Create a staff permission to allow an override.
