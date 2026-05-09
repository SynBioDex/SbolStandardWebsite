+++
# A Projects section created with the Portfolio widget.
widget = "portfolio"
headless = true
active = false  # Accessible via Tools & Resources nav — re-enable to show on homepage
weight = 140

title = "SBOL Tools & Applications"
subtitle = ""

[content]
  page_type = "applications"
  filter_default = 0

  [[content.filter_button]]
    name = "All"
    tag = "*"

  [[content.filter_button]]
    name = "Design"
    tag = "Design"

  [[content.filter_button]]
    name = "Visualization"
    tag = "Visualization"

  [[content.filter_button]]
    name = "Repositories"
    tag = "Repositories"

  [[content.filter_button]]
    name = "Analysis & Modeling"
    tag = "Analysis & Modeling"

  [[content.filter_button]]
    name = "Conversion & Validation"
    tag = "Conversion & Validation"

[design]
  columns = "2"
  view = 3
  flip_alt_rows = false

[design.background]
  color = ""

[advanced]
  css_style = ""
  css_class = ""
+++

SBOL-compatible tools cover the full synthetic biology workflow — from sequence and circuit design to simulation, visualization, and data repositories.

If you would like to feature your application here, please fill out this [survey](https://docs.google.com/forms/d/e/1FAIpQLScOTJLCoTniVPrMh88eg74Eaubh1bFMjncbyG6yt8q4cFLQ-Q/viewform).
