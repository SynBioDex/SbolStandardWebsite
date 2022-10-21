---
title: SBOL Visual Version 2.1.0
date: '2018-11-30'

# Variables in the data specification template
version: 2.1.0
specification: /docs/SBOL-Visual-2.1.pdf
citation: https://www.degruyter.com/document/doi/10.1515/jib-2018-0101/html

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
    - /specifications/sbol-visual/version-2.1.0

links:
- icon: file-pdf
  icon_pack: fas
  name: Specification
  url: /docs/SBOL-Visual-2.1.pdf
- icon: pen-fancy
  # icon: keyboard
  icon_pack: fas
  name: Cite
  url: https://www.degruyter.com/document/doi/10.1515/jib-2018-0101/html
- icon: passport
  icon_pack: fas
  name: Identifier
  url: http://identifiers.org/combine.specifications/sbol-visual.version-2.1.0

---

SBOL Visual 2.1 provides a simple and flexible language for diagrams
of genetic systems and design, including both structure (e.g., nucleic
acid sequence features) and function (e.g., regulatory interactions
and reactions). SBOL Visual 2.1 enhances the prior SBOL Visual 2.0
standard with the addition of methods for showing modular structure
and mappings between elements of a system, and new glyphs for
indicating genomic context (e.g., integration into a plasmid or
genome) and for stop codons. Additionally, interactions arrows were
modified such that they can split or join, with the glyph at the split
or join indicating either superposition or a chemical process.
