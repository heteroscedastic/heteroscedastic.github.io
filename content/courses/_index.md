---
title: Courses
summary: My courses
type: landing

cascade:
  - _target:
      kind: page
      path: /courses/**
    params:
      breadcrumb:
        enable: true

design:
  spacing: '5rem'

sections:
  - block: collection
    content:
      title: Courses
      text: ""
      filters:
        folders:
          - courses
        tags:
          - Course
    design:
      view: article-grid
      columns: 1
---
