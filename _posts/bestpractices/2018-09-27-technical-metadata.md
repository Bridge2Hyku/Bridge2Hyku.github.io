---
layout: page
#
# Content
#
title: "Hyku’s Underlying Metadata"
teaser: "Within Hyku’s stack lies Fedora, which creates a layer of technical metadata that might be useful for you."
categories:
  - best-practices
tags:
  - metadata
  - fedora
  - samvera

#
# Styling
#
header: no
breadcrumbs: yes
image:
    title: levels-title.jpg
    thumb: levels-thumb.jpg
    homepage: levels-home.jpg
---
One of the reasons to move to Hyrax/Hyku from legacy systems is the underlying RDF-based Fedora-4 layer, so it is important to understand what this means for your metadata and data as a whole. Work at Indiana University has created two great documents to help you understand Fedora’s metadata and a switch from XML to RDF:

: Fedora Metadata Storage Philosophy (PDF, 2007)<br>[https://wiki.dlib.indiana.edu/spaces/flyingpdf/pdfpageexport.action?pageId=441](https://wiki.dlib.indiana.edu/spaces/flyingpdf/pdfpageexport.action?pageId=441)

: The Semantics of Metadata: Avalon Media System and the Move to RDF (2017)<br>[https://journal.code4lib.org/articles/12668](https://journal.code4lib.org/articles/12668)

So while objects in Hyku have most of their metadata at the generic work level, [available to view here](/migration/#model-work-types), theres still quite a few things that exist at the Fedora level, [some of which is shown here.](https://wiki.duraspace.org/display/samvera/Technical+Metadata+Application+Profile)

Below are the fields shown in a sample generic object in Hyku within the Fedora GUI. 

<table>
  <tr>
    <th>Prefix</th>
    <th>Predicate</th>
  </tr>
  <tr>
    <td>acl:</td>
    <td>accessControl</td>
  </tr>
  <tr>
    <td>dc:</td>
    <td>creator</td>
  </tr>
 <tr>
    <td>dc:</td>
    <td>relation</td>
  </tr>
 <tr>
    <td>dcterms:</td>
    <td>dateSubmitted</td>
  </tr>
 <tr>
    <td>dcterms:</td>
    <td>isPartOf</td>
  </tr>
 <tr>
    <td>dcterms:</td>
    <td>modified</td>
  </tr>
 <tr>
    <td>dcterms:</td>
    <td>title</td>
  </tr>
 <tr>
    <td>ebucore:</td>
    <td>hasRelatedImage</td>
  </tr>
 <tr>
    <td>ebucore:</td>
    <td>hasRelatedMediaFragment</td>
  </tr>
 <tr>
    <td>fedora:</td>
    <td>created</td>
  </tr>
 <tr>
    <td>fedora:</td>
    <td>createdBy</td>
  </tr>
 <tr>
    <td>fedora:</td>
    <td>hasParent</td>
  </tr>
 <tr>
    <td>fedora:</td>
    <td>lastModified</td>
  </tr>
 <tr>
    <td>fedora:</td>
    <td>lastModifiedBy</td>
  </tr>
 <tr>
    <td>fedora:</td>
    <td>writable</td>
  </tr>
 <tr>
    <td>iana:</td>
    <td>first</td>
  </tr>
 <tr>
    <td>iana:</td>
    <td>last</td>
  </tr>
 <tr>
    <td>ldp:</td>
    <td>contains</td>
  </tr>
 <tr>
    <td>ns001:</td>
    <td>hasModel</td>
  </tr>
 <tr>
    <td>ns002:</td>
    <td>rights</td>
  </tr>
 <tr>
    <td>ns003:</td>
    <td>hasMember</td>
  </tr>
 <tr>
    <td>ns005:</td>
    <td>dpt</td>
  </tr>
 <tr>
    <td>ns006:</td>
    <td>objState</td>
  </tr>
 <tr>
    <td>rdf:</td>
    <td>type</td>
  </tr>
</table>


