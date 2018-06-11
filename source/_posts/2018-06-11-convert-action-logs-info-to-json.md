---
bug: 15296
raised: 0
goal: 6000
supporters: 0
date: '2018-06-11 11:09 -0400'
published: true
title: Convert action_logs.info to JSON
short_description: Action_logs does not give enough detail. This will help resolve this issue.
---
## Work to be done:

Convert action_logs.info to JSON

1) Mode code to store json in info column.

2) Database update to convert existing D::D info to JSON.

3) Add code to store diffs of changed patron in JSON in action_logs.info.
