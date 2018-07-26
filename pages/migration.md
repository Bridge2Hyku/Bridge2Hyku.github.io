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

Careful planning is arguably the most important step in migration. It requires consideration of both the larger context in which the migration takes place as well as an assessment of the content of the current digital collections and an understanding of the requirements of the system to which you are migrating. While this section aims to outline general guidance for migration planning, it is important to keep in mind that each situation is unique. A thoughtful analysis of these different factors will allow you to be better prepared for migration.

### Contextual Considerations

__Institutional Characteristics__

The broader context in which a migration takes place will shape many of the decisions made. Some points to consider include: 
<ul>
    <li>Type, size, and budget of institution:
        <ul><li>These indicate the broader goals of the organization and and overall picture of resources that may be available. Additionally, there may be state or city policies that may impact elements of the migration process.</li>
        </ul>
    <li>Digital collections staffing:
        <ul><li>These will likely be key personnel in a migration. Understanding of the people, expertise, and financial resources available will shape the approach you take to a migration. Some factors to consider include:
            <ul><li>The overall number of staff supporting digital collection management</li>
                <li>The number of IT professionals supporting digital collection management</li>
                <li>The departments of staff supporting digital collection management</li>
            </ul>
        </ul>
</ul>

__Digital Collection Management__

Other contextual considerations specifically around the management of your digital collections are useful to keep in mind when forming a project team: 
<ul>
    <li>Primary stakeholders for your digital collections</li>
    <li>Intended audience(s) for your digital collections</li>
    <li>Structures, committees, and policies in place related to the administration of digital collections.
        <ul><li>This may include individuals or groups that create policy, have technical administrative control over the repository, etc.</li></ul>
    <li>What system interactions and dependencies exist around digital collections?
        <ul><li>For example, the ILS pulls digital collection data from an API, etc.</li></ul>
            </li>
        </ul>
        
### Digital Library Analysis

Making a full assessment of your digital library content, including the types of resources included and the condition of your metadata gives you an overall view of the condition of your digital library and reveals the type of pre-work you may need to plan for before migrating.
 
This analysis is typically most useful when compiled collection by collection, and formatted in such a way to enable visualization of patterns and needs across collections. This exercise also helps identify collections that may be simplest for testing and those that are most challenging.

Overall information that is useful to collect: 

* Number of digital collections to be migrated (Free text)
* Number of digital objects to be migrated (Free text)
* Total size (TB) of digital objects to be migrated (Free text)


### Content Analysis

__Data Types__

This is focused on the type and structure of the digital objects in your current system. What type of content is in your digital library? How are your digital objects structured now? Can they be accomodated in the new system? This is one example of some ways you may characterize content:

* Single sided photograph
* Double sided photograph
* Single sided document
* Multi-page document
* Single audio
* Multi-part audio
* Single video
* Multi-part video file
* Hierarchical work
* Multiple file types (e.g. audio/video file with image or PDF)

__File Types__

An inventory of file formats currently in use will help you create a full picture of your collections and will underscore your decisions moving forward. What file types will be produced or migrated for access purposes? Does the target system support those file types? Do you require copies or production of other file types for access or preservation?

* Examples of file types include: JPEG, TIFF, PDF, MP3, MP4 and others.

__File Locations__

As new standards are implemented and staff come and go, file management practices change. A migration provides an opportunity for an inventory of your files. While migration tools may provide you with the option to migrate existing files or derivatives directly from your current digital library to a new system, you may decide to upload files from your local file system. If you plan for the latter, locating these files, organizing them, and moving them to an accessible or centralized location may be a good strategy and should be a consideration when planning your migration. 

### Metadata Analysis

To adequately plan and prepare for migration, it is crucial to have a deep understanding of your existing metadata as well as the metadata requirements of the new system. The following areas of focus can provide you with insight to inform migration decisions.

__Metadata Profiles__
What is/are the metadata profile(s) for your current digital collections?
<ul><li>What schema(s) are used?
        <ul><li>Examples: Dublin Core, MODS, MARC, EAD, Local metadata schema, etc.</li></ul></li>
    <li>Is the same schema used across your entire digital library or does it vary by collection?</li>
    <li>What fields are required?</li>
    <li>What data type(s) populate those fields?
        <ul><li>Examples: Strings, Numbers, URIs</li></ul></li>
    <li>What controlled vocabularies are used?
        <ul><li>Examples: Library of Congress Name Authority File (LCNAF), Library of Congress Subject Headings (LCSH), Thesaurus of Geographic Names (TGN), DCMI Type Vocabulary, Local vocabulary, etc.</li></ul></li>
    </ul>
    
What is the metadata profile for your new repository? (See examples above)

* What schema(s) are used?
* Is the same schema used across the entire entire digital library or does it vary in some way?
* What fields are required?
* What data type(s) populate those fields?
* What controlled vocabularies are used/suggested?

__Data Quality__

Assessing your current metadata quality will help you make decisions around metadata remediation needs, timing, and strategies. Consulting resources on metadata quality and remediation strategies can help frame your analysis and path forward, but the following areas of focus will give you a broad view of metadata quality in your collections.

Do you have local metadata input guidelines?
Have metadata values been entered consistently across your digital collections?
Does you metadata -  elements and/or values - align with any other standards or best practices?
* Examples: Describing Archives: A Content Standard (DACS), The Digital Public Library of American Application Profile (DPLA-MAP), etc.

How do you indicate copyright in your digital collections?
* What metadata field(s) are used?
* What values appear in this field? Varying local statements? Standard local statements? Rightsstatements.org values or URIs?

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
    <li><a href="http://www.loc.gov/standards/mods/dcsimple-mods.html">Dublin Core to MODS</a></li>
    <li><a href="http://www.loc.gov/marc/marc2dc.html">MARC to Dublin Core</a></li>
    <li><a href="https://www.loc.gov/standards/mods/mods-mapping.html">MARC to MODS</a></li></ul>
    
Crosswalking is not always as simple as changing the field name, as laid out in the white paper <a href="https://groups.niso.org/publications/white_papers/crosswalk/">"Issues in Crosswalking Content Metadata Standards"</a> (1998)  by St. Pierre and LaPlant. Some common issues are:

<ul><li><strong>One-to-Many:</strong> When an element in your current schema has separate elements in your target system.  Example: if your current system only uses "date", it’s possible to enter a schema that has multiple date fields.</li>
    <li><strong>No clear binary:</strong> When an existing element has no clear equivalent in the new system. This occurs often when the granularity of your system is higher than that of the target. Typically this will result in a broader list of entries within the keywords or description fields. When confronting this challenge, you will often lose specificity or may choose to omit fields from your existing metadata altogether.</li>
    <li><strong>Structural differences:</strong> Some schemas (EAD, etc) allow for hierarchical metadata, while others (MARC, etc) are flat. </li></ul>
    
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
