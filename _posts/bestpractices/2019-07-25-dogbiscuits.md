---
layout: page
#
# Content
#
title: "Metadata: CONTENTdm Collections vs Samvera Worktypes"
teaser: "When thinking through your metadata schema crosswalk, it’s important to understand the beginning and end "
categories:
  - best-practices
tags:
  - metadata-schema
  - metadata-migration
  - migration-strategy
#
# Styling
#
header: no
breadcrumbs: yes
image:
    title: dogbiscuits-title.jpg
    thumb: dogbiscuits-thumb.jpg
    homepage: dogbiscuits-home.jpg 
---

In Samvera, metadata schemas are decided at the worktype level. This differs dramatically from CONTENTdm, which houses these decisions at the collection level.  Out of the box Hyrax/Hyku only has one worktype, this means you will likely need to create more worktypes to suit your needs, and/or you will need to crosswalk into a more simplified schema.

What is a worktype in Samvera? “Works represent resources proper, ie. the resources we are managing in our repository and want to describe, such as a thesis, the work depicted by an image, a dataset etc.”

If you are the technical part of your migration, one of the most helpful gems to add to your Samvera stack (along with Hybridge!) is [Dog Biscuits](https://github.com/samvera-labs/dog_biscuits).  This gem helps automate the process of creating models and worktypes, which can be a lengthy process if done manually.  Consider looking at [Dog Biscuits’ wiki](https://github.com/samvera-labs/dog_biscuits/wiki) to help contextualize what your technical needs might be when migrating to Hyku to help work with your metadata specialists and non-technical migration team. 

If you are non-technical, Bridge2Hyku’s migration toolkit includes documentation surrounding [Metadata Analysis](https://bridge2hyku.github.io/migration/#metadata-analysis), and thinking through [crosswalking to Hyku’s model worktypes](https://bridge2hyku.github.io/migration/#model-work-types).  It is important to look at your digital library as a whole when working through the change between collection-based metadata and item-based metadata.  Here are some high-level questions to ask your team when sitting down to do this work: 

* What fields could be subsumed as additional entries into “Notes” or “Description”? 
* Does our institution have any unusual required fields? (These are likely fields that cannot be crosswalked as easily and might require technical additions to your Hyku/Hryax instance)
* What fields are we using that are specific to our needs in CONTENTdm?
* What would be the benefits of having different worktypes in the new repository? What are the drawbacks?
