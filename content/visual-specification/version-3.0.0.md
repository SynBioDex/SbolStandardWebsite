---
title: SBOL Visual Version 3.0.0
date: '2021-04-14'

# Variables in the data specification template
version: 3.0.0
specification: /docs/SBOL-Visual-3.0.pdf
citation: https://www.degruyter.com/document/doi/10.1515/jib-2021-0013/html

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
    - /specifications/sbol-visual/version-3.0.0

links:
- icon: file-pdf
  icon_pack: fas
  name: Specification
  url: /docs/SBOL-Visual-3.0.pdf
- icon: pen-fancy
  # icon: keyboard
  icon_pack: fas
  name: Cite
  url: https://www.degruyter.com/document/doi/10.1515/jib-2021-0013/html
- icon: passport
  icon_pack: fas
  name: Identifier
  url: http://identifiers.org/combine.specifications/sbol-visual.version-3.0.0

---

The major difference between SBOL Visual 3 and SBOL Visual 2 is that
diagrams and glyphs are defined with respect to the SBOL 3 data model
rather than the SBOL 2 data model.

A byproduct of this change is that the use of dashed undirected lines
for subsystem mappings has been removed. Until a decision is made
about how to represent constraints, the specification is mute on both
constraints and dashed undirected lines, which means that it is
acceptable to use them, if desired, as an annotation indicating
identity.

In addition, collection of glyphs has been modified as follows:

* The deprecated Insulator glyph and “shmoo” Macromolecule alternative
  glyph have been removed.
* Deprecated BioPAX alternatives to SBO terms for molecular species
  glyphs have been removed.

The changes for this release were approved as SEP V024.
