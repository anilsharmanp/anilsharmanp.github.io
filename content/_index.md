---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        My thesis aims to study the nuclear structure of nuclei near shell closures, especially those around the doubly-magic 56Ni core. Both experimental methods—such as in-beam gamma-ray spectroscopy with large detector arrays—and theoretical approaches using large-scale shell model calculations will be used. Nuclear excitations is the primary focus for this work, which leads us to understand the mechanism of generation of the angular momentum in nuclei. Recently, our paper on 69Ga nucleus accepted in Physics Review C journal where we established the collective excitations builds upon the single particle excitation scheme.
  
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Publications
#      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent Talks and posters
      filters:
        folders:
          - events
    design:
      view: article-grid
      columns: 2
---
