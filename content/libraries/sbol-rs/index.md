---
title: Rust
summary: A typed Rust SDK and command-line toolkit for SBOL 2, SBOL 3, validation, and version conversion.
tags:
- Libraries
- Rust
sbol_versions: ["2", "3"]
lib_category: primary
date: "2026-07-29T00:00:00Z"

external_link: ""

image:
  focal_point: Smart

links:
- icon: github
  icon_pack: fab
  name: Github
  url: https://github.com/SynBioDex/sbol-rs
- icon: book-open
  icon_pack: fas
  name: API & Documentation
  url: https://docs.rs/sbol
- icon: tools
  icon_pack: fas
  name: Installation
  url: https://github.com/SynBioDex/sbol-rs#installation
- icon: code
  icon_pack: fas
  name: Crates.io
  url: https://crates.io/crates/sbol
- icon: terminal
  icon_pack: fas
  name: CLI Guide
  url: https://github.com/SynBioDex/sbol-rs/blob/master/crates/sbol-cli/README.md
- icon: exchange-alt
  icon_pack: fas
  name: Conversion Guide
  url: https://github.com/SynBioDex/sbol-rs/blob/master/docs/conversion.md
- icon: bug
  icon_pack: fas
  name: Bug & Feature Report
  url: https://github.com/SynBioDex/sbol-rs/issues

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""
slides: ""
---

[sbol-rs](https://github.com/SynBioDex/sbol-rs) is a Rust implementation of the Synthetic Biology Open Language covering both SBOL 2.3.0 and SBOL 3.1.0. It provides typed data models, RDF I/O, validation, and conversion between SBOL 2 and SBOL 3. The project supports RDF/XML, Turtle, JSON-LD, and N-Triples, and includes GenBank and FASTA import into SBOL 3.

Most Rust applications can use the umbrella `sbol` crate for both SBOL versions:

```sh
cargo add sbol
```

The separate `sbol-cli` crate installs an `sbol` command for validating, comparing, converting, upgrading, downgrading, and importing documents:

```sh
cargo install sbol-cli
sbol validate design.ttl
```

Start with the [crate guide](https://github.com/SynBioDex/sbol-rs/blob/master/docs/crate-guide.md) for the SDK architecture and document lifecycle. The repository also provides detailed guides to [validation](https://github.com/SynBioDex/sbol-rs/blob/master/docs/validation.md), [RDF I/O](https://github.com/SynBioDex/sbol-rs/blob/master/docs/rdf-io.md), and [SBOL 2–3 conversion](https://github.com/SynBioDex/sbol-rs/blob/master/docs/conversion.md).

sbol-rs is freely available under the MIT or Apache 2.0 license.
