# SBOL Visual Guidelines

## Compliance Guidelines

- **Features on Different Backbones**  
  Features MUST NOT be on the same backbone if they are not located on the same sequence.

- **Single-Stranded Backbone Representation**  
  Single-stranded regions of nucleic acid constructs MUST use a single line to indicate the backbone.

- **Feature Glyph Alignment**  
  The bounding box of a feature glyph MUST be in contact with the backbone.

- **Feature Glyph Role**  
  The glyph used for a feature MUST contain the role of the feature.

- **Molecular Species Glyph Type**  
  The glyph used for a molecular species MUST contain the type of the molecular species.

- **Molecular Species Glyph Position**  
  The bounding box of a molecular species MUST NOT contact a nucleic acid construct unless it interacts with it.

- **Interaction Crossover Pattern**  
  Interactions that intersect MUST use a crossover pattern that “diverts” to indicate the distinction between edges.

- **Interaction Glyph Type**  
  The glyph used for an interaction MUST contain the type of the interaction.

- **Multi-Head Edge Consistency**  
  An edge with multiple heads MUST use the same glyph for each head.

- **Interaction Node Glyph Type**  
  The glyph used for an interaction node MUST contain the type of the interaction.

- **Edge Connection Rule**  
  An edge MUST NOT connect to the head or tail of another edge.

- **Subsystem Boundary Respect**  
  Glyphs for sequence features and molecular species MUST NOT intersect the boundary of a subsystem.

- **Interface Rectangle Rule**  
  If an interface rectangle is used to indicate that a feature is part of the interface of a subsystem, then any interaction crossing the boundary and connecting with that feature MUST pass through the interface rectangle.

---

## Best Practices Guidelines

- **Double-Stranded Backbone Representation**  
  In a diagram with both single- and double-stranded nucleic acid constructs, double-stranded constructs SHOULD use double-lined backbones.

- **Horizontal Backbone Orientation**  
  Nucleic acid backbones SHOULD be horizontal unless using non-horizontal structure to indicate physical attributes (e.g., closed loop for cyclic plasmid or complex shapes showing secondary structure).

- **Plasmid and Locus Glyph Shapes**  
  Backbones SHOULD use the shape of plasmid and locus glyphs to indicate those features, and the omitted detail glyph to indicate context not shown.

- **Feature Presence on Backbones**  
  A nucleic acid backbone SHOULD have at least one feature glyph unless it is an assembly diagram.

- **Backbone Alignment**  
  Glyphs SHOULD follow the recommendation for backbone alignment in the glyph specification.

- **Reverse Complement Orientation**  
  Reverse complement SHOULD be consistently indicated by 180-degree rotation, not horizontal-only inversion.

- **Inline Orientation**  
  Inline 5’ to 3’ SHOULD be drawn left to right, and reverse complement right to left.

- **Feature Overlap Guidelines**  
  Nucleic acid features SHOULD NOT overlap unless their locations overlap (flexible on bounding box overlap if the glyph itself does not overlap).

- **Intended Feature Overlap**  
  Nucleic acid features SHOULD overlap if their locations overlap.

- **Specific Glyph Usage for Nucleic Acids**  
  A nucleic acid SHOULD use the RECOMMENDED version of the most specific applicable glyph. Novel, more-specific glyphs are acceptable.

- **Specific Glyph Usage for Molecular Species**  
  A molecular species SHOULD use the RECOMMENDED version of the most specific applicable glyph. Novel, more-specific glyphs are acceptable.

- **Overlap Representation for Molecular Species**  
  If a molecular species overlaps a nucleic acid construct, the location of the overlap SHOULD correspond with the location of the interaction; the molecular species glyph SHOULD be distinct from a sequence feature glyph, and the location SHOULD be represented with a feature glyph appropriate to the interaction.

- **Avoid Crossing Interaction Edges**  
  Two interaction edges SHOULD NOT cross one another.

- **Interaction Glyph Specificity**  
  An interaction SHOULD use the RECOMMENDED version of the most specific applicable glyph. Novel, more-specific glyphs are acceptable.

- **Interaction Node Glyph Specificity**  
  An interaction node SHOULD use the RECOMMENDED version of the most specific applicable glyph. Novel, more-specific glyphs are acceptable.

- **Multi-Head/Tail Edge Connection Rule**  
  An edge SHOULD NOT connect to only one head of a multi-head arrow or only one tail of a multi-tail arrow.

- **Subsystem Boundary Design**  
  The boundary of a subsystem SHOULD be a rectangle or rounded rectangle with sides oriented vertically and horizontally, and SHOULD be larger and have a different line style than other glyphs.

- **Object Name Association**  
  If an object’s name is displayed, it SHOULD be clearly visually connected to the object’s associated glyph.
