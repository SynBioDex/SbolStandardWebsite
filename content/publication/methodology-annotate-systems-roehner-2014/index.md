---
title: "A Methodology to Annotate Systems Biology Markup Language Models with the Synthetic Biology Open Language"
date: 2014-02-01
publishDate: 2022-01-12T03:23:30.445219Z
authors: ["Nicholas Roehner", "Chris J. Myers"]
publication_types: ["2"]
abstract: "Recently, we have begun to witness the potential of synthetic biology, noted here in the form of bacteria and yeast that have been genetically engineered to produce biofuels, manufacture drug precursors, and even invade tumor cells. The success of these projects, however, has often failed in translation and application to new projects, a problem exacerbated by a lack of engineering standards that combine descriptions of the structure and function of DNA. To address this need, this paper describes a methodology to connect the systems biology markup language (SBML) to the synthetic biology open language (SBOL), existing standards that describe biochemical models and DNA components, respectively. Our methodology involves first annotating SBML model elements such as species and reactions with SBOL DNA components. A graph is then constructed from the model, with vertices corresponding to elements within the model and edges corresponding to the cause-and-effect relationships between these elements. Lastly, the graph is traversed to assemble the annotating DNA components into a composite DNA component, which is used to annotate the model itself and can be referenced by other composite models and DNA components. In this way, our methodology can be used to build up a hierarchical library of models annotated with DNA components. Such a library is a useful input to any future genetic technology mapping algorithm that would automate the process of composing DNA components to satisfy a behavioral specification. Our methodology for SBML-to-SBOL annotation is implemented in the latest version of our genetic design automation (GDA) software tool, iBioSim."
featured: false
publication: "*ACS Synthetic Biology*"
doi: "10.1021/sb400066m"
---

