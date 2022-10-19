---
title: SBOL Visual Version 2.3.0
date: '2020-12-04'

# Variables in the data specification template
version: 2.3.0
specification: /docs/SBOL-Visual-2.3.pdf
citation: http://www.degruyter.com/document/doi/10.1515/jib-2020-0045/html

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
    - /specifications/sbol-visual/version-2.3.0

links:
- icon: file-pdf
  icon_pack: fas
  name: Specification
  url: /docs/SBOL-Visual-2.3.pdf
- icon: pen-fancy
  # icon: keyboard
  icon_pack: fas
  name: Cite
  url: http://www.degruyter.com/document/doi/10.1515/jib-2020-0045/html
- icon: passport
  icon_pack: fas
  name: Identifier
  url: http://identifiers.org/combine.specifications/sbol-visual.version-2.3.0

---

SBOL Visual 2.3 provides a simple and flexible language for diagrams
of genetic systems and design, including both structure (e.g., nucleic
acid sequence features) and function (e.g., regulatory interactions
and reactions).

SBOL Visual 2.3 enhances the prior SBOL Visual 2.2 standard as follows:

* Adds higher-level "interactions with interactions", such as an
  inducer molecule stimulating a repression interaction
* Binding with a nucleic acid backbone can be shown by overlapping
  glyphs, as with other molecular complexes
* Recommends using polypeptide region glyph to show 2A sequences
* Adds new "unspecified interaction" glyph for visualizing
  interactions whose nature is unknown
* Deprecates "insulator" glyph in favor of new "inert DNA spacer" glyph
