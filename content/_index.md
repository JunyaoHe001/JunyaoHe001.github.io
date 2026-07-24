---
title: ""
date: 2022-10-24
type: landing

design:
  spacing: "4rem"

sections:
  - block: resume-biography-3
    content:
      username: admin
      text: ""
    design:
      css_style: "color: #ffffff; background-color: transparent;"
      background:
        color: black
        image:
          filename: background2024.jpg
          filters:
            brightness: 0.0
          size: cover
          position: center
          parallax: false

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

  - block: markdown
    content:
      title: 'My Research'
      subtitle: ''
      text: |-
        My research is organised around **complex networks and complex systems** as a shared analytical foundation. I study relational and spatial processes across four connected empirical fields:

        - **Urban planning and urban studies**, including digital participation, planning governance, and power relations.
        - **Urban and economic geography**, with particular attention to labour markets, regional restructuring, and spatial inequality.
        - **Mobility and migration**, including job–home networks, residential relocation, interregional migration, and digitally enabled mobility.
        - **Computational social science**, combining network analysis, spatial methods, simulation, text analysis, and interpretable machine learning.

        Current work examines how remote and hybrid work, digitalisation, and emerging technologies reshape urban systems, mobility patterns, and uneven regional development.
    design:
      css_class: my-research-container

  - block: collection
    id: papers
    content:
      title: Recent Publications & Conferences
      text: ""
      filters:
        folders:
          - publication
        count: 10
        exclude_featured: false
    design:
      view: citation
      citation_style: APA
      spacing:
        padding: [0, 0, 0, 0]

  - block: collection
    id: talks
    content:
      title: Lectures & Talks
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
      page_type: post
      count: 5
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      offset: 0
      order: desc
    design:
      view: date-title-summary
      spacing:
        padding: [0, 0, 0, 0]
---