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
        <div class="w-full">
          <div px-0 class="flex flex-col justify-center max-w-screen-xl mx-auto" style="width:1000px; margin-left:-5rem; text-align: ;">

          I completed my Master’s in Media Computer Science from the Faculty of Mathematics and Computer Science, Saarland University, Germany, where my focus was on multimedia, (3D) computer vision and machine learning. I worked on my master thesis at Max Planck Institute for Informatics. During my masters, I was junior researcher at August-Wilhelm Scheer Institute and also interned as computer vision engineer in BASF and Fenris GmbH. Before moving to Europe, I received my bachelor’s degree in Computer Engineering from the Pune University in India.
          
          My research interests span in the broad areas of 3D-Reconstruction, Neural Rendering, Radiance Field Methods, Novel View Synthesis, Motion Capture, Scene Understanding, Scene Interaction, LLMs, VLMs, Digital Twins, AR/VR, and generally (3D) Computer Vision, GenAI, XR, HCI, Data Science, and Deep/Machine Learning, to solve complex problems with impactful AI-driven solutions.
          
          Please reach out to collaborate 😃
          </div>

          <div style="display: flex; flex-wrap: nowrap; justify-content: center; align-items: center; gap: 2rem; margin-top: 1rem;">

          <img src="/uploads/logo_SPPU.png" style="height: 80px; object-fit: contain; transition: transform 0.3s;" onmouseover="this.style.transform='scale(6)'" onmouseout="this.style.transform='scale(1)'">
          <img src="/uploads/Logo_UDS.png" style="height: 60px; object-fit: contain; transition: transform 0.3s;" onmouseover="this.style.transform='scale(1.5)'" onmouseout="this.style.transform='scale(1)' ">
          <img src="/uploads/mpi_logo.svg" style="height: 60px; object-fit: contain; transition: transform 0.3s;" onmouseover="this.style.transform='scale(2)'" onmouseout="this.style.transform='scale(1)'">
          <img src="/uploads/Logo_AWSi.svg" style="height: 60px; object-fit: contain; transition: transform 0.3s;" onmouseover="this.style.transform='scale(2)'" onmouseout="this.style.transform='scale(1)'">
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
