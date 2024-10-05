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
      title: 스킬
      username: admin
    design:
      show_skill_percentage: true

  - block: collection
    id: papers
    content:
      title: 프로젝트
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
      title: 수강 강의
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
      title: "연락"
      text: |-
        <p>이메일 : rlawogus65@gmail.com</p>
        <p>위치 : 전북대학교 공과대학 7호관 </p>
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
