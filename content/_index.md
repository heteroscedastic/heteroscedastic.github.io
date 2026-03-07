---
title: ''
summary: ''
date: 2024-01-01
type: landing

design:
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle

  - block: markdown
    content:
      title: 'Welcome to Stochastic Rambling'
      subtitle: ''
      text: |-
        Statistics of life and few other outliers!

        This is my personal space where I write about statistics, machine learning, data science, and the curious patterns we find in everyday life. Whether it's exploring Bayesian inference, visualizing interesting datasets, or just rambling about probability — you'll find it here.

        Feel free to explore my [projects](/projects/) or read the [blog](/blog/).
    design:
      columns: '1'

  - block: collection
    id: news
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      page_type: blog
      count: 5
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      offset: 0
      order: desc
    design:
      view: card
      spacing:
        padding: [0, 0, 0, 0]

  - block: collection
    content:
      title: Selected Projects
      filters:
        folders:
          - projects
    design:
      view: article-grid
      columns: 3
---
