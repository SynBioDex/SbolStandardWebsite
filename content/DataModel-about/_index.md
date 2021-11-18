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
    - /datamodel/
---

{{< figure width="600px" library="true" src="Logos/SBOLlogo.svg" title="" lightbox="true" >}}

### Purpose

Synthetic biology builds upon the techniques and successes of genetics, molecular biology, and metabolic engineering by applying engineering principles to the design of biological systems. These principles include standardization, modularity, and design abstraction. The field still faces substantial challenges, including long development times, high rates of failure, and poor reproducibility. A common factor of these challenges is the exchange of information about designed systems between laboratories.

The Synthetic Biology Open Language (SBOL) has been developed as a standard to support the specification and exchange of biological design information in synthetic biology. For a quick introduction to SBOL, please browse through [IWBDA 2019 SBOL Workshop presentation](https://github.com/SynBioDex/Community-Media/blob/master/2019/IWBDA19/IWBDA2019.pdf) and [SEED 2018 SBOL presentation](https://github.com/SynBioDex/Community-Media/blob/master/2018/SEED/Workshop-Introduction.pptx).

### Vision

The SBOL data standard is a data exchange representation for synthetic biology designs. Its goal is to improve the efficiency of data exchange and reproducibility of synthetic biology research. SBOL introduces a standardized format for the electronic exchange of information on the structural and functional aspects of biological designs. The standard has been designed to support the explicit and unambiguous description of biological designs by means of a well defined data model. The standard further describes the rules and best practices on how to use this data model and populate it with relevant design details. SBOL uses existing Semantic Web practices and resources, such as Uniform Resource Identifiers (URIs) and ontologies, to unambiguously identify and define genetic design elements. The definition of the data model and associated format, the rules on the addition of data within the format and the representation of this in electronic data files are intended to make the SBOL standard a useful means of promoting global data exchange between laboratories and between software programs.

### Usage

SBOL Data is used as a data exchange format to represent genetic designs and its functional interaction.
This will allow information to be exchanged between software tools, maintain the integrity of the data, and ensure reproducibility of designs.
To get an idea on how the data model has been used in software tools, view all of the [SBOL Data model tools]({{< relref "applications" >}}) that have been reported to us.
Also take a look at sample papers that have been published online for the SBOL data model, featuring the SBOL data model, and software tools supporting the SBOL data model [here]({{< relref "publication" >}}).

### Download SBOL Data Library

We support the SBOL Data models in the following formats: **C/C++**, **Java**, **Javascript**, and **Python**. You can download the SBOL data model [here]({{< relref "libraries" >}}).

### Proposing a New Feature to the SBOL Data Model

To propose a new feature to SBOL visual, a standard procedure must be followed.

1. Submit a [new issue](https://github.com/SynBioDex/SBOL-specification/issues) on the SBOL-visual Github repository.
2. Create a SBOL Enhancement Proposal (SEP)
    * A detailed description about what is an SEP, how to create an SEP, and how to submit an SEP can be found [here](https://github.com/SynBioDex/SEPs/issues/1).
    * A template of what a general SEP should look like can be found [here](https://raw.githubusercontent.com/SynBioDex/SEPs/master/sep_002_template.md).
    * For further assistance, please contact the [SBOL Editors](mailto:sbol-editors@googlegroups.com).
3. The community will discuss on the proposed SEP through the GitHub issue created for the corresponding SEP.
4. When the community has reached a consensus for the proposed SEP, voting will then be initiated to determine if the SEP will get accepted into the new release of SBOL Visual.
