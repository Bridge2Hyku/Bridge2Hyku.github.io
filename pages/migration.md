---
layout: page-fullwidth
title: "Migration"
teaser: "Learn how to assess your current repository content and prepare it for a move to another system"
header:
    image_fullwidth: "header_unsplash_8.jpg"
permalink: "/migration/"
---
<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**Table of Contents**
{: #toc }
*  TOC
{:toc}
</div>
</div>

<div class="medium-8 medium-pull-4 columns" markdown="1">

## Migration Overview

Data migration for digital collections is a complex process. As with most difficult tasks, it can be helpful to break down what needs to be done into smaller blocks of work. In general, data migrations can be divided into four sub-tasks, each with their own sets of outcomes, tools, and techniques: Migration Planning, Metadata Normalization, Content Migration, and Content Verification.

The following sections describe the importance of each of these steps in more detail and provide resources for effectively planning and executing your next content migration. This page does not assume that you have chosen a target system for your migration or that you are migrating from a specific source platform. This information is intended as a general migration guide for both new and seasoned digital collections professionals.

## Migration Planning

Careful planning is arguably the most important step in migration.

Each situation is unique.

How migration fits in with other systems: preservation, library catalog, etc.

### Content Analysis

Data Types

File Types

File Locations

### Metadata Analysis

Metadata Schema

Data Quality

## Normalize Metadata

_add content here..._

### Before Export

_add content here..._

### In Transit

_add content here..._

### After Import

_add content here..._

## Migrate Content

Once you’ve normalized your metadata, you have to move it into your new system.  If you are moving onto a hosted platform, this might require another round of metadata changes to accommodate the platform’s framework. The steps here include: identify the platform’s requirements, crosswalk your schema to the new one, export your content, and finally import your content.

### Model Work Types

Your new digital asset management system should have some basic way of housing metadata. In some systems, like CONTENTdm, the metadata profile is based on the collection. In Hyku/Hyrax, metadata is structured around a work type. Hyku currently uses a “generic work”, which is a Dublin Core-based schema that is standard for Hyrax. The two most important pieces of information to gather from your new platform are the schema preference (Dublin Core, MODS, MARC, etc.)  and the fields available.  

A Hyku generic work has 16 fields

<table>
  <tr>
    <th>Field</th>
    <th>Required</th>
    <th>Predicate</th>
    <th>Definition</th>
  </tr>
  <tr>
    <td>Title</td>
    <td>✓</td>
    <td>dct:title</td>
    <td>A name to aid in identifying a resource.</td>
  </tr>
  <tr>
    <td>Creator</td>
    <td>✓</td>
    <td>dce:creator</td>
    <td>The person or group responsible for the resource. Usually this is the author of the content. Personal names should be entered with the last name first, e.g. “Smith, John”.</td>
  </tr>
  <tr>
    <td>Keyword</td>
    <td>✓</td>
    <td>dce:relation</td>
    <td>Words or phrases you select to describe what the resource is about. These are used to search for content.</td>
  </tr>
  <tr>
    <td>Rights statement</td>
    <td>✓</td>
    <td>edm:rights</td>
    <td>Indicates the copyright and reuse status of the resource. While licenses cannot always be asserted, a rights statement can be. See <a href="RightsStatements.org">RightsStatements.org</a> for more information.</td>
  </tr>
  <tr>
    <td>Contributor</td>
    <td> </td>
    <td>dce:contributor</td>
    <td>A person or group you want to recognize for playing a role in the creation of the resource, but not the primary role.</td>
  </tr>
  <tr>
    <td>Description</td>
    <td> </td>
    <td>dce:description</td>
    <td>Free-text notes about the resource. On Hyku's dashboard it is called “Abstract or Summary"</td>
  </tr>
  <tr>
    <td>License</td>
    <td> </td>
    <td>dct:rights</td>
    <td>Licensing and distribution information governing access to the work.</td>
  </tr>
  <tr>
    <td>Publisher</td>
    <td> </td>
    <td>dce:publisher</td>
    <td>The person or group making the resource available.</td>
  </tr>
  <tr>
    <td>Date created</td>
    <td> </td>
    <td>dct:created</td>
    <td>The date on which the resource was created. Strongly recommended to select a particular date encoding (such as EDTF) to guide date formats.</td>
  </tr>
  <tr>
    <td>Subject</td>
    <td> </td>
    <td>dce:subject</td>
    <td>Headings or index terms describing what the resource is about; these need to conform to an existing vocabulary (Keywords should be used for uncontrolled values).</td>
  </tr>
  <tr>
    <td>Language</td>
    <td> </td>
    <td>dce:language</td>
    <td>The language of the resource’s content. Best practice is to select a language representation to follow, such as <a href="http://id.loc.gov/vocabulary/iso639-1.html">ISO 639-1</a> or full names taken from a controlled vocabulary.</td>
  </tr>
  <tr>
    <td>Identifier</td>
    <td> </td>
    <td>dct:identifier</td>
    <td>A unique handle identifying the resource. This does not affect the identifier minted for managing your resource in Hyku.</td>
  </tr>
  <tr>
    <td>Location</td>
    <td> </td>
    <td>foaf:basedNear</td>
    <td>A place name related to the resource, such as its site of publication, or the city, state, or country the work contents are about. Best practice is to select, if possible, one definition (such as ‘place of origin of the work’) for this field across objects in a collection or collections in your repository.</td>
  </tr>
  <tr>
    <td>Related URL</td>
    <td> </td>
    <td>rdfs:seeAlso</td>
    <td>A link to a website or other specific content (audio, video, PDF document) related to the resource.</td>
  </tr>
  <tr>
    <td>Source</td>
    <td> </td>
    <td>dct:source</td>
    <td>An identifier for a related resource from which the described resource is derived, in whole or in part.</td>
  </tr>
  <tr>
    <td>Resource Type</td>
    <td> </td>
    <td>dct:type</td>
    <td>Pre-defined categories in Hyku to describe the type of content being uploaded. More than one type may be selected.</td>
  </tr>
</table>

For more information regarding these Fields, including expected values and examples, please visit the <a href="https://docs.google.com/document/d/1RXRT08236E98RTKASX-bL60qLoBeZgYXFUSD4XBOIa">_Hyku Metadata Documentation (DRAFT)_</a> and <a href="https://gist.github.com/cmh2166/723bebaee52d9ba4eb68eebc904484">_Hyrax Metadata Technical Documentation_</a>. 

### Map Metadata

Once you know your target system’s metadata schema, you will need to map your current schema to it.  <a href="https://www.getty.edu/publications/intrometadata/metadata-matters/#fn:2">The Getty Institute</a> “refer[s] to _mapping_ as the intellectual activity of comparing and analyzing two metadata schemas, and to _crosswalks_ as the visual product of mapping.”

Many of these crosswalks have become standardized and are available from the Library of Congress. Here are some examples:  

<ul><li><a href="http://www.loc.gov/marc/dccross.html">Dublin Core to MARC</a></li>
    <li><a href="http://www.loc.gov/standards/mods/dcsimple-mods.html">Dublin Core to MODS</a><li>
    <li><a href="http://www.loc.gov/marc/marc2dc.html">MARC to Dublin Core</a></li>
    <li><a href="https://www.loc.gov/standards/mods/mods-mapping.html">MARC to MODS</a></li></ul>
    
Crosswalking is not always as simple as changing the field name, as laid out in the white paper <a href="https://groups.niso.org/publications/white_papers/crosswalk/">"Issues in Crosswalking Content Metadata Standards"</a> (1998)  by St. Pierre and LaPlant. Some common issues are:

<ul><li><strong>One-to-Many:</strong> When an element in your current schema has separate elements in your target system.  Example: if your current system only uses "date", it’s possible to enter a schema that has multiple date fields.</li>
    <li><strong>No clear binary:</strong> When an existing element has no clear equivalent in the new system. This occurs often when the granularity of your system is higher than that of the target. Typically this will result in a broader list of entries within the keywords or description fields. When confronting this challenge, you will often lose specificity or may choose to omit fields from your existing metadata altogether.</li>
    <li><strong>Structural differences:</strong> Some schemas (EAD, etc) allow for hierarchical metadata, while others (MARC, etc) are flat. </li>
    
There are no easy ways around the issues above, and your institution’s decisions on these should come from internal knowledge and context. CONTENTdm and Hyku both use Dublin Core, so the crosswalking required is at the field-level and will require mapping decisions that could be unique to your CONTENTdm instance or even your individual collections.  The Bridge2Hyku toolkit includes CDM-Bridge which comes preloaded with Hyku’s standard target metadata to get you a head start on determining your mapping and easily exporting your metadata through it.  
    


### Source Repository Export

_add content here..._

### Target Repository Import

_add content here..._

## Content Verification

_add content here..._

### Data Integrity

_add content here..._

### Data Presentation

_add content here..._

## Migration Resources

### Deciding to Make The Leap 

- <a href="http://www.dlib.org/dlib/september15/stein/09stein.html">Taking Control: Identifying Motivations for Migrating Library Digital Asset Management Systems</a><br>_Ayla Stein and Santi Thompson (October 2015)_

- <a href="http://hdl.handle.net/10657/1575">Hitting the Road towards a Greater Digital Destination: Evaluating and Testing DAMS at the University of Houston Libraries</a><br>_Annie Wu, Santi Thompson, Rachel Vacek, Sean Watkins, and Andrew Weidner (June 2016)_

- <a href="https://www.slideshare.net/DuraSpace/32818-open-source-repository-upgrades-top-advice-from-practitioners-webinar-recording">Open Source Repository Upgrades: Top Advice from Practitioners</a><br>_Duraspace (March 2018)_

- <a href="https://journal.code4lib.org/articles/8327">Breaking Up With CONTENTdm: Why and How One Institution Took the Leap to Open Source</a><br>_Heather Gilbert and Tyler Mobley (April 2013)_

- <a href="https://www.bepress.com/webinar/evaluating-planning-completing-successful-migration-case-study/">Evaluating, Planning, and Completing a Successful Migration: A Case Study</a><br>_Elizabeth Chance (2018)_

### Metadata Migration Resources 

- <a href="http://dcpapers.dublincore.org/pubs/article/view/3861">Collaborative Metadata Application Profile Development for DAMS Migration</a><br>_Anne Washington and Andrew Weidner (2017)_

- <a href="http://dcpapers.dublincore.org/pubs/article/view/3773">Metadata Quality Control for Content Migration: The Metadata Migration Project at the University of Houston</a><br>_Andrew Weidner and Annie Wu (2015)_

- <a href="http://dcevents.dublincore.org/IntConf/dc-2014/paper/view/218">Automated Enhancement of Controlled Vocabularies: Upgrading Legacy Metadata in CONTENTdm</a><br>_Andrew Weidner, Annie Wu, and Santi Thompson (2014)_

- <a href="https://www.getty.edu/publications/intrometadata/">Getty Institute's Introduction to Metadata 3rd Edition</a><br>_Edited by Murtha Baca (2016)_

{% include _improve_content.html %}

</div>
</div>
