---
title: 'Experience'
date: 2023-10-24
type: landing

design:
  spacing: '5rem'

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: resume-experience
    content:
      username: admin
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
  - block: resume-skills
    content:
      title: Technical Skills
      username: admin
    design:
      show_skill_percentage: true
  - block: resume-hobbies
    content:
      title: Hobbies
      items:
      - name: Hiking
        description: ''
        percent: 60
        icon: person-simple-walk
      - name: Cats
        description: ''
        percent: 100
        icon: cat
      - name: Photography
        description: ''
        percent: 80
        icon: camera
      username: admin
    design:
      show_skill_percentage: true
  - block: resume-awards
    content:
      title: Awards
      username: admin
  - block: resume-languages
    content:
      title: Languages
      username: admin
---
