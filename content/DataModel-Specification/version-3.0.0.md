---
title: SBOL Data Model Version 3.0.0
date: '2020-04-01'

# Variables in the data specification template
version: 3.0.0
specification: /docs/SBOL3.0.0.pdf
citation: https://www.degruyter.com/view/journals/jib/ahead-of-print/article-10.1515-jib-2020-0017/article-10.1515-jib-2020-0017.xml


# Provide an alias for identifiers.org (See GitHub #195)
aliases:
    - /specifications/sbol/version-3.0.0

links:
- icon: file-pdf
  icon_pack: fas
  name: Specification
  url: docs/SBOL3.0.0.pdf
- icon: pen-fancy
  # icon: keyboard
  icon_pack: fas
  name: Cite
  url: https://www.degruyter.com/view/journals/jib/ahead-of-print/article-10.1515-jib-2020-0017/article-10.1515-jib-2020-0017.xml
- icon: passport
  icon_pack: fas
  name: Identifier
  url: http://identifiers.org/combine.specifications/sbol.version-3.0.1

---

Condenses and simplifies previous versions of SBOL, separates sequence features from part/sub-part relationships, renames ComponentDefinition/Component to Component/SubComponent, merges Component and Module classes, ensuring consistency between data model and ontology terms, extends the means to define and reference SubComponents, refines requirements on object URIs, enables graph-based serialization, moves Systems Biology Ontology (SBO) for Component types, makes all sequence associations explicit, makes interfaces explicit, generalizes SequenceConstraints into a general structural Constraint class, and expands the set of allowed constraints.
