---
title:

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

# Provide a short alias (See GitHub #135)
aliases:
    - /visual/
---

{{< figure width="600px" library="true" src="Logos/SBOLVisualLogo.svg" title="" lightbox="true" >}}

### Purpose

People who are engineering biological organisms often find it useful to communicate in diagrams, both about the structure of the nucleic acid sequences that they are engineering and about the functional relationships between sequence features and other molecular species. Some typical practices and conventions have begun to emerge for such diagrams. SBOL Visual aims to organize and systematize such conventions in order to produce a coherent language for expressing the structure and function of genetic designs. At the same time, we aim to make this language simple and easy to use, allowing a high degree of flexibility and freedom in how such diagrams are organized, presented, and styled—in particular, it should be readily possible to create diagrams both by hand and with a wide variety of software programs. Finally, means are provided for extending the language with new and custom diagram elements, and for adoption of useful new elements into the language. For a quick introduction to SBOL Visual, please browse through the [IWBDA 2019 SBOL Visual presentation](https://github.com/SynBioDex/Community-Media/blob/master/2019/IWBDA19/SBOL-Visual.pptx).

### Vision

In order to ground SBOL Visual with precise definitions, we reference its visual elements to data models with a well-defined semantics. SBOL Visual are defined in terms of their relation to the SBOL 2 data model, and terms in the Sequence Ontology, the Systems Biology Ontology, and BioPAX.

### Usage

SBOL Visual acts as a guideline to graphically depict genetic designs and its functional interaction.
A quick introduction can be found [here]({{< relref "visual-glyphs" >}}).  

To get an idea on how these glyphs has been used in software tools, view all of the [SBOL Visual tools]({{< relref "applications" >}}) that have been reported to us.  

Also take a look at sample papers that have been published online for SBOL visual, featuring SBOL visual, and software tools supporting SBOL visual [here]({{< relref "publication" >}}).

### Download Glyphs

We support SBOL Visual glyphs in the following formats: PNG, SVG, and PDF. You can download our copy of the glyphs [here]({{< relref "visual-glyphs" >}}).

If you plan on creating your own glyphs, we recommend following the guidelines in the [SBOL Visual Specification]({{< relref "visual-specification" >}}) to ensure they will work well as part of an SBOL Visual diagram.

### Proposing a New Feature to the SBOL Data Model

To propose a new feature to SBOL visual, a standard procedure must be followed.

1. Submit a [new issue](https://github.com/SynBioDex/SBOL-visual/issues) on the SBOL-visual Github repository.
2. Create a SBOL Enhancement Proposal (SEP)
    * A detailed description about what is an SEP, how to create an SEP, and how to submit an SEP can be found [here](https://github.com/SynBioDex/SEPs/issues/1).
    * A template of what a general SEP should look like can be found [here](https://raw.githubusercontent.com/SynBioDex/SEPs/master/sep_002_template.md).
    * For further assistance, please contact the [SBOL Editors](mailto:sbol-editors@googlegroups.com).
3. The community will discuss on the proposed SEP through the GitHub issue created for the corresponding SEP.
4. When the community has reached a consensus for the proposed SEP, voting will then be initiated to determine if the SEP will get accepted into the new release of SBOL Visual.
