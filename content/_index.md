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
    design:
      # Optional: Control the width of the block content
      columns: '1'
      # Optional: Use custom CSS classes
      css_class: 'max-w-4xl mx-auto px-4'
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
          <div style="font-size: 1.1rem;">
          I completed my Master’s in Media Computer Science from the Faculty of Mathematics and Computer Science, Saarland University, Germany, where my focus was on (3D) computer vision, machine learning, HCI, and computational multimedia. I worked on my master thesis at Max Planck Institute for Informatics. During my masters, I was junior researcher at August-Wilhelm Scheer Institute and also interned as computer vision engineer in BASF and Fenris GmbH. Before moving to Europe, I received my bachelor’s degree in Computer Engineering from the Pune University in India.
          
          My research interests span in the broad areas of 3D-Reconstruction, Neural Rendering, Radiance Field Methods, Novel View Synthesis, Motion Capture, Scene Understanding, Scene Interaction, LLMs, VLMs, Digital Twins, AR/VR, and generally (3D) Computer Vision, GenAI, XR, HCI, Data Science, and Deep/Machine Learning, to solve complex problems with impactful AI-driven solutions.
          
          Please reach out to collaborate 😃
          </div>

          <div class="mt-4 flex flex-wrap justify-center items-center gap-4 md:gap-6">
            <div class="logo-container">
              <img src="/uploads/logo_SPPU.png" class="h-16 md:h-20 object-contain transition-transform duration-300 hover:scale-125" alt="Pune University">
            </div>
            <div class="logo-container">
              <img src="/uploads/Logo_UDS.png" class="h-12 md:h-16 object-contain transition-transform duration-300 hover:scale-125" alt="Saarland University">
            </div>
            <div class="logo-container">
              <img src="/uploads/mpi_logo.svg" class="h-12 md:h-16 object-contain transition-transform duration-300 hover:scale-125 md:hover:scale-150" alt="Max Planck Institute">
            </div>
            <div class="logo-container">
              <img src="/uploads/Logo_AWSi.svg" class="h-12 md:h-16 object-contain transition-transform duration-300 hover:scale-125 md:hover:scale-150" alt="August-Wilhelm Scheer Institute">
            </div>
          </div>

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
      text: 
        <div class="w-full">
        </div>
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
