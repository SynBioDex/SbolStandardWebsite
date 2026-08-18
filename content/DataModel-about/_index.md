---
title: SBOL Data Model

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

subtitle: "The data model for representing and exchanging genetic designs between software tools, with libraries in Python, Java, Rust, JavaScript and C++."
url: /datamodel/
aliases:
  - /datamodel-about/
layout: sbol-page
subnav: datamodel
toc: true
hero_buttons:
  - text: Read the specification
    url: /datamodel-specification/
  - text: Get a library
    url: /libraries/
    style: secondary
summary: "The data model for representing and exchanging genetic designs between software tools, with libraries in Python, Java, Rust, JavaScript and C++."
---

### Purpose

Synthetic biology builds upon the techniques and successes of genetics, molecular biology, and metabolic engineering by applying engineering principles to the design of biological systems. These principles include standardization, modularity, and design abstraction. The field still faces substantial challenges, including long development times, high rates of failure, and poor reproducibility. A common factor of these challenges is the exchange of information about designed systems between laboratories.

The Synthetic Biology Open Language (SBOL) has been developed as a standard to support the specification and exchange of biological design information in synthetic biology. For a quick introduction to SBOL, please browse through [IWBDA 2019 SBOL Workshop presentation](https://github.com/SynBioDex/Community-Media/blob/master/2019/IWBDA19/IWBDA2019.pdf) and [SEED 2018 SBOL presentation](https://github.com/SynBioDex/Community-Media/blob/master/2018/SEED/Workshop-Introduction.pptx).

### Vision

The SBOL data standard is a data exchange representation for synthetic biology designs. Its goal is to improve the efficiency of data exchange and reproducibility of synthetic biology research. SBOL introduces a standardized format for the electronic exchange of information on the structural and functional aspects of biological designs. The standard has been designed to support the explicit and unambiguous description of biological designs by means of a well defined data model. The standard further describes the rules and best practices on how to use this data model and populate it with relevant design details. SBOL uses existing Semantic Web practices and resources, such as Uniform Resource Identifiers (URIs) and ontologies, to unambiguously identify and define genetic design elements. The definition of the data model and associated format, the rules on the addition of data within the format and the representation of this in electronic data files are intended to make the SBOL standard a useful means of promoting global data exchange between laboratories and between software programs.

### Usage

SBOL Data is used as a data exchange format to represent genetic designs and its functional interaction.
This will allow information to be exchanged between software tools, maintain the integrity of the data, and ensure reproducibility of designs.
To get an idea on how the data model has been used in software tools, browse the [applications that support SBOL]({{< relref "applications" >}}).
The [publications list]({{< relref "publication" >}}) collects the papers that define the data model, feature it, or describe tools that support it.

### Libraries

Official libraries implement the data model in **Python**, **Java**, **Rust**, **JavaScript**, and **C/C++**; pick one on the [libraries page]({{< relref "libraries" >}}).

### Proposing a New Feature to the SBOL Data Model

To propose a new feature to SBOL, a standard procedure must be followed.

1. Submit a [new issue](https://github.com/SynBioDex/SBOL-specification/issues) on the SBOL Github repository.
2. Create a SBOL Enhancement Proposal (SEP)
    * Read [what an SEP is and how to submit one](https://github.com/SynBioDex/SEPs/issues/1).
    * Start from the [SEP template](https://raw.githubusercontent.com/SynBioDex/SEPs/master/sep_002_template.md).
    * For further assistance, please contact the [SBOL Editors](mailto:sbol-editors@googlegroups.com).
3. The community will discuss on the proposed SEP through the GitHub issue created for the corresponding SEP.
4. When the community has reached a consensus for the proposed SEP, voting will then be initiated to determine if the SEP will get accepted into the new release of SBOL.
