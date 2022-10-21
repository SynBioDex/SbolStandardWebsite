---
title: SBOL Visual Version 2.2.0
date: '2020-03-15'

# Variables in the data specification template
version: 2.2.0
specification: /docs/SBOL-Visual-2.2.pdf
citation: https://www.degruyter.com/document/doi/10.1515/jib-2020-0014/html

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
    - /specifications/sbol-visual/version-2.2.0

links:
- icon: file-pdf
  icon_pack: fas
  name: Specification
  url: /docs/SBOL-Visual-2.2.pdf
- icon: pen-fancy
  # icon: keyboard
  icon_pack: fas
  name: Cite
  url: https://www.degruyter.com/document/doi/10.1515/jib-2020-0014/html
- icon: passport
  icon_pack: fas
  name: Identifier
  url: http://identifiers.org/combine.specifications/sbol-visual.version-2.2.0

---

SBOL Visual 2.2 provides a simple and flexible language for diagrams
of genetic systems and design, including both structure (e.g., nucleic
acid sequence features) and function (e.g., regulatory interactions
and reactions).

SBOL Visual 2.2 enhances the prior SBOL Visual 2.1 standard as
follows:

* Grounding for molecular species glyphs is changed from BioPAX to SBO
  (BioPAX terms are retained as deprecated alternatives).
* New glyphs are added for introns and polypeptide regions (e.g., protein domains).
* The macromolecule glyph often confused with yeast is deprecated, and a new glyph for proteins added
* Small polygons are recommended as alternative glyphs for simple chemicals.