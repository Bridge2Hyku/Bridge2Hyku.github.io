---
layout: page-fullwidth
title: "Toolkit"
subheadline:
teaser: "Use these tools to analyze your descriptive metadata and migrate your repository content to Hyku"
header:
    image_fullwidth: "header_unsplash_8.jpg"
permalink: "/toolkit/"
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

## Data Migration

The tools below are available to help move your content out of CONTENTdm and into Hyku.

### CDM Bridge
[https://github.com/Bridge2Hyku/cdm-bridge/releases](bit.ly/cdmbridge)<br>
An Electron desktop application for crosswalking and exporting CONTENTdm metadata. It also provides the option of exporting files from CONTENTdm. CDM Bridge connects to the CONTENTdm API and presents a custom crosswalking interface for each collection. Metadata specialists may use the application to generate lists of field values for cleanup and normalization prior to migration. When a collection is ready for migration CDM Bridge generates a CSV, with or without the files from CONTENTdm, that may be used to ingest the collection into Hyku with HyBridge.

### HyBridge
[https://github.com/Bridge2Hyku/hybridge](http://bit.ly/hykubridge)<br>
HyBridge is a Ruby Gem importer that must be installed within the Hyku application. This importer is integrated in the Hyku Dashboard and pairs with CDM Bridge for a basic migration workflow from a local or hosted CONTENTdm to a hosted Hyku repository. Clients should work with their hosted service provider to have HyBridge installed on their hosted Hyku repository and establish a workflow for staging migration content on the service provider's system. Once HyBridge has been installed and CDM Bridge migration content is available on the provider's staging server, HyBridge provides a simple interface for getting batch content into Hyku.

### CDM Migrator
[https://github.com/Bridge2Hyku/cdm_migrator](http://bit.ly/cdm-migrator)<br>
The CDM Migrator is a Ruby Gem designed for a complete CONTENTdm to Hyku export workflow. After installing the gem in Hyku, the application provides two user interfaces. The first allows migrators to crosswalk and export individual CONTENTdm collections to a CSV for metadata normalization, with or without the files stored in CONTENTdm. It then presents a batch import interface for Hyrax via the exported CSV. The CDM Migrator is ideal for institutions migrating from a local CONTENTdm to a local Hyku repository. Developed by Braydon Justice (University of Victoria).

### Hunting
<https://github.com/uhlibraries-digital/hunting><br>
A Ruby gem that provides CONTENTdm API convenience methods. Hunting is useful as a tool that facilitates export and transformation of legacy descriptive metadata for normalization and migration. Hunting gathers high level information about CONTENTdm collections, including aliases, names, and the number of items in a collection. From there, using methods for iterating through a collection's items or for isolating individual items, Hunting gathers complete descriptive metadata for items in a collection. Hunting is effective for creating descriptive metadata reports for use in tools like OpenRefine. Developed by Andrew Weidner (University of Houston).

## Metadata Normalization

Use the tools below to make sense of your data and normalize it for migration.

### OpenRefine
<http://openrefine.org/><br>
A powerful open source application that allows users to make sense of messy data. [Librarians love it](https://bridge2hyku.github.io/best-practices/librarians-love-openrefine/). It is especially appropriate for understanding your metadata in aggregate. OpenRefine’s faceted browsing abilities let users see how values cluster and how metadata can be cleaned up quickly.  Controlled vocabularies can also be used within OpenRefine’s tools to refine your metadata even more. OpenRefine can get bogged down with too much data, so try to limit the size of data that you load. One easy way is to cut out any metadata that involves more than a few words, such as descriptions or transcripts, in your CSV or spreadsheet before using OpenRefine.  

### AutoHotkey
<https://autohotkey.com/><br>
For Windows users, AutoHotkey (AHK) provides a full-featured desktop automation scripting language. It can be used to create simple scripts that automate repetitive tasks with a custom keyboard hotkey. AHK can also be used to create desktop applications, complete with a GUI, that perform complex data transformation work. Below are a few examples of how AHK can be used to enrich descriptive data and streamline workflows:
- [Workflow Tools for Digital Curation](http://journal.code4lib.org/articles/8419) (Andrew Weidner & Daniel Alemneh, 2013) describes simple scripts for file management and an application for automated data entry.
- [Automated Enhancement of Controlled Vocabularies: Upgrading Legacy Metadata in CONTENTdm](http://dcevents.dublincore.org/IntConf/dc-2014/paper/view/218) (Andrew Weidner, Annie Wu & Santi Thompson, 2014) describes data reconciliation and normalization tools for automatically enriching and standardizing controlled vocabulary data in CONTENTdm.
- [AutoType](https://github.com/metaweidner/AutoType) is a simple AHK application for repetitive data entry.

{% include _improve_content.html %}
</div>
</div>
