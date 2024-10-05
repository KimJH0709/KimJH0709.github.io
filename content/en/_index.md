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
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
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

  - block: resume-skills
    id: skills
    content:
      title: SKILL
      username: admin
    design:
      show_skill_percentage: true

  - block: collection
    id: papers
    content:
      title: PROJECTS
      filters:
        folders:
          - project
        featured_only: true
    design:
      view: article-grid
      columns: 3

  - block: collection
    id: papers
    content:
      title: COMPLETION LECTURE
      filters:
        folders:
          - activity
        featured_only: true
    design:
      view: article-grid
      columns: 3

  - block: markdown
    id: contact
    content:
      title: "CONTACT"
      text: |-
        <p>E-mail : rlawogus65@gmail.com</p>
        <p>Loc :  7th Engineering Building of Jeonbuk National University </p>
        <iframe 
            width="900" 
            height="600" 
            style="border: 1px solid black" 
            loading="lazy" 
            allowfullscreen 
            src="https://www.openstreetmap.org/export/embed.html?bbox=127.1315%2C35.8449%2C127.1375%2C35.8479&layer=mapnik&marker=35.84601324617979%2C127.13444961966684">
        </iframe>
    design:
      columns: "1"
---
