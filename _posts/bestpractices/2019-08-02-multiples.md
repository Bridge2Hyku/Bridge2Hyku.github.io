---
layout: page
#
# Content
#
title: "How to Ingest Multiple Worktypes with the B2H Toolkit"
teaser: "If you decide to create multiple worktypes in your Hyrax/Hyku, here is how to work that into the migration workflow"
categories:
  - best-practices
tags:
  - metadata-schema
  - metadata-migration
  - hybridge
  - cdm-bridge
#
# Styling
#
header: no
breadcrumbs: yes
image:
    title: multiples-title.jpg
    thumb:  multiples-thumb.jpg
    homepage:  multiples-home.jpg
---
Using [CDM Bridge](https://github.com/Bridge2Hyku/cdm-bridge/wiki) to help with your migration? If you’ve decided to add non-generic worktypes to your instance of Hyku/Hyrax (more on that [here](https://bridge2hyku.github.io/best-practices/dogbiscuits/))  then you will be required to manually edit your CDM Bridge CSVs.  This is one of the few manual processes required to migrate your content using the Bridge2Hyku workflow.  


When you open any CSV created by CDM Bridge, the first column will always be Object Type, and by default this will include “GenericWork” at the object level and “File” for files attached to that object.  As shown here:

<img src="https://raw.githubusercontent.com/Bridge2Hyku/Bridge2Hyku.github.io/master/images/non-edited-cdmbridge-csv.PNG">

If you attempt to import this CSV with HyBridge into a Hyrax/Hyku instance where GenericWork has been customized to another type, **it will fail**. So you must edit this value to fit with your customizations. For example, if you created “Image” or “Text” works in Hyrax/Hyku, you would need to edit values in Object Type to match those: 

<img src="https://raw.githubusercontent.com/Bridge2Hyku/Bridge2Hyku.github.io/master/images/edited-cdmbridge-csv.PNG">

Along with these edits, you will have to think carefully about how multiple worktypes with different metadata schemas will affect your metadata migration. You will likely be required to change the crosswalk in CDM Bridge (Under Preferences -> Export Fields, for more see the [CDM Bridge wiki](https://github.com/Bridge2Hyku/cdm-bridge/wiki))) to capture the unique fields to each worktype. 

Once you have made these modifications, your import to HyBridge should work like a charm and you should see all of your new items in the repository, with their respective work type(s), once the import is complete. 

