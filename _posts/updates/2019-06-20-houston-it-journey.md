---
layout: page
#
# Content
#
title: "How’s Your Migration Going? UHouston-IT edition"
teaser: "Our pilot partner migration story series continues with University of Houston’s Lead Developer’s answers."
categories:
  - updates
tags:
  - partner-story
  - lessons-learned
  - case-study
#
# Styling
#
header: no
breadcrumbs: yes
image:
    title: journey-title.jpg
    thumb: journey-thumb.jpg
    homepage: journey-home.jpg
---

The University of Houston has been the Bridge2Hyku project’s primary hub.  We’re lucky enough to have received questionnaires from their metadata strategist and lead developer.  Below is the response from Sean Watkins, UH’s Lead Repository Developer. View Anne Washington (Metadata Service Coordinator at UH)’s response [HERE](/updates/houston-metadata-journey/). 


**Original Platform?**<br>
CONTENTdm


**New Platform?**<br>
Custom repository using Hyrax.


**Is this the Platform you had originally planned to migrate to?**<br>
No


**If not, please elaborate on the reasons to pivot**<br>
We set out to use Hyku during its initial announcement and development. After our evaluation of Hyku, it didn’t meet our needs as a valid replacement for CONTENTdm. Although Hyku continues to be developed by other institutions, there is no guarantee our specific needs would be addressed in new releases. Additionally, other features dedicated to our institutional needs would still have to be developed in-house. Because Hyku was developed using the Hyrax stack and many future features of Hyku are planned to be brought into Hyrax, we felt that putting our development efforts into developing our own repository using Hyrax would benefit us in the long term. 


**Broadly, How is your migration going?**<br>
We are approaching a Minimal Viable Product (MVP) for our Hyrax repository. Some migration efforts have already started and we’ll soon be developing tools to assist in migration. Current plans are underway to improve tools to help scale our migration.


**What have been the biggest obstacles?**<br>
Learning and understanding the full Hyrax stack in order to make our customizations have been the biggest obstacle. Documentation is minimal. The documentation that is provided has been extremely helpful for certains areas, but doesn’t cover the full extent of Hyrax that is needed to ensure best practices and onboard new Hyrax developers.


**What’s gone well?**<br>
With the provided documentation we have been able to setup our repository quickly thanks to the Hyrax stack. We have been able to implement many features in a short amount of time.


**What lessons have you learned?**<br>
Having a focused group can go a long way and setting clear goals and broad paths to those goals is a good jumping off point. Be mindful of change and adjust to those constant changes, because they will happen. Work out details along the way. Don’t try to plan everything in the beginning, it will almost always end in failure that could bring you back to the beginning. Working out details as you go will help your team adjust to change and to address failures quickly as you continue to iterate in development and migration.


**What customizations to the platform have you had to do?**<br>
Here’s the current list of features we are implementing for our MVP:

- Full UH Libraries branding
- Homepage focused on searching and browsing the repository
- Custom work types with metadata fields matching our current Metadata Application Profile (MAP)
- Batch ingest tool tailored to our other workflow tools
- Customized search results page to highlight important metadata fields and views
- Streamlined item view page to highlight metadata fields, rights, and link to finding aid
- Custom IIIF viewer to focus on single and paged image content
- Ability to download different image sizes
- Restrict item access via IP address
- Restrict item downloads
- Jobs to link items via our ARK system
- Jobs to link items to ArchivesSpace


**What feature are you most excited about having?**<br>
I think supporting IIIF will benefit the repository the most, however, all the features above are exciting as they get us closer to a more well rounded, feature rich repository from now and into the future.
 
 
**What advice would you share with those currently considering or beginning a migration?**<br>
Having a small cross functional group (people from IT, metadata, digitization, etc.) focused on the migration. Setting up good communication channels that are used often with the migration team and stakeholders can avoid a lot of confusion and missing details during your migration process. Follow the communities using your new platform and try to be active when possible. This can go a long way when needing support and future planning.

 
*Want to see the other B2H Partner’s migration questionnaires?*<br>
Go to our [Migration Stories Page](/partner-stories/)
