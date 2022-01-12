---
title: "An End-to-End Workflow for Engineering of Biological Networks from High-Level Specifications"
date: 2012-08-01
publishDate: 2022-01-12T03:23:30.405216Z
authors: ["Jacob Beal", "Ron Weiss", "Douglas Densmore", "Aaron Adler", "Evan Appleton", "Jonathan Babb", "Swapnil Bhatia", "Noah Davidsohn", "Traci Haddock", "Joseph Loyall", "Richard Schantz", "Viktor Vasilev", "Fusun Yaman"]
publication_types: ["2"]
abstract: "We present a workflow for the design and production of biological networks from high-level program specifications. The workflow is based on a sequence of intermediate models that incrementally translate high-level specifications into DNA samples that implement them. We identify algorithms for translating between adjacent models and implement them as a set of software tools, organized into a four-stage toolchain: Specification, Compilation, Part Assignment, and Assembly. The specification stage begins with a Boolean logic computation specified in the Proto programming language. The compilation stage uses a library of network motifs and cellular platforms, also specified in Proto, to transform the program into an optimized Abstract Genetic Regulatory Network (AGRN) that implements the programmed behavior. The part assignment stage assigns DNA parts to the AGRN, drawing the parts from a database for the target cellular platform, to create a DNA sequence implementing the AGRN. Finally, the assembly stage computes an optimized assembly plan to create the DNA sequence from available part samples, yielding a protocol for producing a sample of engineered plasmids with robotics assistance. Our workflow is the first to automate the production of biological networks from a high-level program specification. Furthermore, the workflow's modular design allows the same program to be realized on different cellular platforms simply by swapping workflow configurations. We validated our workflow by specifying a small-molecule sensor-reporter program and verifying the resulting plasmids in both HEK 293 mammalian cells and in E. coli bacterial cells."
featured: false
publication: "*ACS Synthetic Biology*"
doi: "10.1021/sb300030d"
---

