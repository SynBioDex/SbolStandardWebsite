---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: An End-to-End Workflow for Engineering of Biological Networks from High-Level
  Specifications
subtitle: ''
summary: ''
authors:
- Jacob Beal
- Ron Weiss
- Douglas Densmore
- Aaron Adler
- Evan Appleton
- Jonathan Babb
- Swapnil Bhatia
- Noah Davidsohn
- Traci Haddock
- Joseph Loyall
- Richard Schantz
- Viktor Vasilev
- Fusun Yaman
tags: []
categories: []
date: '2012-08-17'
lastmod: 2020-09-19T21:28:24+01:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2020-09-19T20:28:24.887005Z'
publication_types:
- 2
abstract: 'We present a workflow for the design and production of biological networks
  from high-level program specifications. The workflow is based on a sequence of intermediate
  models that incrementally translate high-level specifications into DNA samples that
  implement them. We identify algorithms for translating between adjacent models and
  implement them as a set of software tools, organized into a four-stage toolchain:
  Specification, Compilation, Part Assignment, and Assembly. The specification stage
  begins with a Boolean logic computation specified in the Proto programming language.
  The compilation stage uses a library of network motifs and cellular platforms, also
  specified in Proto, to transform the program into an optimized Abstract Genetic
  Regulatory Network (AGRN) that implements the programmed behavior. The part assignment
  stage assigns DNA parts to the AGRN, drawing the parts from a database for the target
  cellular platform, to create a DNA sequence implementing the AGRN. Finally, the
  assembly stage computes an optimized assembly plan to create the DNA sequence from
  available part samples, yielding a protocol for producing a sample of engineered
  plasmids with robotics assistance. Our workflow is the first to automate the production
  of biological networks from a high-level program specification. Furthermore, the
  workflow’s modular design allows the same program to be realized on different cellular
  platforms simply by swapping workflow configurations. We validated our workflow
  by specifying a small-molecule sensor-reporter program and verifying the resulting
  plasmids in both HEK 293 mammalian cells and in E. coli bacterial cells.'
publication: ''
url_pdf: https://doi.org/10.1021/sb300030d
doi: 10.1021/sb300030d
---
