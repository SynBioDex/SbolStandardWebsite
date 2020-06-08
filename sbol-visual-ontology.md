---
id: 3698
title: SBOL Visual Ontology
date: 2020-03-03T18:13:41+00:00
author: Goksel Misirli
layout: page
guid: https://sbolstandard.org/?page_id=3698
---
The SBOL Visual Ontology (SBOL-VO) provides a set of controlled terms to describe visual glyphs for genetic circuit designs. The terms are organised based on their descriptions in community-edited&nbsp;[Markdown](https://github.com/SynBioDex/SBOL-visual/tree/master/Glyphs)&nbsp;files. Terms are defined for recommended and alternative glyphs in addition to terms to represent generic glyphs. SBOL-VO consists of the following items.

  * **Terms for glyphs** to represent
      * DNA sequence features (e.g. &#8220;<a href="http://sbols.org/visual/v2#CDSGlyph" target="_blank" rel="noreferrer noopener" aria-label=" (opens in a new tab)">CDSGlyph</a>&#8220;, &#8220;<a rel="noreferrer noopener" aria-label=" (opens in a new tab)" href="http://sbols.org/visual/v2#AptamerGlyph" target="_blank">AptamerGlyph</a>&#8220;, &#8220;<a rel="noreferrer noopener" aria-label=" (opens in a new tab)" href="http://sbols.org/visual/v2#AssemblyScarGlyph" target="_blank">AssemblyScarGlyph</a>&#8221; and &#8220;<a rel="noreferrer noopener" aria-label=" (opens in a new tab)" href="http://sbols.org/visual/v2#AssemblyScarGlyphAlternative" target="_blank">AssemblyScarGlyphAlternative</a>&#8221; )
      * different types of molecular entities (e.g. <a rel="noreferrer noopener" aria-label=" (opens in a new tab)" href="http://sbols.org/visual/v2#ProteinGlyph" target="_blank">ProteinGlyph</a>)
      * binary molecular interactions (e.g. &#8220;<a rel="noreferrer noopener" aria-label=" (opens in a new tab)" href="http://sbols.org/visual/v2#InhibitionGlyph" target="_blank">InhibitionGlyph</a>&#8220;)
      * molecular interactions with multiple participants (e.g. &#8220;<a rel="noreferrer noopener" aria-label=" (opens in a new tab)" href="http://sbols.org/visual/v2#AssociationGlyph" target="_blank">AssociationGlyph</a>&#8220;).
  * **A base term**. The base term in the ontology is called &#8220;Glyph&#8221;.
  * **Properties**. SBOL-VO includes object properties such as &#8220;hasGlyph&#8221; and &#8220;isAlternativeOf&#8221; to define the relationships between different terms.
  * **Annotations**. Terms are annotated using properties such as &#8220;defaultGlyph&#8221; and &#8220;recommended&#8221;.
  * **Ontological axioms**. Logical axioms restricting the use of SBOL-VO terms to specific biological roles and processes. 

## Browse

<a href="http://sbols.org/visual/v2" target="_blank" rel="noreferrer noopener" aria-label=" (opens in a new tab)">Browse the SBOL-VO terms via an HTML page.</a>

The ontology can also be viewed after downloading and opening in an ontology editor, such as Protege. 

## Download

SBOL-VO is available as an RDF file.&nbsp;[Click here](http://synbiodex.github.io/SBOL-visual/Ontology/v2/sbol-vo.rdf)&nbsp;to download the ontology. 

## Computational access: The SBOL-VO web service (SBOL-VOWS) 

**An HTTP-based glyph service**: The SBOL-VO web service(SBOL-VO-WS) has been developed to resolve SBOL-VO glyphs via an REST-based HTTP interface. The matching glyph is returned by using a term from the SBOL-Visual Ontology, the Sequence Ontology (SO) or the Systems Biology Ontology (SBO). The&nbsp;`http://{SBOL-VO-WS}/glyph/{ONTOLOGY_TERM}"}`&nbsp;REST interface returns glyphs. When a term from the SO or the SBO is used and there is no exact match, then a glyph is returned using the closest mathing parent term. The following example demonsrates retrieving the aptamer glyph by using the corresponding SBOL-VO or terms from the SO:

  * <a href="http://vows.sbolstandard.org/glyph/AptamerGlyph" target="_blank" rel="noreferrer noopener" aria-label=" (opens in a new tab)">http://vows.sbolstandard.org/glyph/AptamerGlyph</a>
  * <a rel="noreferrer noopener" aria-label=" (opens in a new tab)" href="http://vows.sbolstandard.org/glyph/SO:0000031" target="_blank">http://vows.sbolstandard.org/glyph/SO:0000031</a>
  * <a rel="noreferrer noopener" aria-label=" (opens in a new tab)" href="http://vows.sbolstandard.org/glyph/SO:0000033" target="_blank">http://vows.sbolstandard.org/glyph/SO:0000033</a>

The web service returns the default PNG images. The PNG and SVG versions can be retrieved explicitly by appending &#8220;/svg&#8221; or &#8220;/png&#8221; to the query interface :

  * <a rel="noreferrer noopener" aria-label=" (opens in a new tab)" href="http://vows.sbolstandard.org/glyph/SO:0000031/svg" target="_blank">http://vows.sbolstandard.org/glyph/SO:0000031/svg</a>
  * <a href="http://vows.sbolstandard.org/glyph/SO:0000031/png" target="_blank" rel="noreferrer noopener" aria-label=" (opens in a new tab)">http://vows.sbolstandard.org/glyph/SO:0000031/png</a>

**Mapping glyphs to terms from ontologies**: Tools can also use the SBOL-VO-WS to get the mapping information and then to subsequently include glyphs, using the&nbsp;`http://{SBOL-VO-WS}/mapping/{ONTOLOGY_TERM}"}`&nbsp;interface. The mapping interface works similar to the glyph interface but it returns information in the JSON format. This interface includes information about the closest parent term, for which a glyph is assigned, and the parent term&#8217;s distance to the query term. URL examples below return information about AptamerGlyph.

  * <a rel="noreferrer noopener" aria-label=" (opens in a new tab)" href="http://vows.sbolstandard.org/mapping/SO:0000031" target="_blank">http://vows.sbolstandard.org/mapping/SO:0000031</a>
  * <a href="http://vows.sbolstandard.org/mapping/SO:0000033" target="_blank" rel="noreferrer noopener" aria-label=" (opens in a new tab)">http://vows.sbolstandard.org/mapping/SO:0000033</a>

**Searching for glyphs**: The SBOL-VO-WS can be used to search for glyphs using the&nbsp;`http://{SBOL-VO-WS}/query/{ONTOLOGY_TERM}"}`&nbsp;REST interface. This query interface is the reverse of the mapping interface and returns information about glyphs using a query term and for all its child terms. Glyphs are searched for by using a term from the SBOL-Visual Ontology, the Sequence Ontology or the Systems Biology Ontology. Examples:

  * Returning information about the CDSGlyph and CDSAlternativeGlyph terms:
      * <a rel="noreferrer noopener" aria-label=" (opens in a new tab)" href="http://vows.sbolstandard.org/query/CDSGlyph" target="_blank">http://vows.sbolstandard.org/query/CDSGlyph</a>
      * <a rel="noreferrer noopener" aria-label=" (opens in a new tab)" href="http://vows.sbolstandard.org/query/SO:0000316" target="_blank">http://vows.sbolstandard.org/query/SO:0000316</a>
  * Returning information about all glyphs that represent molecular interactions:
      * <a href="http://vows.sbolstandard.org/query/SBO:0000231" target="_blank" rel="noreferrer noopener" aria-label=" (opens in a new tab)">http://vows.sbolstandard.org/query/SBO:0000231</a>

**Retrieving metadata about glyphs**: The SBOL-VO-WS can also be used to retrieve metadata about SBOL Visual glyphs, using the for glyphs using the&nbsp;`http://{SBOL-VO-WS}/metadata/{SBOL-VO-TERM}"}`&nbsp;REST interface. Examples:

  * <a href="http://vows.sbolstandard.org/metadata/CDSGlyph" target="_blank" rel="noreferrer noopener" aria-label=" (opens in a new tab)">http://vows.sbolstandard.org/metadata/CDSGlyph</a>

### Programmatic access to SBOL-VOWS

Python and Java examples and related documentation can be found in the following GitHub repository: 

<a href="https://github.com/dissys/sbol-visual-client" target="_blank" rel="noreferrer noopener" aria-label=" (opens in a new tab)">https://github.com/dissys/sbol-visual-client</a> 

The web service returns data using the RDF/JSON format. Hence, any RDF or JSON library can be used to access information regarding the mapping, query, and metadata interfaces. Please note that examples are provided using the RDFLib and Jena libraries for Python and Java programming languages respectively.