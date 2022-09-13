---
widget: slider
weight: 1
active: true
headless: true

design:
  # Slide height is automatic unless you force a specific height (e.g. '400px')
  slide_height: ''
  is_fullscreen: true
  # Automatically transition through slides?
  loop: true
  # Duration of transition between slides (in ms)
  interval: 5000

content:
  slides:
    - title: 👋 Welcome to BMU Lab
      content: Take a look at what we're working on...
      align: center
      background:
        position: right
        color: '#666'
        brightness: 0.7
        media: bmu.jpg
      link:
        icon: microscope
        icon_pack: fas
        text: Learn about our research topics
        url: ../publication/
    - title: Lunch & Learn ☕️
      content: 'Share your knowledge with the group and explore exciting new topics together!'
      align: left
      background:
        position: center
        color: '#555'
        brightness: 0.7
        media: 2.jpg
      link:
        # icon: microscope
        # icon_pack: fas
        text: 😉 Meet our members
        url: ../publication/
    - title: World-Class Medical Ultrasound Lab
      content: 'Graduate and Undergraduate Student Openings!'
      align: right
      background:
        position: center
        color: '#333'
        brightness: 0.7
        media: lib.jpg
      link:
        icon: graduation-cap
        icon_pack: fas
        text: Join Us
        url: ../contact/
---
