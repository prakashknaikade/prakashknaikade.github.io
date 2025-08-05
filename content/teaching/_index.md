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
      text: This space contains summary of research papers I read.
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
      text: This space presents a collection of applied and research-driven project ideas.  
            If you find any of them interesting, I’d be happy to discuss opportunities for collaborative implementation.
      count: 0
      filters:
        folders:
          - teaching-project-ideas
    design:
      view: article-grid
      fill_image: true
      columns: 2
  
  
---
