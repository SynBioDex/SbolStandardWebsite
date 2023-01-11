---
id: 648
title: SBOL 12 Workshop Report
date: 2015-05-05T13:09:19+00:00
author: Goksel Misirli
layout: post
guid: http://sbolstandard.org/?p=648
permalink: /sbol-12-workshop-at-harmony-2015/
categories:
  - Announcements
  - Archives
---
The 12th SBOL workshop took place as part of [HARMONY 2015](http://old_co.mbine.org/events/HARMONY_2015 "HARMONY 2015") on April 20-24, 2015, at  at the <a class="external text" href="http://www.leucorea.de/" rel="nofollow">Leucorea Wittenberg</a>, part of the <a class="external text" href="http://www.uni-halle.de/" rel="nofollow">Martin Luther University Halle-Wittenberg</a>, Germany.

## SBOL Posters:

Curtis Madsen: [SBOL Stack: The One-stop-shop to Storing and Publishing SBOL Data](https://github.com/SynBioDex/Community-Media/blob/master/posters/sbolstack_poster.pdf)  
Tramy Nguyen: [Synthetic Biology Open Language (SBOL) 2.0](https://github.com/SynBioDex/Community-Media/blob/master/posters/softwareinfra-syntheticbiology.pdf)

## Here are the outcomes of the meeting:

  1. SBOL 2.0 Specification 
      1. Significant work was performed on the specification, no decision TODOs remain.  Goal is to finish writing by SEED.
      2. Ontologies selected, when possible, for those needing them. Identifiers.org  to provide the ontology terms.
      3. No significant changes to data model though some required fields changed to optional, especially those with no clear ontology.  Other minor changes include: Interactions no longer require a participation, displayId was moved to Identified, roles removed from Model. Roles in other entities were made optional.
      4. Discussed the linking of ModuleDefinition entities to corresponding ComponentDefinitions
  2. libSBOLj 2.0 Release 
      1. Agreed that beta release will support only compliant URIs. 
          1. TopLevel: <prefix>/<type>/<displayId>/<version>
          2. 1st level child: <prefix>/<type>/<parentId>/<displayId>/<version>
          3. NOTE: also decided <version> is optional.
      2. Agreed that validation errors would be reported through exceptions.
      3. Agreed that beta release would have complete docs with simple examples.
      4. Tested libSBOLj in several applications: 
          1. Nicholas Roehner &#8211; SBOL to SBML converter.
          2. Tramy Nguyen &#8211; SBML to SBOL converter.
          3. Newcastle Group &#8211; VirtualParts Repository, SBOL Stack, and SynBad
          4. Bryan Der &#8211; Cello
          5. Neil Swanston &#8211; (Metabolic) SBML to SBOL converter. Integration with genome-scale models.
      5. Beta release planned before SEED.
  3. Publication Plan 
      1. Abstract on 2.0 submitted to IWBDA.  Hope to submit to special ACS Synthetic Biology special issue.
      2. SBOLv paper is currently under review.
      3. libSBOLj paper under review at IEEE Life Science Letters
      4. libSBOLc paper under development.
  4. Outreach Plan 
      1. Decided to make a new sbol-announce mailing list, make sbol-dev and sbol-visual public lists, and add old SBOL editors to sbol-editors list.
      2. Discussed several improvements to website such as making logos more prominent, better emphasis of international community and industrial supporters. We also need to keep the SBOL tools up to date.
      3. Talked about international advisory board for SBOL
      4. A SEED talk is scheduled to talk about SBOL, the community, and supporting tools
  5. SBOLv and SBGN 
      1. Had dedicated session to interaction with SBGN.
      2. Got a better understanding of the SBGN capabilities.
      3. Conveyed our requirements to SBGN.
      4. Matthew Pocock will continue to follow up with them.

&nbsp;
