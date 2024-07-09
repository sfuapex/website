---
# Leave the homepage title empty to use the site title
title: 
type: landing


sections:
  - block: hero
    content:
      title: |
        APEX Lab
      # image:
      #   filename: gp7.jpeg
      text: |
        <br>
        
        Algorithmically Principled Exploration (APEX)
        <br>
        explore broadly, venture **boldly**
  - block: slider
    content:
      slides:
      - title: Join the APEX Lab
        content: ''
        align: center
        background:
          position: center
          color: '#333'
          image:
            filename: slide/sfu.jpg
            filters:
              brightness: 0.4
          position: center
          color: '#333'
        link:
          icon: graduation-cap
          icon_pack: fas
          text: Join Us
          url: ../contact/
      - title: 
        content: ''
        align: center
        background:
          image:
            filename: slide/gp7.jpeg
            filters:
              brightness: 0.8
          position: center
          color: '#333'
      - title: 
        content: ''
        align: center
        background:
          image:
            filename: slide/gp3.jpeg
            filters:
              brightness: 0.8
          position: center
          color: '#333'
      - title: 
        content: ''
        align: center
        background:
          image:
            filename: slide/gp2.jpeg
            filters:
              brightness: 0.8
          position: center
          color: '#333'
      # - title: 
      #   content: ''
      #   align: center
      #   background:
      #     image:
      #       filename: slide/gp1.jpg
      #       filters:
      #         brightness: 0.8
      #     position: center
      #     color: '#333'
    design:
      slide_height: '350px'
      is_fullscreen: False
      loop: true
      interval: 4000
  
  
  - block: collection
    content:
      title: Latest Publications
      subtitle:
      text: 
      count: 3
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: publication
    design:
      view: card
      columns: '2'

  # - block: collection
  #   content:
  #     title: Latest Posts
  #     subtitle:
  #     text:
  #     count: 1
  #     filters:
  #       author: ''
  #       category: ''
  #       exclude_featured: false
  #       publication_type: ''
  #       tag: ''
  #     offset: 0
  #     order: desc
  #     page_type: post
  #   design:
  #     view: card
  #     columns: '1'
  
  # - block: markdown
  #   content:
  #     title: Heloooooooooooooooooooo
  #     subtitle: ''
  #     text:
  #   design:
  #     columns: '1'
  #     background:
  #       image: 
  #         filename: coders.jpg
  #         filters:
  #           brightness: 1
  #         parallax: false
  #         position: center
  #         size: cover
  #         text_color_light: true
  #     spacing:
  #       padding: ['20px', '0', '20px', '0']
  #     css_class: fullscreen
  
  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
    design:
      columns: '1'
---