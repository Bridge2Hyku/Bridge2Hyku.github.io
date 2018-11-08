---
layout: page
#
# Content
#
title: "Trim that Metadata"
teaser: "Just like the trees in fall, your metadata schema should look a bit slimmer when you remediate it during a migration."
categories:
  - updates
tags:
  - metadata-remediation
  - metadata-migration
  - samvera-migration
  - metadata
#
# Styling
#
header: no
breadcrumbs: yes
image:
    title: leaves-title.jpg
    thumb: leaves-thumb.jpg
    homepage: leaves-home.jpg
---
For many institutions, metadata migration calls for a culling of fields, especially when coming from CONTENTdm.  While CONTENTdm allows different/customizable metadata fields per collection, this is not how many other platforms work, including Hyrax/Hyku. Hyku is based on work types, so that each object type can have a different metadata schema, instead of each collection. 

If you’re planning to migrate from CONTENTdm to another platform, one of the first analyses you should do is an inventory of your metadata fields.  On average, hosted CONTENTdm users have 72 fields across their collections (some users have as many as 900+ fields!).  Quite a bit of trimming and consolidation is required to migrate to a platform like Hyku, where the generic worktype has only 16 fields.  

Below are some examples of what other metadata librarians are trimming: 

!(/leaves-snapshot.png "slack message")

The slack response above should remind you that having fields that won’t have interoperability with other systems is a good place to start with cutting off. 

Anne Washington, Metadata Services Coordinator at University of Houston, was able to turn 8 fields to 2: 
>Creator (LCNAF)<br>Creator (HOT)<br>Creator (ULAN)<br>Creator (Local)<br><br>And<br><br>Subject.Topical (LCSH)<br>Subject.Topical (TGM-1)<br>Subject.Topical (AAT)<br>Subject.Topical (SAA)<br>Subject.Topical (Local)<br><br>Now we have a single field for each: Creator and Subject<br><br>The specificity has been good for migration rework and adding terms to our local vocabulary, but now the relationships for those terms to related controlled vocabs are recorded in our local controlled vocabulary system, Cedar. 

Finally, from Elliot D Williams at the University of Miami:
>One of the areas that we are going to re-examine during our migration is digitization-related metadata. Our current metadata profile has several fields for the equipment and specifications that were used during digitization. However, we haven’t used them consistently. More importantly, that information is recorded elsewhere, as part of our digital projects recordkeeping.  It doesn’t make sense to include it in a system that is primarily oriented towards display of digital content, rather than preservation or management, so we will likely be looking at removing those fields in the next iteration of our metadata profile.
