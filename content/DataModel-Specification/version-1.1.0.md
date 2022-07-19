---
title: SBOL Data Model Version 1.1.0
date: '2012-03-12'

# Variables in the data specification template
version: 1.1.0
specification: /docs/BBFRFC87.pdf
citation: https://www.nature.com/articles/nbt.2891

# View.
#   1 = List
#   2 = Compact
#   3 = Card
#   4 = Citation
view: 3

# Optional header image (relative to `static/img/` folder).
header:
  caption: ""
  image: ""

# Provide an alias for identifiers.org (See GitHub #195)
aliases:
    - /specifications/sbol/version-1.1.0

links:
- icon: file-pdf
  icon_pack: fas
  name: Specification
  url: /docs/BBFRFC87.pdf
- icon: pen-fancy
  # icon: keyboard
  icon_pack: fas
  name: Cite
  url: https://www.nature.com/articles/nbt.2891
- icon: passport
  icon_pack: fas
  name: Identifier
  url: http://identifiers.org/combine.specifications/sbol.version-1.1.0

---

Version 1.1.0 of the SBOL core data model is limited to the
description of discrete segments of DNA, called DNA components. To
remove ambiguity when specifying the design of synthetic DNA, the
information about DNA components is structured. DNA components
described using the SBOL core data model may have an associated DNA
sequence, or may be left as abstract descriptions. This flexibility
allows for the description of DNA component designs which have not yet
been realized, as well as those which are specific implementations of
that design.
