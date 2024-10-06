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
      button:
        text: Download Timetable
        url: ../uploads/timetable.pdf
      # Show a call-to-action button under your biography? (optional)
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: bg.jpg
          filters:
            brightness: 0.5
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

  - block: collection
    content:
      title: HOBBY
      text: ""
      filters:
        folders:
          - hobby
        exclude_featured: false
    design:
      view: card
      columns: 3

  - block: carousel
    content:
      slides:
        - image: unsplash/school.jpg
          content_html: "Jeonbuk National University, Class of 2021"
        - image: unsplash/character.jpg
          content_html: "MBTI : INTP"
        - image: unsplash/certificate.jpg
          content_html: "Acquisition of 24-year Engineer Information Processing"
      duration: 2000
      items: 1
      height: 400
      unit: px

  - block: markdown
    id: contact
    content:
      title: "CONTACT"
      text: |-
        <p><i class="fas fa-envelope"></i> E-mail : rlawogus65@gmail.com</p>
        <p><i class="fas fa-phone"></i> TEL : 010 - 3340 - 5731</p>
        <p><i class="fas fa-map-marker-alt"></i> Loc :  7th Engineering Building of Jeonbuk National University </p>

        {{< googlemapen id="myMap" lat="35.8203" lng="127.1345" >}}
    design:
      columns: "1"
---
