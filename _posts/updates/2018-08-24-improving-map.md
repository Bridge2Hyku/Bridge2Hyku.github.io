---
layout: page
#
# Content
#
title: "Improving your Metadata Application Profile for System Migration"
teaser: "Recommendations for collaboratively improving your metadata application profile."
categories:
  - updates
tags:
  - metadata
  - migration
  - metadata-migration
  - recommendations
  - links

#
# Styling
#
header: no
breadcrumbs: yes
image:
    title: puzzle-title.jpg
    thumb: puzzle-thumb.jpg
    homepage: puzzle-home.jpg
---

 A system migration provides a good opportunity to assess your metadata, improve your input guidelines, and possibly revise your [Metadata Application Profile (MAP)](https://github.com/DLFMetadataAssessment/MetadataSpecsClearinghouse/wiki#application-profiles) altogether.

Some reasons you may want to consider developing a new profile or updating your existing profile are to:
* Take advantage of new metadata properties that provide better access to your resources
* Align your metadata schema more closely with the actual use of elements in your digital library
* Meet the requirements of a new digital library system.
* Simplify your existing set of metadata elements

While this is a useful and likely necessary exercise, it is a significant undertaking. The University of Houston Libraries recently completed a project to revise our MAP in preparation for a migration to a new digital asset management system (DAMS). Below is a summary of our unique experience developing our MAP as well as some general recommendations for those planning similar work.

## Our Process

In 2015, the University of Houston (UH) Libraries chose the open source system Hyku (then known as the Hydra-in-a-Box project) to replace CONTENTdm [<sup>1</sup>](#Footnotes). To meet the technical specifications of the new system and to improve our digital library metadata overall, we initiated a project to revise our MAP.

The University of Houston Digital Library (UHDL) has many stakeholders, and we wanted to make sure they were all represented during the MAP development process. In late 2016, we formed a team of key digital projects stakeholders including: the digital project coordinator and curators from UH Special Collections; and metadata specialists from the Metadata and Digitization Services Department. The group was led by the project manager for the Digital Asset Management System Implementation Team and the Metadata Librarian. The group held bi-weekly meetings and created a [wiki](https://github.com/uhlibraries-digital/bcdams-map/wiki) to communicate between meetings and record the team’s work on GitHub.

At the time, the final Hydra-in-a-Box/Hyku metadata schema had not been finalized, so the team used the [Digital Public Library of American (DPLA) Metadata Application Profile v. 4](https://pro.dp.la/hubs/metadata-application-profile) as a starting point for discussion. We also discussed and developed a shared understanding of the role of particular systems in our digital collections ecosystem. For systems that contain different descriptive metadata, for example a digital library and a finding aid system, it was important to be explicit about the system of record for a particular type of data. This way, we knew what information must be represented in the digital library and what information could remain only in the finding aid system.

We created an issue in GitHub for each field in the evolving [target application profile](https://github.com/uhlibraries-digital/bcdams-map/wiki/04-BCDAMS-Element-Set) and then focused meeting discussion on one or two specific fields, documenting discussion and decisions as we went along. We started with fields that were straightforward and could generally be agreed upon. For example, our current field `dc.title` and input guidelines for titles could easily be mapped to `dcterms:title` without much discussion. We then moved to more complex fields. For example, determining properties and mappings for our `Format`, `Type`, `Genre`, and `Physical Description` fields required lengthier discussions to reach consensus. We used metadata reports from our current digital library to analyze the existing field usage and ultimately make decisions about the elements and guidelines to be used in the new system.

The final deliverables for this group were a [machine actionable MAP](https://vocab.lib.uh.edu/bcdams-map/about) - the [metadata element set](https://vocab.lib.uh.edu/bcdams-map/) and the [input guidelines](https://vocab.lib.uh.edu/bcdams-map/guidelines) - and a [crosswalk](https://github.com/uhlibraries-digital/bcdams-map/wiki/05-UHDL-Crosswalk) from the existing MAP to the new MAP. The entire process took about 10 months to complete, but the MAP continues to evolve as we work on metadata normalization and content migration in earnest.

## Recommendations

Based on the success of our MAP development process, the following recommendations may be useful if you are embarking on a MAP revision or development process:

* Include stakeholders from various teams from the beginning of the process
* Create a shared space to discuss and record decisions
* Develop a shared understanding of the purpose of systems that contain descriptive metadata and establish systems of record
* Provide access to metadata documentation and data from the existing repository
* Document, document, document. You will need to be able to recall decisions that you made and your rationale
* Determine a starting point. Starting a MAP from scratch would likely be too time consuming for a team consisting of stakeholders from a variety of departments. Outlining a starting point with the shared understanding that there is flexibility will help frame initial discussions and move things along

## Resources

To learn more about the details and outcomes of the UH Libraries Descriptive Metadata Working Group, see:

Washington, Anne, Andrew Weidner. Collaborative Metadata Application Profile Development for DAMS Migration. *DCMI International Conference on Dublin Core and Metadata Applications.* Washington, D.C., October 2017. http://hdl.handle.net/10657/2069

### Other examples of mapping work

__University of Oregon Libraries and the Oregon State University:__

Simic, Julia and Sarah Seymore. (2016). From Silos to Opaquenamespace: Oregon Digital’s Migration to Linked Open Data in Hydra. *Art Documentation: Journal of the Art Libraries Society of North America 35*(2), 305-320.
https://doi.org/10.1086/688730

__Artexte, Canadian organization providing access to contemporary arts publications:__

Neugebauer, T., MacDonald, C. & Tayler. (2010). Artexte metadata conversion to EPrints: adaptation of digital repository software to visual and media arts documentation. *International Journal on Digital Libraries, 11*, 263. https://doi.org/10.1007/s00799-011-0077-5

## Examples of Metadata Application Profiles:

Metadata Application Profile Clearinghouse
https://dlfmetadataassessment.github.io/MetadataSpecsClearinghouse/

### Footnotes <a id="Footnotes"></a>

1. Wu, Annie, Santi Thompson, Rachel Vacek, Sean Watkins, Andy Weidner. (2016). Hitting the Road towards a Greater Digital Destination: Evaluating and Testing DAMS at the University of Houston Libraries. *Information Technology and Libraries, 35*(2). https://doi.org/10.6017/ital.v35i2.9152
