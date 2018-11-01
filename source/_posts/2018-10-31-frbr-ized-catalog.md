---
bug: 0
raised: 0
goal: 22000
supporters: 0
date: '2018-10-31 14:36 -0400'
published: true
title: FRBR-ized Catalog
short_description: FRBR-ized Catalog
tags: 'Featured, Catalog'
---
## FRBR-ized Catalog

### We're looking for sponsors to bring a FRBR-ized catalog in to Koha. Below you will find our 5 phase approach and associated costs which will bring a FRBR style catalog in to Koha. 


A FRBR-ized catalog can enable users to find what they are seeking by collocating bibliographic records that are related to other bibliographic records. This document will outline the steps needed to attain a FRBR style catalog. Bibliographic records will be assigned a GroupID that relates to the FRBR concept of 'work'. All related bibliographic records will need the GroupID assigned. Searches will pull the groups of bibliographic records with the same GroupID and display the bibliographic records to users. We propose a 5 phase approach to this development as outlined below.

**Phase 1** will set the architecture needed for subsequent phases. A MARC tag and subfield will be added to bibliographic frameworks to hold the GroupID. This MARC tag will be configurable through settings and can be unique to each library. The default MARC tag if none is specified will be 998 subfield a. Secondly, a new database table will be created that stores all the GroupIDs, description of the work, and source of the id. The initial implementation will only have a single "local" source. Future development (in phase5) will utilize the source field.

**Phase 2** allows catalogers to assign GroupIDs to the bibliographic record. GroupIDs can be added to bibliographic records in three ways.
1. A button is provided when cataloging. Clicking on the button brings a new popup window where GroupIDs can be searched and selected for addition to the bibliographic record
2. If no existing GroupID is found when cataloging, the cataloger can add a new GroupID in the popup window and it will be created and assigned to the bibliographic record.
3. If the cataloger previously created the GroupID and the number is known, they can manually add it to the tag/subfield when cataloging.

**Phase 3** will allow for the display of the grouped bibliographic records in the OPAC. The exact specifics of the display have not been determined at this point. It is expected that the most relevant biblioographic record in the group will be displayed first and all other related bibliographic records will appear under the main record.

**Phase 4** involves the removal of duplicate search results. Once a bibliographic record is displayed, as a primary result or related result, it will not display itself as a primary result in the search results.

**Phase 5** is a future development that depends on external sources of data such as MANA KB or BookBrainz. The expected functionality is that we can link Koha bibliographic records to an external source using a standard id (e.g. ISBN/ISSN/UPC). This linking would be done either at the time of cataloging or through a nightly cron. Future development may involve linking existing GroupIDs to other GroupIDs. (For example, fan fiction Fifty Shades GroupID is linked to Twilight Series GroupID). The display of primary Groups or linked Groups would also need to be addressed.


**Technical specifications**

**Phase 1** - Add a "group ID" to the bibliographic record.
a - The groupID will be stored in the koha database for use in grouping and fetching records
b - The groupID will be stored in the MARC record as well
c - The groupID will also contain a 'source' field, this way multiple group IDs can use different sources of truth

**Phase 2** - Build a system for entering the groupID
a - The initial method will allow for adding/grouping manually

**Phase 3** - Records containing a group ID will display the other records containing the same group ID on the results or details page
a - Provide an API to retrieve records by GroupID
b - Develop OPAC display using React or similar framework

**Phase 4** - Filter duplicate record results (if one record refers to another, don't return the second as a unique result)
a - This development will be targeted at the Elasticsearch engine

**Phase 5** - Develop a system for storing the group ID and allowing lookup by ISBN
a - This may use the MANA system in development for Koha
b - This may use an outside source such as 'Bookbrainz' as it matures
c - This will be exapandable to allow for multiple future linkings

**Cost:
Phase 1 - $4000
Phase 2 - $2000
Phase 3 - $8000
Phase 4 - $8000
Phase 5 - This requires the other developments and further discussion before pricing**
