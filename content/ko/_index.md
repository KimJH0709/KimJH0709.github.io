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
        text: 시간표 다운로드
        url: uploads/timetable.pdf
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
          - projects
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

  - block: collection
    content:
      title: 취미
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
          content_html: "전북대학교 21학번"
        - image: unsplash/character.jpg
          content_html: "MBTI : INTP"
        - image: unsplash/certificate.jpg
          content_html: "24년 정보처리기사 취득"
      duration: 2000
      items: 1
      height: 400
      unit: px

  - block: markdown
    id: contact
    content:
      title: "연락"
      text: |-
        <p><i class="fas fa-envelope"></i> 이메일 : rlawogus65@gmail.com</p>
        <p><i class="fas fa-phone"></i> 연락처 : 010 - 3340 - 5731</p>
        <p><i class="fas fa-map-marker-alt"></i> 위치 : 전북대학교 공과대학 7호관</p>

        {{< googlemap id="myMap" lat="35.8203" lng="127.1345" >}}
    design:
      columns: "1"
---
