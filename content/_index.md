---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/Shariati-Resume-H2025.pdf
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
  # - block: markdown
  #   content:
  #     title: '📚 My Research'
  #     subtitle: ''
  #     text: |-
  #       Use this area to speak to your mission. I'm a research scientist in the Moonshot team at DeepMind. I blog about machine learning, deep learning, and moonshots.
# 
  #       I apply a range of qualitative and quantitative methods to comprehensively investigate the role of science and technology in the economy.
  #       
  #       Please reach out to collaborate 😃
  #   design:
  #     columns: '1'
  
  - block: resume-experience
    id: experience
    content:
      username: admin
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false
  - block: resume-skills
    id: skills
    content:
      title: Skills
      username: admin
    design:
      columns: '2'
      show_skill_percentage: true
  #- block: resume-awards
  #  content:
  #    title: Awards
  #    username: admin
  - block: resume-languages
    content:
      title: Languages
      username: admin


  - block: collection
    id: projects
    content:
      title: Project Experiences
      # subtitle: ''
      # text: ''
      # Page type to display. E.g. post, talk, publication...
      # page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 0
      # Filter on criteria
      filters:
        folders:
          - project
        featured_only: false
        # author: ""
        # category: ""
        # tag: ""
        # exclude_featured: false
        # exclude_future: false
        # exclude_past: false
        # publication_type: ""
      # Choose how many pages you would like to offset by
      # offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      #order: desc
    design:
      # Choose a layout view
      view: showcase #card #date-title-summary
      columns: '2'
      # Reduce spacing
      # spacing:
      #   padding: [0, 0, 0, 0]


  - block: collection
    id: papers
    content:
      title: Upcoming Publications
      filters:
        folders:
          - publication
        featured_only: true
      count: 0
    design:
      view: article-grid
      columns: 3

  - block: collection
    content:
      title: Recent Publications
      text: ""
      count: 0
      filters:
        folders:
          - publication
        exclude_featured: true #false
    design:
      view: article-grid #citation
      columns: 4
  #- block: collection
  #  id: plant #talks
  #  content:
  #    title: Plant Publications
  #    filters:
  #      folders:
  #        - event
  #  design:
  #    view: article-grid
  #    columns: 4



---
