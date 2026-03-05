---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-01-05
type: landing

design:
  # Default section spacing
  spacing: '0'

sections:
  # Developer Hero - Gradient background with name, role, social, and CTAs
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Hello, I'm"
      show_status: false
      show_scroll_indicator: false
      typewriter:
        enable: true
        prefix: "I build"
        strings:
          - "deep learning models"
          - "satellite image analysis"
          - "end-to-end ML pipelines"
          - "research-grade AI systems"
        type_speed: 70
        delete_speed: 40
        pause_time: 2500
      cta_buttons:
        - text: Get In Touch
          url: "#contact"
          icon: envelope
        - text: Skills
          url: "#skills"
          icon: arrow-down
    design:
      style: split
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["2rem", "0", "2rem", "0"]

  # Experience Timeline
  - block: resume-experience
    id: experience
    content:
      username: me
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Education Timeline
  - block: resume-experience
    id: education
    content:
      username: me-edu
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Filterable Portfolio - Alpine.js powered project filtering
  - block: portfolio
    id: projects
    content:
      title: "Featured Projects"
      subtitle: "A selection of my research and engineering work"
      count: 0
      filters:
        folders:
          - projects
      buttons:
        - name: All
          tag: '*'
        - name: Research
          tag: Research
        - name: Geospatial
          tag: Geospatial
        - name: NLP
          tag: NLP
      default_button_index: 0
    design:
      columns: 3
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Visual Tech Stack - Icons organized by category
  - block: tech-stack
    id: skills
    content:
      title: "Tech Stack"
      subtitle: "Tools and technologies I work with"
      categories:
        - name: AI / ML
          items:
            - name: PyTorch
              icon: devicon/pytorch
            - name: TensorFlow
              icon: devicon/tensorflow
            - name: OpenCV
              icon: devicon/opencv
            - name: Jupyter
              icon: devicon/jupyter
        - name: Data & Scientific
          items:
            - name: Python
              icon: devicon/python
            - name: NumPy
              icon: devicon/numpy
            - name: Pandas
              icon: devicon/pandas
            - name: CUDA
              icon: devicon/cuda
        - name: Geospatial
          items:
            - name: GDAL
              icon: devicon/gdal
            - name: QGIS
              icon: custom/qgis
            - name: Rasterio
              icon: custom/rasterio
            - name: GeoPandas
              icon: custom/geopandas
        - name: Engineering
          items:
            - name: Git
              icon: devicon/git
            - name: Docker
              icon: devicon/docker
            - name: GitHub Actions
              icon: brands/github
            - name: Linux
              icon: devicon/linux
    design:
      style: grid
      show_levels: false
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Contact Section
  - block: contact-info
    id: contact
    content:
      title: Get In Touch
      subtitle: "Open to research collaborations and engineering opportunities"
      text: |-
        I'm always interested in hearing about new research projects, engineering challenges, and opportunities.
        Whether you want to collaborate, discuss ideas, or just say hi — feel free to reach out!
      email: thomas.olive@aol.com
      autolink: true
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "6rem", "0"]
---
