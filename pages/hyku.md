---
layout: page-fullwidth
title: "Hyku"
subheadline:
teaser: "Learn about what Hyku offers for your institution"
header:
    image_fullwidth: "header_unsplash_8.jpg"
permalink: "/hyku/"
---
<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
{: #toc }
*  TOC
{:toc}
</div>
</div>

<div class="medium-8 medium-pull-4 columns" markdown="1">

## National Digital Platform {#national-digital-platform}

Hyku, the repository software produced by the Hydra-In-a-Box project, was built as a part of the Institute for Museum and Library Services' <a href="https://www.imls.gov/issues/national-issues/national-digital-platform">National Digital Platform</a> initiatve. It strives to be <a href="http://hydrainabox.samvera.org/">"a feature-rich, robust, flexible digital repository that is easy to install, configure, and maintain."</a>

## Hyku vs Hyrax vs Omeka {#product-comparison}

Hyku is an "out of the box" version of the Samvera community's Hyrax repository platform. If you do not have any web developers on staff or already plan to use a consortium to help offload technical issues, Hyku might be the right fit for you. Check out <a href="https://wiki.duraspace.org/pages/viewpage.action?pageId=85530575">this article</a> on Hyku's wiki. If you have developers on staff and are looking to have customized workflows and tech specs, consider using <a href="http://hyr.ax/">Hyrax</a> and joining the <a href="http://samvera.org/">Samvera community</a>. If you're looking to build an online exhibition or digital humanities project, <a href="https://omeka.org/news/2010/09/21/omeka-and-peers/">Omeka is a wonderful tool</a>. If you're looking to build a robust institutional repository or digital collections system, you might be better served by the Fedora/Solr/Blacklight-backed Hyku.  

## Hyku Features {#hyku-features}

These are just some of the features listed in Hyku's <a href="https://wiki.duraspace.org/display/hyku/Hyku+Features">current documentation</a>.

* <strong>Responsive interface</strong> – Displays clearly and is usable on the range of screen sizes and mobile devices.
* <strong>Redesigned, consolidated dashboard</strong> – A single interface with advanced tooling to access all administrative and management tasks and reporting.
* <strong>Batch work upload</strong> – Upload multiple files to create multiple works of the same work type.
* <strong>Highlighted Work</strong> – A depositor can designate works to be highlighted on their User Profile.
* <strong>DPLA ready</strong> – Crosswalks directly to DPLA Metadata Application Profile v4.
* <strong>Faceted search and browse</strong> – Powered by Blacklight, an intuitive interface makes it easy to search and find content quickly.

## Hyku Metadata Schema {#metadata}

In Hyku, the metadata is based around work types.  The Generic work that comes standard out of the box includes 16 fields that comply with DPLA harvesting and are listed below. 

<table>
  <tr>
    <th>Field</th>
    <th>Required</th>
    <th>Predicate</th>
    <th>Definition</th>
  </tr>
  <tr>
    <td>Title</td>
    <td>X</td>
    <td>dct:title</td>
    <td>A name to aid in identifying a resource.</td>
  </tr>
  <tr>
    <td>Creator</td>
    <td>X</td>
    <td>dce:creator</td>
    <td>The person or group responsible for the resource. Usually this is the author of the content. Personal names should be entered with the last name first, e.g. “Smith, John”.</td>
  </tr>
  <tr>
    <td>Keyword</td>
    <td>X</td>
    <td>dce:relation</td>
    <td>Words or phrases you select to describe what the resource is about. These are used to search for content.</td>
  </tr>
  <tr>
    <td>Rights statement</td>
    <td>X</td>
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

## Institutional Repository {#institutional-repository}

Hyku is a good fit for institutional repository use cases, with out of the box support for self-deposit workflows and robust access controls.

## Cultural Heritage Repository {#cultural-heritage}

The Hyku development community is still working on adding functionality for cultural heritage use cases. The Hyku Pilot that occured in 2017 included a <a href="https://docs.google.com/document/d/1mpYLs2pqwKDCCxF0Kb-JTC4OjPLgmbJ6d1IBunxHqAw/edit?usp=sharing">gap assessment document</a> that should help determine whether or not Hyku is a good fit for your institution.


{% include _improve_content.html %}
</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
