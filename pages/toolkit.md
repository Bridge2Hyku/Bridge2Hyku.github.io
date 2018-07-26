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

The tools below are available to help move your content out of CONTENTdm.

### CDM Migrator

The [CDM Migrator](https://github.com/UVicLibrary/cdm_migrator) is designed to export individual CONTENTdm collections to a CSV for metadata normalization. It then provides a batch import interface for Hyrax via a CSV upload. Developed by Braydon Justice (University of Victoria).

### CDM Bridge

An Electron application in development for mapping and exporting CONTENTdm metadata. It also provides the option of exporting files from CONTENTdm.

### Hunting

A [Ruby gem](https://github.com/uhlibraries-digital/hunting) for pulling metadata and info from CONTENTdm. Developed by Andrew Weidner (University of Houston).

## Metadata Normalization

Use the tools below to make sense of your data and normalize it for migration.

### OpenRefine

[Open Refine](http://openrefine.org/) is a powerful open source application that allows users to make sense of messy data.

### AutoHotkey

For Windows users, [AutoHotkey](https://autohotkey.com/) (AHK) provides a full-featured desktop automation scripting language. It can be used to create simple scripts that automate repetitive tasks with a custom keyboard hotkey. AHK can also be used to create desktop applications, complete with a GUI, that perform complex data transformation work. Below are a few examples of how AHK can be used to enrich descriptive data and streamline workflows:
- [Workflow Tools for Digital Curation](http://journal.code4lib.org/articles/8419) (Andrew Weidner & Daniel Alemneh, 2013) describes simple scripts for file management and an application for automated data entry.
- [Automated Enhancement of Controlled Vocabularies: Upgrading Legacy Metadata in CONTENTdm](http://dcevents.dublincore.org/IntConf/dc-2014/paper/view/218) (Andrew Weidner, Annie Wu & Santi Thompson, 2014) describes data reconciliation and normalization tools for automatically enriching and standardizing controlled vocabulary data in CONTENTdm.
- [AutoType](https://github.com/metaweidner/AutoType) is a simple AHK application for repetitive data entry.


{% include _improve_content.html %}
</div>
</div>
