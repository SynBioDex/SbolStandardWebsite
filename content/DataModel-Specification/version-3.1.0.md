---
title: SBOL Data Model Version 3.1.0
date: '2022-10-26'

# Variables in the data specification template
version: 3.1.0
specification: /docs/SBOL3.1.0.pdf
citation: https://www.degruyter.com/document/doi/10.1515/jib-2022-0058/html


# Provide an alias for identifiers.org (See GitHub #195)
aliases:
    - /specifications/sbol/version-3.1.0

links:
- icon: file-pdf
  icon_pack: fas
  name: Specification
  url: docs/SBOL3.1.0.pdf
- icon: pen-fancy
  # icon: keyboard
  icon_pack: fas
  name: Cite
  url: https://www.degruyter.com/document/doi/10.1515/jib-2022-0058/html
- icon: passport
  icon_pack: fas
  name: Identifier
  url: http://identifiers.org/combine.specifications/sbol.version-3.1.0
---

SBOL Version 3.1.0 improves on version 3.0.0 by including a number of
corrections and clarifications as well as several other updates and
enhancements. First, this version includes a complete set of
validation rules for checking whether documents are valid SBOL
3. Second, the best practices section has been moved to an online
repository that allows for more rapid and interactive of sharing these
conventions. Third, it includes updates based upon six community
approved enhancement proposals. Two enhancement proposals are related
to the representation of an object's namespace. In particular, the
Namespace class has been removed and replaced with a namespace
property on each class. Another enhancement is the generalization of
the CombinatorialDeriviation class to allow direct use of Features and
Measures. Next, the Participation class now allow Interactions to be
participants to describe higher-order interactions. Another change is
the use of Sequence Ontology}terms for Feature orientation. Finally,
this version of SBOL has generalized from using Unique Reference
Identifiers (URIs) to Internationalized Resource Identifiers (IRIs) to
support international character sets.

Version 3.1.0 of SBOL was published on October 26, 2022
