---

# Projects Section

widget: portfolio

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 2

title: Projects
subtitle: ''

content:
  # Page type to display. E.g. project.
  page_type: project

  # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
  filter_default: 0

  # Filter toolbar (optional).
  # Add or remove as many filters (`filter_button` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove the toolbar, delete the entire `filter_button` block.
  filter_button:
  - name: All
    tag: '*'
  - name: Speckle Imaging
    tag: LSCI
  - name: Multiphoton Microscopy
    tag: Multiphoton Microscopy
  # - name: Computational Modeling
  #     tag: Computational Modeling

design:
  # Choose how many columns the section has. Valid values: '1' or '2'.
  columns: "2"

  view: masonry
  
---