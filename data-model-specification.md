---
id: 1290
title: SBOL Data Model Specifications
date: 2016-06-01T21:13:37+00:00
author: Chris Myers
layout: page
guid: http://sbolstandard.org/?page_id=1290
---
[Report an Issue with the Current SBOL Specification](https://github.com/SynBioDex/SBOL-specification/issues)

<table style="border-color: #ffffff; background-color: #ffffff;" align="center">
  <tr>
    <td width="70%">
      <h3>
        3.x.x Release
      </h3>
    </td>
    
    <td style="text-align: right;" colspan="2" width="30%">
      &nbsp;
    </td>
  </tr>
  
  <tr>
    <td width="70%">
      <p>
        <strong><em style="font-family: inherit; font-weight: inherit;">3.0.0</em></strong>
      </p>
      
      <em style="font-family: inherit; font-weight: inherit;">Condenses and simplifies previous versions of SBOL, separates sequence features from part/sub-part relationships, renames ComponentDefinition/Component to Component/SubComponent, merges Component and Module classes, ensuring consistency between data model and ontology terms, extends the means to define and reference SubComponents, refines requirements on object URIs, enables graph-based serialization, moves Systems Biology Ontology (SBO) for Component types, makes all sequence associations explicit, makes interfaces explicit, generalizes SequenceConstraints into a general structural Constraint class, and expands the set of allowed constraints.</em>
    </td>
    
    <td style="text-align: right;">
      <a href="https://sbolstandard.org/wp-content/uploads/2020/04/SBOL3.0specification.pdf">Specification</a>
    </td>
    
    <td style="text-align: right;">
      &nbsp;
    </td>
  </tr>
</table>

<table style="border-color: #ffffff; background-color: #ffffff;">
  <tr>
    <td width="70%">
      <h3>
        2.x.x Release
      </h3>
    </td>
    
    <td style="text-align: right;" colspan="2" width="30%">
      <a href="http://sbolstandard.org/software/libsbol/">Library Implementation</a>
    </td>
  </tr>
  
  <tr>
    <td width="70%">
      <strong>2.3.0</strong><br /><em>Includes means of succinctly representing sequence modifications, an extension to support organization and attachment of experimental data, and an extension for describing numerical parameters of design elements. The new version also includes<br />specifying types of synthetic biology activities, unambiguous locations for sequences with multiple encodings, and refinement of a number of validation rules.</em>
    </td>
    
    <td style="text-align: right;">
      <a href="http://sbolstandard.org/wp-content/uploads/2016/06/SBOL2.3.0.pdf">Specification</a>
    </td>
    
    <td style="text-align: right;">
      &nbsp;
    </td>
  </tr>
  
  <tr>
    <td width="70%">
      <strong>2.2.1</strong><br /><em>Clarification on ontology terms on roles for proteins and small molecules, refining a number of validation rules, and illustrating a design for combinatorial derivations using Prov-O.</em>
    </td>
    
    <td style="text-align: right;">
      <a href="http://sbolstandard.org/wp-content/uploads/2016/06/SBOL-data-model-2.2.1.pdf">Specification</a>
    </td>
    
    <td style="text-align: right;">
      &nbsp;
    </td>
  </tr>
  
  <tr>
    <td width="70%">
      <strong>2.2.0</strong><br /><em>Introduces new classes for representing combinatorial genetic designs, physical implementations of genetic designs, and attachments to external files. It also adds best practices for using existing classes to encode provenance for the Design-Build-Test-Learn cycle.</em>
    </td>
    
    <td style="text-align: right;">
      <a href="http://sbolstandard.org/wp-content/uploads/2018/01/BBF-RFC114-SBOL2.2.0.pdf">Specification</a>
    </td>
    
    <td style="text-align: right;">
      <a href="https://doi.org/10.1515/jib-2018-0001">Cite</a>
    </td>
  </tr>
  
  <tr>
    <td width="70%">
      <strong>2.1.0</strong><br /><em>A backwards-compatible release extending the data model and updating ontology terms and best practices.</em>
    </td>
    
    <td style="text-align: right;">
      <a href="http://sbolstandard.org/wp-content/uploads/2016/10/BBF-RFC112-SBOL2.1.0.pdf">Specification</a>
    </td>
    
    <td style="text-align: right;">
      <a href="https://www.degruyter.com/view/j/jib.2016.13.issue-3/jib-2016-291/jib-2016-291.xml">Cite</a>
    </td>
  </tr>
  
  <tr>
    <td width="70%">
      <strong>2.0.1</strong><br /><em>An updated version of SBOL 2.0 data model to refine validation rules.</em>
    </td>
    
    <td style="text-align: right;">
      <a href="http://sbolstandard.org/wp-content/uploads/2015/08/SBOLv2.0.1.pdf">Specification</a>
    </td>
    
    <td style="text-align: right;">
      &nbsp;
    </td>
  </tr>
  
  <tr>
    <td>
      <strong>2.0.0</strong><br /><em>An extension of version 1.1 data model to allow flexibility and extendibility of the following: Represent non-DNA structural components of a biological design; Describe the behavioral aspects of a biological design; Associate structure and function to a design; Support rich annotation of biological designs.</em>
    </td>
    
    <td style="text-align: right;">
      <a href="http://sbolstandard.org/wp-content/uploads/2015/08/BBF-RFC108-SBOL2.0.pdf">Specification</a>
    </td>
    
    <td style="text-align: right;">
      <a href="https://www.ncbi.nlm.nih.gov/pubmed/26528570">Cite</a>
    </td>
  </tr>
</table>

<!--TABLE 1.X.X SECTION -->

<table style="border-color: #ffffff; background-color: #ffffff;" align="center">
  <tr>
    <td width="70%">
      <h3>
        1.x.x Release
      </h3>
    </td>
    
    <td style="text-align: right;" colspan="2" width="30%">
      &nbsp;
    </td>
  </tr>
  
  <tr>
    <td width="70%">
      <strong>1.1.0</strong><br />Define the vocabulary that contain a set of preferred terms and the core data model composed of a common computational representation, to enable the electronic exchange of information describing DNA components used in synthetic biology.
    </td>
    
    <td style="text-align: right;">
      <a href="http://whub44.webhostinghub.com/~sbolst5/wp-content/uploads/2014/12/BBFRFC87.pdf"><span style="color: #191e23;">Specification</span></a>
    </td>
    
    <td style="text-align: right;">
      <a href="http://www.nature.com/nbt/journal/v32/n6/full/nbt.2891.html"><span style="color: #191e23;">Cite</span></a>
    </td>
  </tr>
</table>