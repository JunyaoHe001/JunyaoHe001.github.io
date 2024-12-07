---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "4rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within content/authors/)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      # button:
      #   text: Download CV
      #   url: uploads/resume.pdf
    design:
      # css_class: dark
      css_style: "color: #ffffff; background-color: transparent;"
      background:
        color: black
        image:
          # Add your image background to assets/media/.
          filename: background2024.jpg
          filters:
            brightness: 0.0
          size: cover
          position: center
          parallax: false

  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        - **Urban Planning**  
          I am a doctoral researcher at Utrecht University, specializing in urban planning and social network analysis. My research focuses on understanding power dynamics and stakeholder collaboration in urban planning processes, with a strong emphasis on leveraging digital tools.
        - **Analytical Methods**  
          I apply both qualitative and quantitative methods, such as social network analysis and geospatial modeling, to explore how emerging technologies influence urban planning and public participation.
        - **Collaborations**  
          Please feel free to reach out for collaborations or discussions on planning, data analysis, or urban innovation! 😊
    design:
      css_class: my-research-container

  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 4


  - block: collection
    id: papers
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
      citation_style: APA
      css_class: 'custom-block' # 调用自定义CSS
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
    
  - block: collection
    id: talks
    content:
      title: Lecture & Talks
      filters:
        folders:
          - event
        count: 8
    design:
      view: article-grid
      columns: 4
    
  - block: collection
    id: news
    content:
      title: Recent News
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
        padding: [0, 0, 0, 0]
---
