---
title: SBOL Visual

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

subtitle: "The visual language for genetic design diagrams: standard glyphs, defined semantics and best practices that tools and journals share."
url: /visual/
aliases:
  - /visual-about/
layout: sbol-page
subnav: visual
toc: true
hero_buttons:
  - text: Read the specification
    url: /visual-specification/
  - text: Browse the glyphs
    url: /visual-glyphs/
    style: secondary
summary: "The visual language for genetic design diagrams: standard glyphs, defined semantics and best practices that tools and journals share."
---

{{< figure width="320px" library="true" src="Logos/SBOLVisualLogo.svg" title="" lightbox="true" >}}

### Purpose

People who are engineering biological organisms often find it useful to communicate in diagrams, both about the structure of the nucleic acid sequences that they are engineering and about the functional relationships between sequence features and other molecular species. Some typical practices and conventions have begun to emerge for such diagrams. SBOL Visual aims to organize and systematize such conventions in order to produce a coherent language for expressing the structure and function of genetic designs. At the same time, we aim to make this language simple and easy to use, allowing a high degree of flexibility and freedom in how such diagrams are organized, presented, and styled—in particular, it should be readily possible to create diagrams both by hand and with a wide variety of software programs. Finally, means are provided for extending the language with new and custom diagram elements, and for adoption of useful new elements into the language. For a quick introduction to SBOL Visual, please browse through the [IWBDA 2019 SBOL Visual presentation](https://github.com/SynBioDex/Community-Media/blob/master/2019/IWBDA19/SBOL-Visual.pptx).

### Vision

In order to ground SBOL Visual with precise definitions, we reference its visual elements to data models with a well-defined semantics. SBOL Visual glyphs are defined in terms of their relation to the SBOL 2 data model, and terms in the Sequence Ontology, the Systems Biology Ontology, and BioPAX.

### Usage

SBOL Visual acts as a guideline to graphically depict genetic designs and its functional interaction.
The [glyph library]({{< relref "visual-glyphs" >}}) is the quickest introduction.  

To see how tools use these glyphs, browse the [applications that support SBOL Visual]({{< relref "applications" >}}).  

The [publications list]({{< relref "publication" >}}) collects the papers that define SBOL Visual, feature it, or describe tools that support it.

### Download Glyphs

Glyphs are available as PNG, SVG, and PDF; download them from the [glyph library]({{< relref "visual-glyphs" >}}).

If you plan on creating your own glyphs, we recommend following the guidelines in the [SBOL Visual Specification]({{< relref "visual-specification" >}}) to ensure they will work well as part of an SBOL Visual diagram.

### Proposing a New Feature to SBOL Visual

To propose a new feature to SBOL visual, a standard procedure must be followed.

1. Submit a [new issue](https://github.com/SynBioDex/SBOL-visual/issues) on the SBOL-visual Github repository.
2. Create a SBOL Enhancement Proposal (SEP)
    * Read [what an SEP is and how to submit one](https://github.com/SynBioDex/SEPs/issues/1).
    * Start from the [SEP template](https://raw.githubusercontent.com/SynBioDex/SEPs/master/sep_002_template.md).
    * For further assistance, please contact the [SBOL Editors](mailto:sbol-editors@googlegroups.com).
3. The community will discuss on the proposed SEP through the GitHub issue created for the corresponding SEP.
4. When the community has reached a consensus for the proposed SEP, voting will then be initiated to determine if the SEP will get accepted into the new release of SBOL Visual.
