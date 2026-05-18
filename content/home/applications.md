+++
# A Projects section created with the Portfolio widget.
widget = "portfolio"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = false  # Activate this widget? true/false
weight = 140  # Order that this section will appear.

title = "SBOL Tools & Applications"
subtitle = ""

[content]
  # Page type to display. E.g. project.
  page_type = "applications"
  
  # Filter toolbar (optional).
  # Add or remove as many filters (`[[content.filter_button]]` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove toolbar, delete/comment all instances of `[[content.filter_button]]` below.
  
  # Default filter index (e.g. 0 corresponds to the first `[[filter_button]]` instance below).
  filter_default = 0
  
  [[content.filter_button]]
    name = "All"
    tag = "*"
 
  [[content.filter_button]]
    name = "SBOL1 Import"
    tag = "SBOL1 Import"
  
  [[content.filter_button]]
    name = "SBOL1 Export"
    tag = "SBOL1 Export"
  
  [[content.filter_button]]
    name = "SBOL2 Import"
    tag = "SBOL2 Import"
  
  [[content.filter_button]]
    name = "SBOL2 Export"
    tag = "SBOL2 Export"
  
  [[content.filter_button]]
    name = "Sequence Design"
    tag = "Sequence Design"
  
  [[content.filter_button]]
    name = "Circuit Design"
    tag = "Circuit Design"

  [[content.filter_button]]
    name = "Modeling"
    tag = "Modeling"

  [[content.filter_button]]
    name = "SBOL Visual"
    tag = "SBOL Visual"

  [[content.filter_button]]
    name = "Visualization"
    tag = "Visualization"
  
  [[content.filter_button]]
    name = "Knowledge Management"
    tag = "Knowledge Management"

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "2"

  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact
  #   3 = Card
  #   5 = Showcase
  view = 3

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
  # {{< figure width="600px" library="true" src="SBOL_2_demo_workflow_chris.png" title="" lightbox="true" >}}
[advanced]
 # Custom CSS. 
 css_style = ""
 
 # CSS class.
 css_class = ""
+++

If you are a synthetic biologist, you may not be aware that there are already many software tools available that support different aspects of the synthetic biology workflow, such as optimizing DNA assembly or simulating gene networks.  Each of the software tools listed here supports exchange of genetic designs in the SBOL file format (SBOL core) or supports display of genetic designs using standard SBOL Visual glyphs.

If you would like us to feature your application here, please fill out this [survey](https://docs.google.com/forms/d/e/1FAIpQLScOTJLCoTniVPrMh88eg74Eaubh1bFMjncbyG6yt8q4cFLQ-Q/viewform).