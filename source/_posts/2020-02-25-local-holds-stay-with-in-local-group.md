---
bug: 0
raised: 1000
goal: 5000
supporters: 1
date: '2020-02-25 12:57 -0700'
published: true
title: Local Holds Stay with in Local group
module: Holds
short_description: Local Hold Priority Groups
RT: 42268
Supporter1: NEKLS - George for 1000.
---
Upcoming in Koha (estimate 20.05) is the option to add 'Local hold groups'.  This new feature will allow libraries to restrict your items to your a local group *always* and items would never leave your group to fill a hold outside of the group.

If you would like those items to leave your group to fill holds then you may be looking for seomthing we coined 'Local hold priority groups'.  This is best described by the example below:

A Library consortium is made up of 3 districts which includes 14 libraries (or branches).  
- District A with 3 libraries: Main, West, East 
- District B with 6 libraries
- District C with 1 library

In this example...
District A is made up of small rural libraries that share funding amongst the 5 libraries. The collections are moderate and the patron base is on the smaller side. They **consider** themselves 1 library with 3 branches.
District B is based in a large city.  It has 6 branches and one source of funding for new materials.  It's well funded and has a large patron base. 
District C is the suburban area and has 1 branch.  It's also funded well and has medium large patron base.   

When an item from District A is purchased, the libraries in that District would prefer to allow the 5 District A libraries to have preference on holds before sending the item to District B or District C.  What happens currently is that items in District A are being sent consistently to the larger districts with large patron bases with lots of hold requests which slows access to the libraries in District A from using the items in their libraries.

This development will allow for the creation of these hold priority groups.  All patrons in the priority group would be given priority over holds from other groups.  Within the priority group all libraries branches are considered equal and would be filled in the order they exist in the queue.

If a we have a biblio with 3 items system wide - 1 owned by District A MAIN, 1 owned by District B -branch 2 and  1 owned by District C.  District A and District C are 'priority groups'

And now imagine the title has 30 requests on it in this order:

01 request at District C 
02 request at District B - branch 1
03 request at District B - branch 1
04 request at District C 
05 request at District A - EAST
06 request at District B - branch 5
07 request at District C 
08 request at District C 
09 request at District B - branch 6 
10 request at District C 
11 request at District B - branch 5 
12 request at District B - branch 4 
13 request at District A - EAST
14 request at District C 
15 request at District B - branch 4
16 request at District C 
17 request at District B - branch 4
18 request at District B - branch 3
19 request at District B - branch 2 
20 request at District B - branch 3
21 request at District C 
22 request at District B - branch 2
23 request at District A - WEST
24 request at District B - branch 1
25 request at District C 
26 request at District B - branch 2 
27 request at District B - branch 1
28 request at District B - branch 5
29 request at District B - branch 2
30 request at District C 

Requests 05, 13, 23 should be filled by the District A MAIN copy in chronological order
Requests 1,4,7,8,10,14,16,21,25,30 should be filled by the District C copy in chronological order

And then all of the other requests should be filled in chronological order once the prioritized requests have been filled.  For example, once hold 23 is filled for District A, that item is free to fill a hold at District B