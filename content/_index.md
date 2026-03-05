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
      greeting: "Hi, I'm"
      show_status: true
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "I build"
        strings:
          - "geospatial deep learning models"
          - "satellite image analysis"
          - "end-to-end ML pipelines"
          - "research-grade AI systems"
        type_speed: 70
        delete_speed: 40
        pause_time: 2500
      cta_buttons:
        - text: View My Work
          url: "#projects"
          icon: arrow-down
        - text: Get In Touch
          url: "#contact"
          icon: envelope
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["6rem", "0", "4rem", "0"]

  # Experience Timeline
  - block: resume-experience
    id: experience
    content:
      title: Experience
      date_format: Jan 2006
      items:
        - title: R&D AI Engineer
          company: Diginove
          company_url: ''
          company_logo: ''
          location: Montpellier, France
          date_start: '2024-09-01'
          date_end: ''
          description: |2-
            * Design and deployment of deep learning models for satellite image processing
            * Conditional GAN (SENWISE project) for thermal super-resolution: Sentinel-3 × Landsat (1000 m → 30 m, SSIM ≈ 98.8%)
            * ESA-funded research; full ownership from architecture to production inference pipeline
            * Tech stack: PyTorch, GDAL, Rasterio, Python, Docker
        - title: Research Intern — Computer Vision & NLP
          company: Synchromedia Lab, ETS Montreal
          company_url: ''
          company_logo: ''
          location: Montreal, Canada
          date_start: '2024-01-01'
          date_end: '2024-08-31'
          description: |2-
            * Designed Attention–NMF model: CNN attention encoder + NMF decoder with linear independence constraint
            * Task: handwritten text extraction from ancient multispectral document images
            * Work submitted to ICASSP 2025
            * Tech stack: PyTorch, NumPy, Python
        - title: Automation Intern
          company: Bioderma / Naos Group
          company_url: ''
          company_logo: ''
          location: Lyon, France
          date_start: '2021-05-01'
          date_end: '2021-08-31'
          description: |2-
            * Automated quality-control reporting pipeline for production lines
            * Reduced manual reporting time significantly through scripted data aggregation
            * Tech stack: Python, Excel automation, PLC data interfaces
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
      title: Education
      date_format: Jan 2006
      items:
        - title: M.Sc. Electrical Engineering (Research Profile)
          company: École de Technologie Supérieure (ETS Montreal)
          company_url: ''
          company_logo: ''
          location: Montreal, Canada
          date_start: '2022-09-01'
          date_end: '2024-08-31'
          description: |2-
            * Specialisation in image processing, computer vision, and applied deep learning
            * Research thesis: multispectral document analysis using attention-based NMF
            * Coursework: Signal Processing, Machine Learning, Computer Vision, Optimization
        - title: Engineering Degree — Robotics & Computer Science
          company: ECAM Lyon
          company_url: ''
          company_logo: ''
          location: Lyon, France
          date_start: '2018-09-01'
          date_end: '2022-06-30'
          description: |2-
            * Generalist engineering curriculum with specialisation in robotics and IT
            * Final year focus: embedded systems, automation, signal processing
            * International exchange: ETS Montreal (2022–2024)
    design:
      columns: '1'
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
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
