---
title: iBioSim
summary: iBioSim has been developed for the modeling, analysis, and design of genetic circuits.
tags: ["Circuit Design", "Modeling", "Visualization", "SBOL Visual", "SBOL1 Import", "SBOL1 Export", "SBOL2 Import", "SBOL2 Export"]
date: "2020-06-30T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  # caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
- icon: edge
  icon_pack: fab
  name: Link
  url: https://async.ece.utah.edu/tools/ibiosim/
- icon: github
  icon_pack: fab
  name: Source Code
  url: https://github.com/MyersResearchGroup/iBioSim

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

iBioSim has been developed for the modeling, analysis, and design of genetic circuits. While iBioSim primarily targets models of genetic circuits, models representing metabolic networks, cell-signaling pathways, and other biological and chemical systems can also be analyzed. iBioSim also includes modeling and visualization support for multi-cellular and spatial models as well. It is capable of importing and exporting models specified using the Systems Biology Markup Language (SBML). It can import all levels and versions of SBML and is able to export Level 3 Version 1. It supports all core SBML modeling constructs except some types of fast reactions, and also has support for the hierarchical model composition, layout, flux balance constraints, and arrays packages. It was the first tool to produce correct results for all examples in the SBML benchmark suite. It has also been tested successfully on the stochastic benchmark suite and the curated models in the BioModels database. Finally, it is one of the first tools to also support the Synthetic Biology Open Language (SBOL), an emerging standard for information exchange in synthetic biology.

{{< youtube g4xayzlyC2Q >}}


| | |
| ---| ---|
| Contact Person | Chris Myers |
| Organization(s) | University of Utah |
| Programming Language | Java/C++ |
| OS/Platform | Linux, Mac, Windows |
| Availability | Open-Source |
| License | MIT |