+++
# A Projects section created with the Portfolio widget.
widget = "blank"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = false  # Activate this widget? true/false
weight = 40  # Order that this section will appear.

title = "Latest SBOL Specifications"
subtitle = ""

[content]
  # Page type to display. E.g. project.
  page_type = "about"

  # Filter toolbar (optional).
  # Add or remove as many filters (`[[content.filter_button]]` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove toolbar, delete/comment all instances of `[[content.filter_button]]` below.
  
  # Default filter index (e.g. 0 corresponds to the first `[[filter_button]]` instance below).
  filter_default = 0

[design]

  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "2"

  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact
  #   3 = Card
  #   5 = Showcase
  view = 5

  # For Showcase view, flip alternate rows?
  flip_alt_rows = false

[design.background]
  # Apply a background color, gradient, or image.
  #   Uncomment (by removing `#`) an option to apply it.
  #   Choose a light or dark text color by setting `text_color_light`.
  #   Any HTML color name or Hex value is valid.
  
  # Background color.
  # color = "navy"
  
  # Background gradient.
  # gradient_start = "DeepSkyBlue"
  # gradient_end = "SkyBlue"
  
  # Background image.
  # image = "background.jpg"  # Name of image in `static/img/`.
  # image_darken = 0.6  # Darken the image? Range 0-1 where 0 is transparent and 1 is opaque.

  # Text color (true=light or false=dark).
  # text_color_light = true  
  
[advanced]
 # Custom CSS. 
 css_style = ""
 
 # CSS class.
 css_class = ""

# Commenting this section out. This can be used if we want a shorter description. 
# The Synthetic Biology Open Language (SBOL) has been developed as a standard to support the specification and exchange of biological design information in synthetic biology, following an open community process involving both wet bench scientists and dry scientific modelers and software developers, across academia, industry, and other institutions.

+++

SBOL has a come a long way! As our community has grown, so has our specification and data model! Here are the quick links to the latest specifications: 
* SBOL - [Version 3.0.1](/docs/SBOL3.0.1.pdf)
* SBOL Visual - [Version 3.0.0](/docs/SBOL-Visual-3.0.pdf)

{{< figure library="true" src="sbol3_evolution.svg" title="" lightbox="false" >}}
