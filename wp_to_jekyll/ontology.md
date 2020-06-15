---
id: 3380
title: Ontology
date: 2018-12-13T20:10:48+00:00
author: Goksel Misirli
layout: page
guid: http://sbolstandard.org/?page_id=3380
---
The SBOL-OWL ontology provides a set of controlled terms that are used to describe genetic circuit designs using SBOL. Terms are included for the followings.

  * Descriptions of SBOL entities (e.g. &#8220;[ComponentDefinition](http://sbolstandard.org/v2#ComponentDefinition)&#8220;) that are exchanged electronically. Constraints and validation rules that are enforced on SBOL entities are also captured as part of the ontology.
  * SBOL entities (e.g. &#8220;[TopLevel](http://sbolstandard.org/v2#TopLevel)&#8220;) that are not serialised but are used to group different SBOL entities. SBOL-OWL exposes these entities to semantic reasoning tools via parent-child relationships. 
  * Terms (e.g. &#8220;[inline](http://sbolstandard.org/v2#inline)&#8220;) that are used to restrict values of SBOL entities.
  * Properties (e.g. &#8220;[sequence](http://sbolstandard.org/v2#sequence)&#8220;) linking SBOL entities to accepted values.
  * Metadata terms (e.g. &#8220;[Promoter](http://sbolstandard.org/v2#Promoter)&#8220;) for commonly used descriptions of design entities. Such terms may require the use of several SBOL entities and properties.

## Browse

<a href="https://dissys.github.io/sbol-owl/sbol-owl.html" rel="noopener" target="_blank">Browse the SBOL-OWL terms via an HTML page.</a> 

## Download

SBOL-OWL is available in different formats.

  * <a href="https://dissys.github.io/sbol-owl/sbol.owl" rel="noopener" target="_blank">OWL file</a>
  * <a href="https://dissys.github.io/sbol-owl/sbol.rdf" rel="noopener" target="_blank">RDF file</a>
  * <a href="https://dissys.github.io/sbol-owl/sbol.omn" rel="noopener" target="_blank">OMN file (Manchester Syntax)</a>

## Semantic reasoning

SBOL-OWL can be combined with any SBOL document to query genetic circuit designs using semantic queries. The semanticSBOL Java library has been developed to facilitate this process. The resulting files can then be submitted to existing reasoners for semantic inferencing. The library also includes methods to check the consistency of SBOL files, to execute semantic queries, and to list inconsistencies programmatically.

[Click here](https://github.com/dissys/sbol-owl) to access the documentation and examples to use the library programmatically. 

The semanticSBOL library can be used from the command line to merge SBOL files with the SBOL-OWL ontology. 

Usage: sbolowl\_file sboldesign\_file merged_file  
`</p>
<ul>
<li>sbolowl_file: The RDF version of the SBOL-OWL ontology</li>
<li>sboldesign_file: An SBOL file including genetic circuit designs</li>
<li> merged_file: The output file name</ul>
</li>
<p>`

Example:  
`java -cp semanticSBOL-1.0-SNAPSHOT-jar-with-dependencies.jar dissys.keele.ac.uk.RDFMerger sbol.rdf mapsto.rdf mapsto_sbolowl_consistent.rdf`

### Download semanticSBOL

  * [Click here](https://dissys.github.io/sbol-owl/semanticSBOL-1.0-SNAPSHOT-jar-with-dependencies.jar) to download the standalone sbol-sem Java library as a single file including all the dependencies.
  * [Click here](https://dissys.github.io/sbol-owl/semanticSBOL-1.0-SNAPSHOT.jar) to download the sbol-sem Java library only. Dependencies are not included.