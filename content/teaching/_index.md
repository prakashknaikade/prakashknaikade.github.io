---
title: Teaching
type: landing

cascade:
  - _target:
      kind: page
    params:
      show_breadcrumb: true

design:
  # Section spacing
  spacing: '1.5rem'
  
sections:
  - block: collection
    id: teaching-misc
    content:
      title: Research Papers I Read
      count: 0
      filters:
        folders:
          - teaching-papers
    design:
      view: article-grid
      fill_image: true
      columns: 2
  - block: collection
    id: teaching-project-ideas
    content:
      title: Research Project Ideas
      count: 0
      filters:
        folders:
          - teaching-project-ideas
    design:
      view: article-grid
      fill_image: true
      columns: 2
  
  
---
