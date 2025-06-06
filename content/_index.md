---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "2rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I was junior researcher at August-Wilhelm Scheer Institute. I worked on my master thesis at Max Planck Institute for Informatics.

        My research interests span in the broad areas of Neural Rendering, Radiance Field Methods, Novel View Synthesis, Motion Capture, 3D-Reconstruction, Scene Understanding, Scene Interaction, Digital Twins, AR/VR, GenAI, LLMs, and generally Computer Vision, Computer Graphics, HCI, Deep/Machine Learning & Data Science, to solve the real world problems with impactful AI aided solutions.
        
        Please reach out to collaborate 😃
    design:
      columns: '2'
  # - block: collection
  #   id: papers
  #   content:
  #     title: 📌 Featured Publications
  #     filters:
  #       folders:
  #         - publications
  #       featured_only: false
  #   design:
  #     view: article-grid
  #     columns: 2
  - block: collection
    id: papers
    content:
      title: 📜 Publications
      text: ""
      filters:
        folders:
          - publications
    design:
      view: article-cite-grid
  - block: collection
    id: news
    content:
      title: 📰 Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: ""
  - block: markdown
    id: ama
    content:
      title: '💬 Ask Me Anything'
      subtitle: ''
      text:
        Want to Learn More About Me - Type your questions below!

        <script
        type="module"
        src="https://gradio.s3-us-west-2.amazonaws.com/5.0.1/gradio.js">
        </script>

        <gradio-app 
        src="https://prakashknaikade-ask-about-me.hf.space" 
        initial_height = "0px"
        info = "false"
        container = "false"
        eager="false"> 
        </gradio-app>

---
